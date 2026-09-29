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


