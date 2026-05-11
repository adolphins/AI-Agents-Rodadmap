# 🛠️ 阶段六：大模型微调与企业级私有部署

> **"Tailoring the brain."** 
> 面对垂直业务（如医疗、法律、特定代码风格），通用大模型的表现往往不如人意。掌握 PEFT 参数高效微调与企业级部署方案，是建立技术壁垒的关键。

## 🎯 核心目标
1. 掌握模型微调数据的准备与清洗格式（如 JSONL 格式 QA 对）。
2. 理解并实践 **LoRA** (Low-Rank Adaptation) 参数高效微调技术。
3. 熟练使用 **LLaMA-Factory** 等开箱即用的微调框架。
4. 掌握大模型量化（GPTQ）与高性能推理部署（**vLLM**）。

---

## 📚 优质学习资源推荐

### 📺 视频教程
* [Bilibili] [LLaMA-Factory 官方教学：从零微调大模型](https://www.bilibili.com/video/BV1hK421d74W) *(极大降低微调门槛的神兵利器)*
* [YouTube] [Fine-tuning LLMs with LoRA & QLoRA EXPLAINED](https://www.youtube.com/watch?v=1YmO4f5E34s) *(讲得最透彻的 LoRA 理论课)*

### 📖 文章与指南
* [LLaMA-Factory GitHub Repo](https://github.com/hiyouga/LLaMA-Factory)
* [vLLM 官方文档 (极致加速推理)](https://docs.vllm.ai/en/latest/)
* [Hugging Face PEFT 官方文档](https://huggingface.co/docs/peft/index)

---

## 💻 练习与代码记录

- [ ] **`01_dataset_prep/` - 数据准备**
  - [ ] 爬取或整理业务数据，编写脚本转化为大模型微调标准格式 (JSONL)
  - [ ] 数据的切分（Train/Eval 集）
- [ ] **`02_llama_factory_lora/` - LoRA 微调**
  - [ ] 使用 LLaMA-Factory WebUI 对 Qwen / DeepSeek 进行指令微调
  - [ ] 导出合并微调后的 LoRA 权重
- [ ] **`03_quantization/` - 模型量化**
  - [ ] 测试 INT8/INT4 量化对显存的节省比例及性能损耗
- [ ] **`04_vllm_deployment/` - 高性能部署**
  - [ ] 使用 Docker + vLLM 启动兼容 OpenAI API 格式的本地服务
  - [ ] （选修）编写 `docker-compose.yml` 管理多个服务

---

## 🏆 阶段实战项目：垂直领域信息抽取大模型

**项目说明:**
选取特定业务数据（如微博娱乐八卦数据、中医药文本数据），构建微调数据集。使用 LoRA 技术对开源大模型（如 Qwen-7B）进行微调，使其能够精准地从非结构化文本中提取特定的实体（Entity）和关系（Relation），并以结构化 JSON 返回。