<div align="center">

# probable-adventure
## Switch Careers to AI Agent Development · Learning Path

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

> A curated, hands-on learning path from zero to building production-grade AI Agents.  
> Focus on **RAG** and **Agent Systems** — the two most in-demand skills for AI application engineers.

</div>

---

## The Roadmap

### Phase 1: Python & Backend Foundations
**Goal:** Master Python advanced features and build RESTful APIs with FastAPI. Learn to wrap AI models in a web UI using Streamlit.

- **Course:** [黑马程序员 - Python 全套教程](https://www.bilibili.com/video/BV1qW4y1a7fU) | [FastAPI Full Course](https://www.youtube.com/watch?v=0sOvCWFmrtA)
- **Book:** *Fluent Python* (2nd Edition) — focus on decorators, generators, and concurrency
- **Project:** `Basic Chatbot` — A multi-turn chat web app using Python + Streamlit + any LLM API

---

### Phase 2: Prompt Engineering & Low-Code Agents
**Goal:** Learn to "command" AI with natural language. Rapidly prototype business logic using low-code platforms.

- **Course:** [吴恩达 - ChatGPT Prompt Engineering](https://www.bilibili.com/video/BV1Mo4y1p7iH) | [Dify Official Tutorials](https://www.youtube.com/@DifyAI)
- **Docs:** [Prompt Engineering Guide](https://www.promptingguide.ai/zh) | [Dify Docs](https://docs.dify.ai/v/zh-hans)
- **Project:** `Interview Agent` — A resume-aware mock interviewer built on Coze or Dify

---

### Phase 3: LLM Theory & NLP Fundamentals
**Goal:** Understand how Transformers work under the hood. Stop being a "black-box user."

- **Course:** [Andrej Karpathy - Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY) | [3Blue1Brown - Neural Networks](https://www.bilibili.com/video/BV1bx411M7Zx)
- **Article:** [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) | [Hugging Face NLP Course](https://huggingface.co/learn/nlp-course/zh-CN/chapter1/1)
- **Project:** `Text Classifier` — News classification using BERT / FastText with PyTorch

---

### Phase 4: Advanced RAG Systems (Core)
**Goal:** Eliminate hallucinations by connecting LLMs to private data. Master document parsing, embedding, and retrieval optimization.

- **Course:** [吴恩达 - LangChain for LLM Application Development](https://www.bilibili.com/video/BV1Ku4y1T7qz) | [RAG Advanced Techniques](https://www.bilibili.com/video/BV15c411F7Z1)
- **Docs:** [LangChain Python Docs](https://python.langchain.com/docs/get_started/introduction) | [Milvus Docs](https://milvus.io/docs/zh-CN)
- **Project:** `HR Resume RAG` — Intelligent resume search with multi-turn conversational filtering

---

### Phase 5: Agent Systems & Multi-Agent Orchestration (Core)
**Goal:** Give AI "hands and eyes." Build agents that can plan, use tools, and collaborate.

- **Course:** [DeepLearning.AI - AI Agents in LangGraph](https://learn.deeplearning.ai/courses/ai-agents-in-langgraph) | [AutoGen vs CrewAI vs LangGraph](https://www.bilibili.com/video/BV1Jw411h7Z5)
- **Docs:** [LangGraph Docs](https://langchain-ai.github.io/langgraph/) | [OpenAI Function Calling](https://platform.openai.com/docs/guides/function-calling)
- **Project:** `Smart Voyage Agent` — Multi-intent travel assistant (weather + ticketing agents coordinated via LangGraph)

---

### Phase 6: Fine-Tuning & Private Deployment
**Goal:** Build domain-specific models and deploy them in production environments.

- **Course:** [LLaMA-Factory 官方教学](https://www.bilibili.com/video/BV1hK421d74W) | [LoRA & QLoRA Explained](https://www.youtube.com/watch?v=1YmO4f5E34s)
- **Docs:** [LLaMA-Factory GitHub](https://github.com/hiyouga/LLaMA-Factory) | [vLLM Docs](https://docs.vllm.ai/en/latest/)
- **Project:** `Domain NER Model` — Fine-tune Qwen-7B with LoRA for entity/relation extraction

---

### Phase 7: Multimodal & AIGC (Optional)
**Goal:** Expand beyond text into images and vision. Broaden your AI application boundary.

- **Course:** [秋叶 - Stable Diffusion 保姆级入门](https://www.bilibili.com/video/BV1iM4y1y7oA) | [Hugging Face Diffusion Models](https://www.youtube.com/watch?v=sFztFnnclbg)
- **Docs:** [Stable Diffusion Art Tutorials](https://stable-diffusion-art.com/) | [Diffusers Docs](https://huggingface.co/docs/diffusers/index)
- **Project:** `Style Image Generator` — A tool that uses LLM prompt refinement + SD + LoRA for styled image generation

---

## Suggested Learning Order

```
Phase 1 → Phase 2 → Phase 4 → Phase 5  (Get job-ready first)
         ↘ Phase 3 ↗ Phase 6           (Deepen theory later)
                  ↘ Phase 7             (Optional expansion)
```

**Don't start with math and theory.** Build working RAG and Agent projects first, then come back to Phase 3 and 6 to understand why they work.

## Practical Tips

1. **You don't need to buy GPUs.** Rent on [AutoDL](https://www.autodl.com/) or [阿里云 PAI](https://www.aliyun.com/product/bigdata/pai) for ~¥50/day.
2. **Your GitHub is your resume.** Don't just copy the sample projects — change the domain (e.g., medical → legal, travel → IT ops) to make them unique.
3. **Key interview topics:** How do you improve RAG recall? (Answer: Rerank, hybrid search, query rewriting.)

---

<div align="center">

**Keep building. Good luck on your probable adventure!**

</div>
