# 🔍 阶段四：RAG 系统与向量数据库开发

> **"Give AI a proper brain."** 
> 大模型知道的只是过去的通用知识，RAG（检索增强生成）技术能让大模型随时查阅企业私有数据，消除“幻觉”，是目前企业落地最广泛的技术。

## 🎯 核心目标
1. 熟练掌握 **LangChain** 框架的核心理念与常用组件。
2. 掌握文档处理策略（Chunking）与向量化（Embedding）。
3. 熟练使用 **Milvus** / **Faiss** 等向量数据库进行 CRUD 与检索。
4. 突破基础 RAG 瓶颈，掌握高阶 RAG 优化技巧（Query 改写、重排序 Rerank、混合检索）。

---

## 📚 优质学习资源推荐

### 📺 视频教程
* [YouTube] [LangChain Crash Course](https://www.youtube.com/watch?v=lG7Uxts9QXs)
* [Bilibili] [吴恩达联合 LangChain 创始人：基于 LangChain 的大模型应用开发](https://www.bilibili.com/video/BV1Ku4y1T7qz)
* [Bilibili] [RAG 高级技巧详解（Query改写/Rerank/HyDE）](https://www.bilibili.com/video/BV15c411F7Z1)

### 📖 文章与指南
* [LangChain 官方文档 (Python)](https://python.langchain.com/docs/get_started/introduction)
* [Milvus 中文官方文档](https://milvus.io/docs/zh-CN)
* [BGE M3 Embedding 模型介绍](https://huggingface.co/BAAI/bge-m3) *(目前非常好用的开源多语言 Embedding 模型)*

---

## 💻 练习与代码记录

- [ ] **`01_langchain_basics/` - 框架基础**
  - [ ] LangChain 基础组件测试 (PromptTemplate, OutputParsers)
  - [ ] 构建基本 Chain 与 LCEL (LangChain Expression Language) 语法
- [ ] **`02_document_loaders/` - 数据清洗与切分**
  - [ ] 解析 PDF、Word、HTML 等异构文档
  - [ ] 测试不同的 Text Splitter 策略
- [ ] **`03_vector_databases/` - 向量数据库**
  - [ ] Faiss 本地索引存储与相似度检索
  - [ ] Milvus / Chroma 数据库连接与混合检索测试
- [ ] **`04_advanced_rag/` - 高阶 RAG 优化**
  - [ ] 实现基于 BERT 分类器的 Query 路由策略
  - [ ] 接入 BGE-Reranker 对检索结果进行重排序
  - [ ] 结合 Redis 实现记忆缓存功能

---

## 🏆 阶段实战项目：智能简历推荐系统 (SmartRecruit RAG)

**项目说明:**
构建一个面向 HR 的简历检索系统。系统不仅能通过向量检索匹配候选人，还能利用大模型对检索结果进行信息汇总与评价，支持多轮对话追问（如：“这些候选人中谁的 Python 经验最丰富？”）。