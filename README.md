<div align="center">

# 🚀 AI Agents Self-Learning Handbook

</div>

在 AI 驱动的时代，与 LLM 及 Agents 的协作已成为各岗位的核心能力。

无论您的职能背景如何，掌握 AI Agents 的核心知识都是应对未来挑战、提升工作效能的必要基础, 也将是你在智能时代保持竞争力的关键一步。


## 前置导读：AI Agents 高层架构概览

在正式深入之前，我们为何要先了解 Agents 的架构？这并非要求初学者立即掌握底层细节，而是旨在建立一个 High-Level 的全局认知。



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
├── 4. Agent 与工具调用【核心】
│   ├── Function Calling / Tool Use
│   ├── MCP Client / Server
│   ├── ReAct、Plan-and-Execute、工作流
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

<div align="center">

**保持好奇，持续动手 —— 祝你顺利走完这条 AI Agent 之路！** ⭐

</div>


## 📚 Reference Links

### Python 与 Web 开发基础
-   [黑马程序员 - Python 全套教程](https://www.bilibili.com/video/BV1qW4y1a7fU)
-   [FastAPI Full Course](https://www.youtube.com/watch?v=0sOvCWFmrtA)
-   [Fluent Python 2nd Edition](https://www.oreilly.com/library/view/fluent-python-2nd/9781492056348/part04.html)
-   [FastAPI 官方中文文档](https://fastapi.tiangolo.com/zh/)
-   [Streamlit 文档](https://docs.streamlit.io/)

### Prompt Engineering 与 AI 应用平台
-   [吴恩达 - ChatGPT Prompt Engineering](https://www.bilibili.com/video/BV1Mo4y1p7iH)
-   [Prompt Engineering Guide](https://www.promptingguide.ai/zh)
-   [Dify Official Tutorials](https://www.youtube.com/@DifyAI)
-   [Dify 官方文档](https://docs.dify.ai/v/zh-hans)

### 大模型理论与 NLP 基础
-   [Andrej Karpathy - Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY)
-   [3Blue1Brown - 深度学习之神经网络](https://www.bilibili.com/video/BV1bx411M7Zx)
-   [The Illustrated Transformer（图解 Transformer）](https://jalammar.github.io/illustrated-transformer/)
-   [Hugging Face NLP Course](https://huggingface.co/learn/nlp-course/zh-CN/chapter1/1)

### RAG 与 LangChain 应用开发
-   [吴恩达 - 基于 LangChain 的大模型应用开发](https://www.bilibili.com/video/BV1Ku4y1T7qz)
-   [RAG 高级技巧详解](https://www.bilibili.com/video/BV15c411F7Z1)
-   [LangChain Python 文档](https://python.langchain.com/docs/get_started/introduction)
-   [Milvus 中文文档](https://milvus.io/docs/zh-CN)
-   [BGE M3 Embedding](https://huggingface.co/BAAI/bge-m3) — 当前最佳开源多语言 Embedding 模型

### AI Agents 与多智能体系统
-   [DeepLearning.AI - AI Agents in LangGraph](https://learn.deeplearning.ai/courses/ai-agents-in-langgraph)
-   [多智能体系统开发：AutoGen vs CrewAI vs LangGraph](https://www.bilibili.com/video/BV1Jw411h7Z5)
-   [LangGraph 官方文档](https://langchain-ai.github.io/langgraph/)
-   [OpenAI Function Calling 指南](https://platform.openai.com/docs/guides/function-calling)
-   [ReAct: Synergizing Reasoning and Acting](https://react-lm.github.io/)

### 模型微调与推理部署
-   [LLaMA-Factory 官方教学：从零微调大模型](https://www.bilibili.com/video/BV1hK421d74W)
-   [LoRA & QLoRA Explained](https://www.youtube.com/watch?v=1YmO4f5E34s)
-   [LLaMA-Factory GitHub](https://github.com/hiyouga/LLaMA-Factory)
-   [vLLM 文档](https://docs.vllm.ai/en/latest/)

### 图像生成与 Diffusion 模型
-   [秋叶 - Stable Diffusion 保姆级入门教程](https://www.bilibili.com/video/BV1iM4y1y7oA)
-   [Hugging Face Diffusion Models Course](https://www.youtube.com/watch?v=sFztFnnclbg)
-   [Stable Diffusion Art Tutorials](https://stable-diffusion-art.com/)
-   [Diffusers 官方文档](https://huggingface.co/docs/diffusers/index)

