# probable-adventure 🚀 AI Agent Developer Learning Path (AI大模型与智能体开发自学路线图)

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-121212?style=for-the-badge)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=FastAPI&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

本项目记录了我从零基础转行到 **AI大模型与智能体（AI Agent）开发** 的全过程。学习路径深度贴合企业真实业务需求，以 **RAG（检索增强生成）** 和 **Agent（智能体）** 为核心方向，涵盖从基础构建到企业级私有化部署的全栈技术。

---

## 🛠️ 技术栈 (Tech Stack)

- **语言 & 后端:** Python, FastAPI, Flask
- **前端 & 可视化:** Streamlit, Gradio
- **核心框架:** LangChain, LangGraph, LlamaIndex
- **大模型生态:** HuggingFace, Transformers, OpenAI API, Ollama
- **向量检索 & 数据库:** Milvus, Faiss, ElasticSearch, MySQL, Neo4j (图数据库)
- **微调与部署:** LoRA, LLaMA-Factory, DeepSpeed, vLLM, Docker

---

## 🗺️ 学习路径与进度追踪 (Learning Path)

你可以勾选 `[x]` 来标记你的学习进度。

### 阶段一：编程基石与数据处理 
> **目标:** 掌握 Python 高阶编程，独立完成后端服务与可视化界面搭建。

- [ ] Python 进阶 (OOP、深浅拷贝、闭包、装饰器)
- [ ] 并发编程 (多线程、多进程、互斥锁)
- [ ] 网络编程与 API 开发 (FastAPI / Flask 构建 RESTful API)
- [ ] 数据分析基础 (Numpy, Pandas, SQL 复杂查询)
- [ ] 可视化 Web UI 构建 (掌握 Streamlit)
- 💻 **实战项目:** `01_Basic_Chatbot` - 使用 Python + Streamlit + API 搭建一个带 Web 界面的简易对话机器人。

### 阶段二：Prompt 工程与低代码 Agent 
> **目标:** 建立“AI指挥官”思维，熟悉工作流设计，实现快速落地。

- [ ] 高阶提示词技巧 (Zero-shot, Few-shot, COT 思维链)
- [ ] 低代码平台实战 (Coze 工作流编排、插件调用)
- [ ] Dify 平台深度实战 (知识库构建、Docker 私有化部署)
- [ ] Ollama 本地模型部署部署 (DeepSeek, Qwen 等)
- 💻 **实战项目:** `02_Interview_Agent` - 基于 Coze/Dify 搭建能解析简历并进行多轮对话的模拟面试官。

### 阶段三：大模型核心理论与 NLP 基础 
> **目标:** 拒绝“调包侠”，深入理解 Transformer 底层架构。

- [ ] PyTorch 框架基础 (张量操作、简单神经网络搭建)
- [ ] NLP 核心技术 (分词、Word Embedding、FastText)
- [ ] 深入剖析 Transformer 架构 (Encoder, Decoder, Attention 机制)
- [ ] 主流模型架构演进 (BERT, GPT, DeepSeek)
- [ ] HuggingFace 深度指北 (模型下载、加载、Pipeline 使用)
- 💻 **实战项目:** `03_Text_Classification` - 基于 BERT/FastText 构建海量新闻文本快速分类系统。

### 阶段四：RAG 系统开发 (⭐️ 核心)
> **目标:** 解决大模型“幻觉”，让 AI 掌握企业私有领域知识。

- [ ] LangChain 核心组件全解 (Models, Prompts, Memory, Chains)
- [ ] 向量数据库原理与实战 (Milvus, Faiss)
- [ ] 文档处理与切分策略 (Chunking, Embedding)
- [ ] 高阶 RAG 优化 I：Query 改写、路由策略 (Query Routing)
- [ ] 高阶 RAG 优化 II：重排序 (Rerank)、混合检索 (BM25 + Dense)
- 💻 **实战项目:** `04_HR_Resume_RAG` - 智能简历推荐系统（支持异构数据解析与多轮对话筛选）。

### 阶段五：高阶 Agent 与多智能体系统 (⭐️ 核心)
> **目标:** 赋予 AI “手和眼”，实现自主规划、工具调用与多智能体协同。

- [ ] Agent 核心架构剖析 (ReAct 范式：Thought -> Action -> Observation)
- [ ] 工具调用 (Function Calling / MCP 协议集成)
- [ ] API 自动化系统开发 (读写数据库、调用第三方 API)
- [ ] LangGraph 框架深度实战 (状态机模式编排复杂工作流)
- [ ] 多智能体协作机制 (A2A, Multi-Agent 架构)
- 💻 **实战项目:** `05_Smart_Voyage_Agent` - 多意图旅行助手（集成路由 Agent、天气查询 Agent、购票 Agent）。

### 阶段六：大模型微调与私有化部署 (🚀 进阶)
> **目标:** 掌握参数高效微调，打造垂直领域专属大模型。

- [ ] PEFT 微调理论 (LoRA, QLoRA, P-Tuning)
- [ ] 微调数据准备与清洗 (QA 对构造、数据格式转换)
- [ ] 微调框架实战 (LLaMA-Factory / DeepSpeed)
- [ ] 模型量化与加速部署 (GPTQ, AWQ, vLLM 推理加速)
- [ ] (可选) 知识图谱与 GraphRAG (Neo4j 集成)
- 💻 **实战项目:** `06_LLM_Finetuning` - 基于开源模型 + LoRA 微调，实现垂直业务领域的特定信息抽取。

### 阶段七：多模态大模型开发 (🎨 拓展)
> **目标:** 掌握 AIGC 图文生成技术，拓宽应用边界。

- [ ] 计算机视觉基础 (CNN, ResNet, YOLO 简介)
- [ ] Stable Diffusion 原理与模型构建
- [ ] SD 高级应用 (LoRA 微调、图生图、ControlNet)
- 💻 **实战项目:** `07_Multimodal_App` - 基于 Stable Diffusion 的特定风格图像生成小工具。

---

## 📂 仓库目录结构指南

```text
├── 01_Python_and_Backend/     # 阶段一：基础与 Web UI
├── 02_Prompt_and_LowCode/     # 阶段二：提示词与 Dify/Coze 实践
├── 03_LLM_Theory_NLP/         # 阶段三：PyTorch 与 Transformer
├── 04_Advanced_RAG/           # 阶段四：RAG 系统与向量数据库
├── 05_Agent_Systems/          # 阶段五：LangGraph 与多智能体
├── 06_Finetuning_Deploy/      # 阶段六：微调脚本与 Docker 部署
├── 07_Multimodal_AIGC/        # 阶段七：多模态与 SD
└── README.md
