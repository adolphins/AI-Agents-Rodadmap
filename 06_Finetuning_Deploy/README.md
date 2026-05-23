# Phase 6: Fine-Tuning & Private Deployment

> Tailor the brain. Build domain-specific models and deploy them at scale.

## Goals

- Prepare and clean fine-tuning datasets (JSONL QA pairs).
- Apply **LoRA / QLoRA** for parameter-efficient fine-tuning.
- Use **LLaMA-Factory** for streamlined training workflows.
- Deploy with quantization (GPTQ, AWQ) and high-performance inference (**vLLM**).

## Resources

- **Video:** [LLaMA-Factory 官方教学](https://www.bilibili.com/video/BV1hK421d74W) | [LoRA & QLoRA Explained](https://www.youtube.com/watch?v=1YmO4f5E34s)
- **Docs:** [LLaMA-Factory GitHub](https://github.com/hiyouga/LLaMA-Factory) | [vLLM Docs](https://docs.vllm.ai/en/latest/) | [Hugging Face PEFT Docs](https://huggingface.co/docs/peft/index)

## Project: Domain NER Model

Fine-tune an open-source model (e.g., Qwen-7B) for vertical-domain information extraction.

Requirements:
- Build a domain dataset (e.g., Traditional Chinese Medicine, legal documents)
- Fine-tune with LoRA using LLaMA-Factory
- Export merged weights and deploy via vLLM with OpenAI-compatible API
