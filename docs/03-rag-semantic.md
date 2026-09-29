# 第 3 层：RAG 与数据语义【必须】

> 学习目标：掌握 RAG 架构、向量数据库、数据语义的完整体系

---

## 学习要点

### RAG 基础与文档处理

- [ ] RAG 的核心概念与应用场景
- [ ] 文档加载与解析（PDF、Word、HTML 等）
- [ ] 文本分块（Chunking）的策略与技巧
- [ ] Embedding 与向量化

### 向量检索与重排

- [ ] 向量相似度搜索（Semantic Search）
- [ ] 检索质量评估与优化
- [ ] 重排（Reranking）机制
- [ ] 多步检索策略

### 向量数据库

- [ ] Milvus、Pinecone、Weaviate 等主流方案
- [ ] 索引管理与更新
- [ ] 向量数据库的选型

### 语义层与数据治理

- [ ] 指标、维度、实体的定义
- [ ] 数据血缘与溯源
- [ ] 受控 Metric API 的设计
- [ ] 避免 Agent 任意写 SQL 的设计原则

### 引用与来源追踪

- [ ] RAG 的可解释性与引用
- [ ] 来源追踪与验证
- [ ] 检索评测方法

---

## 推荐学习资源

| 资源 | 链接 | 说明 |
|------|------|------|
| **吴恩达 - LangChain 应用** | [视频](https://www.bilibili.com/video/BV1Ku4y1T7qz) | RAG 应用开发入门 |
| **RAG 高级技巧详解** | [视频](https://www.bilibili.com/video/BV15c411F7Z1) | RAG 优化和进阶 |
| **LangChain 官方文档** | [文档](https://python.langchain.com/docs/get_started/introduction) | 官方参考 |
| **Milvus 中文文档** | [文档](https://milvus.io/docs/zh-CN) | 开源向量数据库 |
| **BGE M3 Embedding** | [模型](https://huggingface.co/BAAI/bge-m3) | 最佳开源多语言 Embedding |

---

## 学习建议

1. **从简单开始**：不要一开始就设计复杂的语义层，先实现基础 RAG
2. **重视检索质量**：好的检索是 RAG 的关键，花时间优化
3. **设计受控接口**：如果 Agent 要访问数据，设计安全的、受控的 Metric API 而不是让它写 SQL

---

更详细的资源列表见：[reference/learning-resources.md](../reference/learning-resources.md)

---

**返回**：[知识体系总览](./README.md)
