# 📚 完整学习资源列表

本文档包含按知识体系分层的详细学习资源。知识体系总览与学习路径见 [项目首页](../README.md)

---

## 第 1 层：软件基础

### Python 编程与开发

| 资源                        | 链接                                                                               | 说明                  |
| ------------------------- | -------------------------------------------------------------------------------- | ------------------- |
| 黑马程序员 - Python 全套教程       | https://www.bilibili.com/video/BV1qW4y1a7fU                                      | 中文视频教程，适合初学者        |
| Fluent Python 2nd Edition | https://www.oreilly.com/library/view/fluent-python-2nd/9781492056348/part04.html | Python 进阶书籍，重点讲 OOP |

### FastAPI 与 Web 框架

| 资源                  | 链接                                          | 说明               |
| ------------------- | ------------------------------------------- | ---------------- |
| FastAPI Full Course | https://www.youtube.com/watch?v=0sOvCWFmrtA | 完整的 FastAPI 课程视频 |
| FastAPI 官方中文文档      | https://fastapi.tiangolo.com/zh/            | 官方文档中文版          |
| Streamlit 文档        | https://docs.streamlit.io/                  | 快速构建 ML 应用的框架    |

---

## 第 2 层：LLM 应用基础

### Transformer 与深度学习理论

| 资源                                             | 链接                                                       | 说明                  |
| ---------------------------------------------- | -------------------------------------------------------- | ------------------- |
| Andrej Karpathy - Let's build GPT from scratch | https://www.youtube.com/watch?v=kCc8FmEb1nY              | 从零开始实现 GPT，深入理解原理   |
| 3Blue1Brown - 深度学习之神经网络                        | https://www.bilibili.com/video/BV1bx411M7Zx              | 直观理解神经网络（中文字幕）      |
| The Illustrated Transformer                    | https://jalammar.github.io/illustrated-transformer/      | 图解 Transformer，易于理解 |
| Hugging Face NLP Course                        | https://huggingface.co/learn/nlp-course/zh-CN/chapter1/1 | 官方免费 NLP 课程         |

### Prompt Engineering

| 资源                               | 链接                                          | 说明               |
| -------------------------------- | ------------------------------------------- | ---------------- |
| 吴恩达 - ChatGPT Prompt Engineering | https://www.bilibili.com/video/BV1Mo4y1p7iH | 简短精炼的 Prompt 工程课 |
| Prompt Engineering Guide         | https://www.promptingguide.ai/zh            | 完整的 Prompt 技巧指南  |

### LLM 应用平台与工具

| 资源                      | 链接                              | 说明             |
| ----------------------- | ------------------------------- | -------------- |
| Dify Official Tutorials | https://www.youtube.com/@DifyAI | Dify 官方教程频道    |
| Dify 官方文档               | https://docs.dify.ai/v/zh-hans  | 低代码 LLM 应用构建平台 |

---

## 第 3 层：RAG 与数据语义

### RAG 技术与框架

| 资源                          | 链接                                                         | 说明               |
| --------------------------- | ---------------------------------------------------------- | ---------------- |
| 吴恩达 - 基于 LangChain 的大模型应用开发 | https://www.bilibili.com/video/BV1Ku4y1T7qz                | LangChain 应用开发入门 |
| RAG 高级技巧详解                  | https://www.bilibili.com/video/BV15c411F7Z1                | 深入讲解 RAG 的各种优化技巧 |
| LangChain Python 文档         | https://python.langchain.com/docs/get_started/introduction | LangChain 官方文档   |

### 向量数据库与 Embedding

| 资源               | 链接                                 | 说明                      |
| ---------------- | ---------------------------------- | ----------------------- |
| Milvus 中文文档      | https://milvus.io/docs/zh-CN       | 开源向量数据库，适合 RAG          |
| BGE M3 Embedding | https://huggingface.co/BAAI/bge-m3 | 当前最佳的开源多语言 Embedding 模型 |

---

## 第 4 层：Agent 与工具调用 ⭐

### Agent 综合教程与项目

| 资源                                       | 社区热度       | 链接                                                      | 说明                        |
| ---------------------------------------- | ---------- | ------------------------------------------------------- | ------------------------- |
| **mlabonne/llm-course**                  | **83k+ ⭐** | https://github.com/mlabonne/llm-course                  | 完整的 LLM 工程师课程，包含 Agent 模块 |
| **ashishpatel26/500-AI-Agents-Projects** | **高关注**    | https://github.com/ashishpatel26/500-AI-Agents-Projects | 500+ 个 Agent 实战项目案例库      |

### Agent 设计模式与框架

| 资源                                                    | 链接                                                              | 说明                           |
| ----------------------------------------------------- | --------------------------------------------------------------- | ---------------------------- |
| DeepLearning.AI - AI Agentic Design Patterns          | https://learn.deeplearning.ai/courses/ai-agents-in-langgraph    | 学习 Agent 的 4 大核心设计模式         |
| DeepLearning.AI - LangGraph: Building Stateful Agents | https://learn.deeplearning.ai/courses/langgraph                 | 构建有状态的、支持人机交互的复杂 Agent       |
| DeepLearning.AI - Building Agentic RAG                | https://www.deeplearning.ai/short-courses/building-agentic-rag/ | 将 RAG 升级为具有自我纠正的 Agentic RAG |
| LangGraph Academy                                     | https://langchain-ai.github.io/langgraph/                       | LangChain 官方出品的 LangGraph 教程 |

