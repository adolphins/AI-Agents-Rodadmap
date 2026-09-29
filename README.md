# 🚀 AI Agents 学习路线图

在 AI 驱动的时代，与 LLM 及 Agents 的协作已成为各岗位的核心能力。本项目是一份系统的 **AI Agents 学习路线图和资源集合**，旨在帮助开发者从零开始掌握 Agent 的核心知识。

---

## 核心知识体系（7 层）

```
AI Agent 工程师知识体系
│
├── 1. 软件基础【必须】
│   ├── Python Advance(OOP / Concurrent)、Git
│   └── HTTP / API / JSON / FastAPI
│
├── 2. LLM 应用基础【必须】
│   ├── Transformer / Token / Embedding：理解原理
│   ├── Prompt 与 Context Engineering
│   ├── LLM API、流式输出、成本与延迟
│   └── Structured Output：JSON Schema / Pydantic / 校验
│
├── 3. RAG 与数据语义【必须】
│   ├── 文档解析、分块、Embedding、检索、重排
│   ├── 引用来源、检索评测、索引更新
│   ├── Semantic Layer：指标、维度、实体、血缘
│   └── 受控 Metric API，避免 Agent 任意写 SQL
│
├── 4. Agent 与工具调用【核心】 ⭐
│   ├── Agent 核心概念、特征、对比
│   ├── Function Calling 原理与 Tool 设计
│   ├── 四大设计模式（Reflection / Tool Use / Planning / Multi-Agent）
│   ├── 三种工作流（ReAct / Plan-Execute / Router）
│   ├── MCP 协议与标准化工具集成
│   ├── API、数据库、SaaS、浏览器等工具集成
│   └── Human-in-the-Loop 人工审批
│
├── 5. Runtime 与生产化【核心】
│   ├── 会话状态、任务状态、Checkpoint
│   ├── 重试、超时、异步任务、并发
│   ├── Sandbox、权限传递、工具限权
│   ├── API Gateway、限流、缓存、模型降级
│   └── 部署、日志、监控、成本控制
│
├── 6. 安全、治理与评测【全程贯穿】
│   ├── Prompt Injection 与 Tool 安全
│   ├── Trace、审计、Token / Cost 监控
│   └── RAG / Agent 离线评测与回归测试
│
└── 7. 高级专题【后置】
    ├── Multi-Agent
    ├── Agentic RAG / GraphRAG
    ├── Coding Agent / Browser Agent
    ├── Fine-tuning、量化、自托管模型
    └── 推理优化：vLLM / TGI
```

### 知识体系说明

- **第 1-3 层**：基础铺垫，必须掌握
- **第 4-5 层**：Agent 的核心，最关键的两层
- **第 6 层**：全程贯穿于前面所有层次（非可选）
- **第 7 层**：进阶专题，根据应用场景选取

---

## 学习规划

| Step  | 对应层级    | 预计时间  | 学习目标            |
| ----- | ------- | ----- | --------------- |
| **1** | 第 1-3 层 | 5-7 天 | 理解 Agent 架构本质   |
| **2** | 第 4 层   | 2-3 周 | 掌握工具调用机制        |
| **3** | 第 4-5 层 | 2-3 周 | 学习 Agent 编排与生产化 |
| **4** | 第 5-6 层 | 1-2 周 | 确保安全与可观测性       |

**总计：6-10 周 从入门到生产级别**

---

## 📚 项目结构

```
AI-Agents-Rodadmap/
├── README.md （你在这里）
├── docs/ （知识体系详解）
│   ├── README.md （使用说明）
│   ├── 01-software-basics.md
│   ├── 02-llm-basics.md
│   ├── 03-rag-semantic.md
│   ├── 04-agent-tools.md ⭐ 核心层
│   ├── 05-runtime-production.md
│   ├── 06-security-governance.md
│   └── 07-advanced-topics.md
└── reference/ （学习资源）
    ├── learning-resources.md （详细学习资源列表）
    ├── reference-links.md （50+ 参考链接）
    └── framework-comparison.md （框架对比：LangGraph/CrewAI/AutoGen）
```

---

## 🎯 如何使用本项目

### 第 1 步：了解知识体系

仔细阅读上面的"核心知识体系"，理解 7 层结构和学习路径。

### 第 2 步：根据学习进度选择资源

根据 Step 1-4，参考相应的学习资源：

- 📖 [完整学习资源列表](./reference/learning-resources.md) - 按知识体系分层推荐
- 🔗 [参考链接汇总](./reference/reference-links.md) - 所有推荐资源的链接
- 🔧 [框架对比指南](./reference/framework-comparison.md) - 选择合适的框架

### 第 3 步：深入学习

根据学习进度，阅读 `docs/` 目录中对应的详解文件：

- **Step 1** → [docs/01-03](./docs/) （基础知识）
- **Step 2** → [docs/04](./docs/04-agent-tools.md) （Agent 核心）
- **Step 3** → [docs/04-05](./docs/) （编排与生产化）
- **Step 4** → [docs/06](./docs/06-security-governance.md) （安全与治理）

### 第 4 步：动手实践

- 完成推荐课程中的代码练习
- 用选定的框架实现简单 Agent
- 基于自己的应用场景设计方案

---

## 📄 许可证

本项目采用 MIT License，详见 [LICENSE](./LICENSE)
