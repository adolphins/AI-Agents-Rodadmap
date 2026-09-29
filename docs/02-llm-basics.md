# 第 2 层：LLM 应用基础【必须】

> 学习目标：理解 Transformer 原理、掌握 Prompt Engineering、学会使用 LLM API

---

## 学习要点

### Transformer 与深度学习理论

- [ ] Transformer 架构的核心概念（Self-Attention、Multi-Head Attention）
- [ ] Token 与分词（Tokenization）
- [ ] Embedding 的原理与应用
- [ ] Positional Encoding 与位置编码

### Prompt Engineering

- [ ] Prompt 设计的最佳实践
- [ ] Few-shot Learning 与 Chain-of-Thought
- [ ] Prompt 工程与优化技巧

### LLM API 与集成

- [ ] OpenAI / Claude / 其他 LLM 的 API 使用
- [ ] 流式输出（Streaming）处理
- [ ] 成本与延迟的考虑
- [ ] 错误处理与重试机制

### Structured Output

- [ ] JSON Schema 定义
- [ ] Pydantic 模型与验证
- [ ] 结构化输出的校验

---

## 推荐学习资源

| 资源 | 链接 | 说明 |
|------|------|------|
| **Andrej Karpathy - Build GPT** | [视频](https://www.youtube.com/watch?v=kCc8FmEb1nY) | 从零构建 GPT，深入理解原理 |
| **The Illustrated Transformer** | [文章](https://jalammar.github.io/illustrated-transformer/) | 图解 Transformer，直观易懂 |
| **吴恩达 - Prompt Engineering** | [视频](https://www.bilibili.com/video/BV1Mo4y1p7iH) | 简短精炼的 Prompt 工程课 |
| **Hugging Face NLP Course** | [课程](https://huggingface.co/learn/nlp-course/zh-CN/chapter1/1) | 免费官方 NLP 教程 |
| **Prompt Engineering Guide** | [文档](https://www.promptingguide.ai/zh) | 完整的技巧指南 |

---

## 学习建议

1. **理论与实践结合**：理解 Transformer 的原理是基础，但要通过 API 调用实践
2. **大量 Prompt 实验**：Prompt Engineering 是一门"手艺"，需要反复尝试
3. **关注成本**：学会使用较小的模型，理解 Token 计数

---

更详细的资源列表见：[reference/learning-resources.md](../reference/learning-resources.md)

---

**返回**：[知识体系总览](./README.md)
