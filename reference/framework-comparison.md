# 🔧 Agent 框架对比指南

对应知识体系 **第 4 层（Agent 与工具调用）** 与 **第 5 层（Runtime 与生产化）**。

选框架的核心问题不是"哪个最强"，而是**"我的编排复杂度需要多强的控制力"**。

---

## 速查表

| 维度 | LangGraph | CrewAI | AutoGen | Pydantic AI |
| --- | --- | --- | --- | --- |
| 出品方 | LangChain | CrewAI Inc. | Microsoft | Pydantic 团队 |
| 核心抽象 | 有向图状态机 | Crew / Agent / Task | 可对话 Agent 群组 | 类型化 Agent 函数 |
| 编排方式 | 显式定义节点与边 | 角色分工 + 流程模板 | Agent 间自由对话 | 代码即流程 |
| 控制粒度 | 最细 | 中 | 粗（靠对话收敛） | 细（但偏单 Agent） |
| 状态持久化 | 内置 Checkpointer | 较弱 | 较弱 | 需自行实现 |
| Human-in-the-Loop | 内置中断/恢复 | 有限支持 | 支持（人类作为 Agent） | 需自行实现 |
| 可观测性 | LangSmith 原生 | 基础日志 | 基础日志 | Logfire 原生 |
| 学习曲线 | 陡 | 平缓 | 中 | 平缓 |
| 生产成熟度 | 高 | 中 | 中（偏研究） | 中上 |

---

## LangGraph

**是什么**：把 Agent 建模成一张有向图 —— 节点是步骤（调模型、调工具、人工审批），边是状态流转条件。

**适合**
- 流程需要**确定性**：什么时候循环、什么时候中断、什么时候走人工，都要能画出来
- 需要 Checkpoint / 断点续跑 / 时间旅行调试
- 已经在用 LangChain 生态（LangSmith 追踪、各类 Tool 封装）

**不适合**
- 只想快速做个 Demo —— 图的定义本身就有不少样板代码

**关键能力**
- `StateGraph` 显式状态定义，天然契合第 5 层的"会话状态 / 任务状态"
- `interrupt()` 实现 Human-in-the-Loop，人工审批后从断点恢复
- Checkpointer 支持 SQLite / Postgres 持久化

📖 https://langchain-ai.github.io/langgraph/

---

## CrewAI

**是什么**：用"公司团队"作比喻 —— 给每个 Agent 一个角色（Role）、目标（Goal）、背景故事（Backstory），然后派发 Task。

**适合**
- 任务天然可按**角色**拆分（研究员 → 分析师 → 撰稿人）
- 快速验证多 Agent 协作想法，代码量最少
- 团队里非资深工程师也要能读懂流程

**不适合**
- 需要精确控制每一步分支的场景 —— 角色抽象会把控制权交给 LLM
- 对状态持久化、失败重试有硬性要求的生产系统

**关键能力**
- `Sequential` / `Hierarchical` 两种内置流程
- 角色化 Prompt 自动生成，省掉大量 Prompt 工程

📖 https://docs.crewai.com/

---

## AutoGen

**是什么**：微软出品，把 Agent 建模成**会聊天的参与者**，通过多轮对话自发收敛到答案。

**适合**
- 探索性任务：解法不确定，让 Agent 互相质疑、迭代
- 需要代码执行闭环（内置 Code Executor + 沙箱）
- 研究场景、论文复现

**不适合**
- 对成本敏感 —— 自由对话轮次不可控，Token 消耗容易失控
- 需要可预测延迟的线上服务

**关键能力**
- `GroupChat` + `GroupChatManager` 管理多 Agent 发言顺序
- `UserProxyAgent` 让人类作为对话参与者介入
- 内置 Docker 沙箱执行代码（对应第 5 层的 Sandbox 要求）

📖 https://microsoft.github.io/autogen/

---

## Pydantic AI

**是什么**：Pydantic 团队出品，把 Agent 当普通 Python 函数写，用类型系统约束输入输出。

**适合**
- 强调 **Structured Output**（第 2 层核心要求）—— 返回值就是 Pydantic Model，自带校验
- 单 Agent + 多工具的场景，不需要复杂编排
- 已有 FastAPI / Pydantic 技术栈，想无缝接入

**不适合**
- 复杂多 Agent 编排 —— 框架刻意不提供重量级编排抽象

**关键能力**
- 依赖注入（Dependency Injection）传递运行时上下文
- 类型安全的 Tool 定义，IDE 能直接补全
- Logfire 原生集成，开箱即用的追踪

📖 https://ai.pydantic.dev/

---

## 怎么选

```
需要精确控制流程 / 断点续跑 / 人工审批？
  └─ 是 → LangGraph

任务能按角色清晰拆分，且想快速出原型？
  └─ 是 → CrewAI

需要 Agent 互相博弈、探索性求解 + 代码执行？
  └─ 是 → AutoGen

单 Agent 多工具，最看重输出结构化与类型安全？
  └─ 是 → Pydantic AI
```

**给本项目学习路径的建议**：

- **Step 2（第 4 层）**：先用 **Pydantic AI** 或裸 OpenAI SDK 手写一遍 Function Calling 循环。不要一上来就用框架 —— 不手写一次，永远不知道框架帮你藏了什么。
- **Step 3（第 4-5 层）**：转 **LangGraph**。状态管理、Checkpoint、Human-in-the-Loop 这三件事它做得最完整，正好覆盖第 5 层的要求。
- **Step 4 及之后（第 7 层）**：需要多 Agent 时再评估 CrewAI / AutoGen。

---

## 选型时容易踩的坑

**1. 框架锁定（Vendor Lock-in）**
把业务逻辑写进框架的抽象里，换框架时等于重写。建议：工具函数、Prompt 模板、数据访问层保持框架无关，只让编排层依赖框架。

**2. 用框架逃避理解**
框架把 Function Calling 的请求/响应循环包起来了，但线上出问题时你还是得看原始 Tool Call。对应知识体系第 4 层 —— 先懂原理再用框架。

**3. 忽略成本可观测性**
多 Agent 框架的 Token 消耗是单 Agent 的数倍且难以预估。接框架的同时就要接上 LangSmith / Langfuse（第 6 层要求），不要等账单出来才补。

**4. 拿 Multi-Agent 解决单 Agent 问题**
大多数业务场景，一个 Agent + 设计良好的工具集就够了。Multi-Agent 带来的调试成本和不确定性通常大于收益。

---

## 相关资源

- [多智能体系统开发：AutoGen vs CrewAI vs LangGraph](https://www.bilibili.com/video/BV1Jw411h7Z5)
- [Anthropic - Building Effective Agents](https://www.anthropic.com/research/building-effective-agents) — 何时该用 Agent，何时用 Workflow
- [DeepLearning.AI - AI Agents in LangGraph](https://learn.deeplearning.ai/courses/ai-agents-in-langgraph)

---

**返回**：[项目首页](../README.md) ｜ [完整学习资源](./learning-resources.md)
