### 1. GitHub 高 Star 路线图与项目

| 项目名称 / 仓库 | 社区认可度 (Star) | 核心内容与适合人群 |
| --- | --- | --- |
| **`mlabonne/llm-course`** | **83k+ ⭐** | **全网最火的 LLM & AI 工程师课程。** 包含了完整的学习路径，从 Transformer 基础到 RAG、Tool Calling、Agent 编排与模型部署，附带丰富可运行的 Colab Notebooks。 |
| **`ashishpatel26/500-AI-Agents-Projects`** | **高关注度开源库** | **智能体实战案例库。** 汇总了 500+ 个不同行业（医疗、金融、代码生成等）的 Agent 落地项目，分类整理了 CrewAI、LangGraph、AutoGen、Agno 等框架的使用场景。 |


### 2. 权威平台交互式路线图

* **roadmap.sh — AI Engineer Roadmap (`roadmap.sh/ai-engineer`)**
* **权威性：** 开发者社区最流行的交互式路线图标准（包含 AI Agent 专区）。
* **学习路径：** Python / API 基础 $\rightarrow$ LLM & Prompt $\rightarrow$ RAG 与向量数据库 $\rightarrow$ **AI Agents（ReAct 模式、Tool Calling、Multi-Agent、LangGraph / CrewAI）** $\rightarrow$ Agent 评估（Evals）、安全护栏（Guardrails）与云端部署。

### 3. 顶尖机构与官方免费实战课程

* **DeepLearning.AI（吴恩达团队短课）：** *公认最经典的 AI 微课程，每门课约 1-2 小时，直奔主题*
* *AI Agentic Design Patterns with AutoGen*：讲解 Agent 的四大核心设计模式（Reflection、Tool Use、Planning、Multi-agent collaboration）。
* *LangGraph: Building Stateful Agents*：与 LangChain 团队联合出品，手把手教你用有向图和状态机搭建带记忆、支持人机回溯（Human-in-the-loop）的复杂 Agent。
* *Building Agentic RAG with LlamaIndex*：讲解如何将传统 RAG 升级为具有路由、纠错和自我修正功能的 Agentic RAG。

* **LangChain 官方 —— LangGraph Academy**
* 官方推出的免费视频教程，专门讲解智能体在生产环境中的持久化（Persistence）、状态流转、条件路由与异常重试机制。

### 4. 智能体架构与设计哲学必读（理论基石）

* **Anthropic 官方技术指南 — *Building Effective Agents***
* **业内标杆指南：** 详细阐述了**何时该用工作流（Workflows），何时才需要自主智能体（Agents）**。对比了 Routing（路由）、Parallelization（并行）、Orchestrator-Workers（主从编排）等架构形态，是避开“过度设计”的必读文章。

* **MCP 官方文档 (`modelcontextprotocol.io`)**
* **核心标准：** 由 Anthropic 提出并迅速成为业界标准的**模型上下文协议**。学习如何将数据库、API 和本地工具标准化暴露给大模型和 Agent。


### 💡 建议的学习步骤

1. **Step 1（铺垫）：** 先通读 Anthropic 的 *Building Effective Agents*，理解 Agent 的架构本质（本质就是用 Control Loop 包装 LLM）。
2. **Step 2（单体 Agent）：** 在 `mlabonne/llm-course` 或 DeepLearning.AI 上学习 Function Calling、ReAct 范式以及 Tool/MCP 的接入。
3. **Step 3（状态机与多 Agent）：** 学习 **LangGraph**，掌握有状态（Stateful）路由与多智能体协作（Multi-Agent Systems）。
4. **Step 4（工程落地与护栏）：** 参考 `roadmap.sh/ai-engineer`，补充沙箱隔离（Sandbox）、评估（Evals，如 DeepEval/Ragas）与可观测性（LangSmith/Langfuse）。

!(dev.to)[https://dev.to/cypriantinasheaarons/the-ai-agents-roadmap-nobody-is-talking-about-2026-edition-5774#:~:text=The%20Learning%20Roadmap%20%F0%9F%9B%A3%20*%20Step%201%20%E2%80%94%20Python%20%2B%20APIs%20(Week%201)%20%F0%9F%90%8D]
