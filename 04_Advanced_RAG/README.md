# Phase 4: Advanced RAG Systems

> Give AI a proper memory. Connect LLMs to private data and eliminate hallucinations.

## Goals

- Master **LangChain** core components (Models, Prompts, Memory, Chains).
- Implement document parsing, chunking strategies, and embedding.
- Use vector databases (**Milvus**, **Faiss**, **Chroma**) for semantic search.
- Apply advanced optimizations: query rewriting, reranking, hybrid retrieval (BM25 + dense).

## Resources

- **Video:** [吴恩达 - LangChain for LLM Application Development](https://www.bilibili.com/video/BV1Ku4y1T7qz) | [RAG Advanced Techniques](https://www.bilibili.com/video/BV15c411F7Z1)
- **Docs:** [LangChain Python Docs](https://python.langchain.com/docs/get_started/introduction) | [Milvus Docs](https://milvus.io/docs/zh-CN)
- **Model:** [BGE M3 Embedding](https://huggingface.co/BAAI/bge-m3) — best open-source multilingual embedding model

## Project: HR Resume RAG

Build an intelligent resume search system for recruiters.

Requirements:
- Parse heterogeneous resumes (PDF, Word) and chunk effectively
- Vector search + re-ranking for accurate candidate matching
- Multi-turn conversational filtering (e.g., "Who has the most Python experience?")
