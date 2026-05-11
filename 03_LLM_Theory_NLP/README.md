# 🧠 阶段三：大模型核心理论与 NLP 基础

> **"What I cannot create, I do not understand." - Richard Feynman**
> 拒绝做“调包侠”。本阶段我们将深入引擎内部，搞懂神经网络、词向量以及奠定当前 AI 时代的 Transformer 架构。

## 🎯 核心目标
1. 掌握深度学习基础概念，熟练使用 **PyTorch** 搭建简单的神经网络。
2. 搞懂 NLP 核心概念（Tokenization, Word Embedding）。
3. 深入理解 **Transformer** 架构的 Encoder、Decoder 及 Self-Attention（自注意力机制）。
4. 熟悉 **HuggingFace** 生态，能自由下载、加载和使用预训练模型。

---

## 📚 优质学习资源推荐

### 📺 视频教程
* [Bilibili] [3Blue1Brown - 深度学习之神经网络的结构](https://www.bilibili.com/video/BV1bx411M7Zx) *(无痛理解神经网络数学原理的唯一神作)*
* [YouTube] [Andrej Karpathy - Let's build GPT: from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY) *(前 OpenAI 首席科学家手把手教你从零写 GPT，极其硬核！)*
* [Bilibili] [PyTorch 深度学习快速入门教程（绝对通俗易懂）](https://www.bilibili.com/video/BV1hE411t7RN)

### 📖 必读论文与教程
* [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) *(图解 Transformer，全网最友好的入门文章)*
* [Hugging Face NLP Course](https://huggingface.co/learn/nlp-course/zh-CN/chapter1/1) *(官方出品的 NLP 免费互动课程)*
* [Paper] *Attention Is All You Need* *(经典起源论文，选读)*

---

## 💻 练习与代码记录

- [ ] **`01_pytorch_basics/` - PyTorch 框架**
  - [ ] Tensor 张量的基本运算
  - [ ] 构建简单的全连接层 (Linear) 预测房价
- [ ] **`02_nlp_fundamentals/` - NLP 基础**
  - [ ] 使用 `jieba` / `tiktoken` 进行分词实操
  - [ ] 训练 FastText 或 Word2Vec 词向量
- [ ] **`03_transformer_impl/` - 架构剖析**
  - [ ] 手写简易的 Self-Attention 机制机制 (Numpy 或 PyTorch)
  - [ ] BERT 模型调用测试
- [ ] **`04_huggingface_hub/` - HuggingFace 实战**
  - [ ] `transformers` 库的 `pipeline` 快速上手
  - [ ] 离线下载并在本地加载预训练模型

---

## 🏆 阶段实战项目：海量文本分类系统

**项目说明:**
使用深度学习方法（基于 PyTorch + BERT 或 FastText），对海量新闻文本或用户评论进行情感分析与多分类。
体会深度学习模型训练（Training）、验证（Validation）与评估（F1-score, Recall）的完整流程。