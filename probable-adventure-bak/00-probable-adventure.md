<div align="center">
  
# 🚀 probable-adventure  
## AI 大模型与智能体开发 · 全栈自学路线图

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![LangChain](https://img.shields.io/badge/LangChain-121212?style=flat-square&logo=langchain&logoColor=white)](https://www.langchain.com/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=FastAPI&logoColor=white)](https://fastapi.tiangolo.com/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com/)

> **从零基础到企业级 AI Agent 开发**  
> 深度贴合真实业务需求，以 **RAG** 和 **Agent** 为核心，覆盖全栈技术路线：  
> 构建 → 优化 → 微调 → 私有化部署

</div>

---

## 📚 技术栈总览

| 类别               | 工具/框架                                                                 |
| ------------------ | ------------------------------------------------------------------------- |
| **语言 & 后端**    | Python, FastAPI, Flask                                                    |
| **前端可视化**     | Streamlit, Gradio                                                         |
| **核心框架**       | LangChain, LangGraph, LlamaIndex                                          |
| **大模型生态**     | HuggingFace, Transformers, OpenAI API, Ollama                             |
| **向量 & 数据库**  | Milvus, Faiss, ElasticSearch, MySQL, Neo4j                                |
| **微调与部署**     | LoRA, LLaMA-Factory, DeepSpeed, vLLM, Docker                              |

---

## 🗺️ 学习路径 & 进度追踪

> ✅ 每完成一项请勾选 `[x]`，建议按顺序推进，也可根据兴趣跳跃学习。

### 📌 阶段一：编程基石与数据处理  
**目标**：掌握 Python 高阶编程，独立完成后端服务与可视化界面搭建。

- [ ] Python 进阶（基础数据结构、控制流、函数式编程、OOP、异常处理…）
- [ ] 并发编程（多线程、多进程、互斥锁、并发/并行）
- [ ] 网络编程与 API 开发（FastAPI/Flask，RESTful）
- [ ] 数据分析基础（Numpy, Pandas, SQL 复杂查询）
- [ ] 可视化 Web UI 构建（**Streamlit 必学**）

📁 **实战项目**：`01_Basic_Chatbot` – 使用 Python + Streamlit + API 搭建带 Web 界面的简易对话机器人

---

### 📌 阶段二：Prompt 工程与低代码 Agent  
**目标**：建立“AI 指挥官”思维，快速落地业务级智能体。

- [ ] 高阶提示词技巧（Zero-shot, Few-shot, COT 思维链…）
- [ ] 低代码平台实战（Coze 工作流编排、多 Agent 协同）
- [ ] Dify 平台深度实战（知识库构建、Docker 私有化部署）
- [ ] Ollama 本地模型部署（DeepSeek, Qwen 等）

📁 **实战项目**：`02_Interview_Agent` – 基于 Coze/Dify 搭建模拟面试官（解析简历+多轮对话）

---

### 📌 阶段三：大模型核心理论与 NLP 基础  
**目标**：拒绝“调包侠”，深入理解 Transformer 底层原理。

- [ ] 机器学习与深度学习基础
- [ ] PyTorch 框架基础（张量操作、简易神经网络）
- [ ] NLP 核心技术（分词、Word Embedding、FastText）
- [ ] Transformer 架构剖析（Encoder, Decoder, Attention）
- [ ] 主流模型演进（BERT, GPT, DeepSeek）
- [ ] HuggingFace 深度指北（下载、加载、Pipeline）

📁 **实战项目**：`03_Text_Classification` – 基于 BERT/FastText 构建新闻文本快速分类系统

---

### 📌 阶段四：RAG 系统开发 ⭐️ 核心  
**目标**：解决模型“幻觉”，让 AI 掌握企业私有领域知识。

- [ ] LangChain 核心组件全解（Models, Prompts, Memory, Chains…）
- [ ] 向量数据库实战（Milvus, Faiss, ElasticSearch）
- [ ] 文档处理与切分策略（Chunking, Embedding）
- [ ] 高阶 RAG 优化 I：Query 改写、路由策略
- [ ] 高阶 RAG 优化 II：重排序 (Rerank)、混合检索 (BM25+Dense)

📁 **实战项目**：`04_HR_Resume_RAG` – 智能简历推荐系统（异构数据解析 + 多轮对话筛选）

---

### 📌 阶段五：高阶 Agent 与多智能体系统 ⭐️ 核心  
**目标**：赋予 AI “手和眼”，实现自主规划与多智能体协同。

- [ ] Agent 核心架构（ReAct 范式：Thought→Action→Observation）
- [ ] 工具调用（Function Calling / MCP 协议集成）
- [ ] API 自动化系统（读写数据库、调用第三方 API）
- [ ] LangGraph 深度实战（状态机编排复杂工作流）
- [ ] 多智能体协作（A2A, Multi-Agent 架构）

📁 **实战项目**：`05_Smart_Voyage_Agent` – 多意图旅行助手（路由/天气/购票多 Agent 协同）

---

### 📌 阶段六：大模型微调与私有化部署 🚀 进阶  
**目标**：打造垂直领域专属大模型，具备生产级部署能力。

- [ ] PEFT 微调理论（LoRA, QLoRA, P-Tuning）
- [ ] 微调数据准备与清洗（QA 对、格式转换）
- [ ] 微调框架实战（LLaMA-Factory / DeepSpeed）
- [ ] 模型量化与加速部署（GPTQ, AWQ, vLLM）
- [ ] （可选）知识图谱与 GraphRAG（Neo4j 集成）

📁 **实战项目**：`06_LLM_Finetuning` – 基于开源模型 + LoRA 微调，实现垂直领域信息抽取

---

### 📌 阶段七：多模态大模型开发 🎨 拓展  
**目标**：处理图像、声音等非文本数据，拓宽应用边界。

- [ ] 计算机视觉基础（CNN, ResNet, YOLO, U-Net）
- [ ] Stable Diffusion 原理与模型构建
- [ ] SD 高级应用（LoRA 微调、图生图、ControlNet）

📁 **实战项目**：`07_Multimodal_App` – 基于 Stable Diffusion 的特定风格图像生成工具

---

## 💡 给自学者的避坑与学习建议

> **以下建议能帮你少走弯路，提升求职竞争力**

1. **按图索骥，别一上来就死磕底层算法**  
   ✅ 正确顺序：**阶段一 → 阶段二 → 阶段四 → 阶段五**（先跑通 RAG 和 Agent），**阶段三、阶段六** 用于进阶时再深入理解原理。

2. **拥抱开源社区，不必自购昂贵算力**  
   - 租用 GPU：[AutoDL](https://www.autodl.com/)、[阿里云 PAI](https://www.aliyun.com/product/bigdata/pai) 等，几十元/天。  
   - 常逛社区：**GitHub、HuggingFace、魔搭社区 (ModelScope)**，学习别人的 Agent 实现。

3. **吃透重点技术栈（企业面试核心）**  
   - 必备技能：**Python + PyTorch + LangChain/LangGraph + Milvus/Faiss + FastAPI**  
   - 加分痛点：**RAG 的召回准确率如何提升？** → 重排序(Rerank)、混合检索、Query 改写。

4. **丰富你的 GitHub / 简历作品集**  
   - 不必完全照搬示例项目，可**更换业务场景**：  
     - 原项目“医疗知识图谱” → 改做“电商法律法规 RAG 知识库”  
     - 原项目“差旅 Agent” → 改做“IT 自动运维工单 Agent”  
   - 这样既有技术验证，又能拥有**独特且立体的个人作品集**。

---

<div align="center">
  
**🎯 保持好奇，持续动手 —— 祝你顺利走完这条“probable-adventure”之路！**

⭐️ 如果这个路线对你有帮助，欢迎给仓库点个 Star ~

</div>
