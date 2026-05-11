# 🎨 阶段七：多模态大模型与 AIGC

> **"A picture is worth a thousand words."** 
> AI 的能力不仅仅停留在文本。掌握图像识别（CV）、图像生成（Stable Diffusion）等多模态技术，能够极大拓宽 AI 应用的业务场景。

## 🎯 核心目标
1. 了解计算机视觉（CV）领域的基础知识与经典模型（CNN, ResNet, YOLO）。
2. 深刻理解 **AIGC 与 Diffusion（扩散）模型** 的核心原理。
3. 熟练部署与使用 **Stable Diffusion WebUI / ComfyUI**。
4. 掌握 SD 进阶玩法：ControlNet 姿态控制、LoRA 风格微调。

---

## 📚 优质学习资源推荐

### 📺 视频教程
* [Bilibili] [秋叶 - Stable Diffusion 保姆级入门教程](https://www.bilibili.com/video/BV1iM4y1y7oA) *(国内做 SD 最好懂的 UP 主，新手必看)*
* [YouTube] [Hugging Face - Diffusion Models Course](https://www.youtube.com/watch?v=sFztFnnclbg) *(深入原理)*

### 📖 文章与指南
* [Stable Diffusion Art - 免费且极佳的 SD 教程合集](https://stable-diffusion-art.com/)
* [Hugging Face Diffusers 文档](https://huggingface.co/docs/diffusers/index)

---

## 💻 练习与代码记录

- [ ] **`01_cv_basics/` - CV 基础**
  - [ ] OpenCV 基础图像处理测试
  - [ ] 调用预训练模型进行简单的图像分类测试
- [ ] **`02_stable_diffusion/` - SD 原理与实操**
  - [ ] 部署 SD WebUI 环境
  - [ ] 熟练掌握文生图（txt2img）与图生图（img2img）提示词写法
- [ ] **`03_advanced_sd/` - 进阶图像控制**
  - [ ] 安装并测试 ControlNet（如 Canny 边缘检测、OpenPose 姿态控制）
  - [ ] 训练一个简单的 SD LoRA（如人物脸型控制或特定画风）
- [ ] **`04_api_integration/` - 多模态集成**
  - [ ] 使用 Python API 调用本地 SD 服务生成图片
  - [ ] 测试支持视觉的大模型 (如 GPT-4V / Qwen-VL) 进行图像识别

---

## 🏆 阶段实战项目：风格化图像生成小程序

**项目说明:**
开发一个多模态应用小工具。用户输入自然语言描述，系统调用支持视觉的大语言模型优化提示词（Prompt 润色），然后传递给后端部署的 Stable Diffusion 模型（叠加特定画风的 LoRA），最终生成精美的图像并在前端展示。