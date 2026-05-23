# 💬 阶段二：Prompt 工程与低代码 Agent 开发

> **"Language is the new programming language."** 
> 本阶段旨在建立“AI指挥官”思维。在写大量代码之前，先学会如何用自然语言准确“控制”大模型，并通过低代码平台快速验证业务逻辑。

## 🎯 核心目标
1. 掌握进阶 Prompt 编写技巧，学会消除模型幻觉、规范输出格式。
2. 熟练使用 **Coze (扣子)** 编排工作流和插件。
3. 深入掌握 **Dify** 平台，理解企业级应用如何进行私有化构建与知识库管理。
4. 掌握 **Ollama** 的使用，能够在本地部署和运行开源大模型。

---

## 📚 优质学习资源推荐

### 📺 视频教程
* [Bilibili] [吴恩达 - 面向开发者的 ChatGPT 提示词工程 (中英字幕)](https://www.bilibili.com/video/BV1Mo4y1p7iH) *(绝对的经典必看)*
* [YouTube] [Dify Official Tutorials](https://www.youtube.com/@DifyAI) *(官方教程，了解最新特性)*
* [Bilibili] [Ollama + 任何大模型本地部署教程](https://www.bilibili.com/video/BV15m411E73g)

### 📖 文章与指南
* [Prompt Engineering Guide (DAIR.AI)](https://www.promptingguide.ai/zh) *(目前最全面、最权威的提示词工程开源指南)*
* [Dify 官方中文文档](https://docs.dify.ai/v/zh-hans) *(实战必备)*
* [Coze 官方文档](https://www.coze.cn/docs/guides/welcome)

---

## 💻 练习与代码记录

- [ ] **`01_prompt_engineering/` - 提示词技巧**
  - [ ] Zero-shot & Few-shot 样本提示练习
  - [ ] COT (思维链) 提升逻辑推理能力练习
  - [ ] 信息抽取与 JSON 格式化输出强制规范
- [ ] **`02_local_deployment/` - 本地模型部署**
  - [ ] 安装 Ollama 并运行 `DeepSeek-R1` 或 `Qwen`
  - [ ] 使用 Python `requests` 调用本地 Ollama 接口
- [ ] **`03_coze_dify_configs/` - 平台配置备份**
  - [ ] 导出 Coze 工作流配置 (JSON/YAML)
  - [ ] 导出 Dify 知识库与应用配置

---

## 🏆 阶段实战项目：技术面试助手 (Interview Agent)

**项目说明:**
无需写太多复杂的后端代码，完全基于 **Coze** 或 **Dif