### Function Calling 与工具集成

| 资源                                      | 链接                                                       | 说明                                  |
| --------------------------------------- | -------------------------------------------------------- | ----------------------------------- |
| OpenAI Function Calling 指南              | https://platform.openai.com/docs/guides/function-calling | OpenAI 官方 Function Calling 文档       |
| ReAct: Synergizing Reasoning and Acting | https://react-lm.github.io/                              | ReAct 模式的原始论文与讲解                    |
| 多智能体系统开发对比                              | https://www.bilibili.com/video/BV1Jw411h7Z5              | AutoGen vs CrewAI vs LangGraph 对比分析 |

### MCP 协议与标准化工具集成

| 资源                                         | 链接                                                           | 说明                            |
| ------------------------------------------ | ------------------------------------------------------------ | ----------------------------- |
| MCP 官方文档                                   | https://modelcontextprotocol.io                              | Anthropic 提出的标准化工具集成协议        |
| Anthropic 官方指南 - Building Effective Agents | https://www.anthropic.com/research/building-effective-agents | 何时用 Agent，何时用 Workflow，架构设计哲学 |

### Agent 框架对比

详见：[reference/framework-comparison.md](./framework-comparison.md)

主要框架：

- **CrewAI** - 面向团队协作的 Agent 框架
- **AutoGen** - 微软出品，支持多智能体通信
- **LangGraph** - LangChain 出品，基于有向图的状态机 Agent

---

## 第 5 层：Runtime 与生产化

### 状态管理与持久化

| 资源                | 链接                                        | 说明                          |
| ----------------- | ----------------------------------------- | --------------------------- |
| LangGraph Academy | https://langchain-ai.github.io/langgraph/ | 讲解 Persistence、状态流转、异常重试    |
| LangSmith 文档      | https://smith.langchain.com/              | LangChain 官方的 Agent 监控和调试工具 |

### 部署与可观测性

| 资源                       | 链接                             | 说明                |
| ------------------------ | ------------------------------ | ----------------- |
| Langfuse 文档              | https://langfuse.com/          | 开源的 LLM 应用可观测性平台  |
| roadmap.sh - AI Engineer | https://roadmap.sh/ai-engineer | 完整的工程化路线图，涵盖部署和监控 |

---

## 第 6 层：安全、治理与评测

### Agent 评估与测试框架

| 资源       | 链接                                          | 说明              |
| -------- | ------------------------------------------- | --------------- |
| DeepEval | https://github.com/confident-ai/deepeval    | Agent 离线评估框架    |
| Ragas    | https://github.com/explodinggradients/ragas | RAG/Agent 的评估框架 |

### 安全与防护

| 资源                                          | 链接                             | 说明                            |
| ------------------------------------------- | ------------------------------ | ----------------------------- |
| roadmap.sh - AI Engineer (Security Section) | https://roadmap.sh/ai-engineer | Prompt Injection、Tool 安全、权限控制 |

---

## 第 7 层：高级专题

### 多智能体系统

| 资源         | 链接                                          | 说明              |
| ---------- | ------------------------------------------- | --------------- |
| 多智能体系统开发对比 | https://www.bilibili.com/video/BV1Jw411h7Z5 | 多 Agent 协作的实现方式 |

### 模型微调与推理优化

| 资源                     | 链接                                          | 说明                    |
| ---------------------- | ------------------------------------------- | --------------------- |
| LLaMA-Factory 官方教学     | https://www.bilibili.com/video/BV1hK421d74W | 从零微调大模型，包含 LoRA、QLoRA |
| LLaMA-Factory GitHub   | https://github.com/hiyouga/LLaMA-Factory    | 开源的大模型微调框架            |
| LoRA & QLoRA Explained | https://www.youtube.com/watch?v=1YmO4f5E34s | 微调技术深入讲解              |
| vLLM 文档                | https://docs.vllm.ai/en/latest/             | 高性能的 LLM 推理引擎         |

### Coding Agent 与浏览器 Agent

| 资源    | 链接  | 说明                |
| ----- | --- | ----------------- |
| (待更新) |     | Coding Agent 专题资源 |
| (待更新) |     | 浏览器 Agent 专题资源    |

---

## 🎯 按学习路径推荐

### 快速入门路线（4 周）

1. Anthropic - Building Effective Agents（1 周）
2. DeepLearning.AI - AI Agentic Design Patterns（1 周）
3. DeepLearning.AI - LangGraph（1 周）
4. 实战项目（1 周）

### 深度学习路线（10 周）

1. mlabonne/llm-course（完整学习，3 周）
2. 所有 DeepLearning.AI 课程（3 周）
3. roadmap.sh AI Engineer 路线图（2 周）
4. 开源项目学习与贡献（2 周）

---

## 📝 资源使用建议

**质量优先**：选择 DeepLearning.AI、Anthropic、LangChain 等官方和知名机构的资源

**按需选取**：不需要学完所有资源，根据自己的目标选择相关部分

**理论+实践**：看完理论视频后，立即用代码实现，加深理解

**定期更新**：这个领域发展很快，定期查看官方文档和最新课程
