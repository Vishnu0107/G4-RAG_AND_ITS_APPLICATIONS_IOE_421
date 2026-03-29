# Agentic RAG with Adaptive Chunking

## Overview
This project improves Retrieval-Augmented Generation (RAG) for long documents by combining adaptive chunking, efficient retrieval, and agent-based orchestration for more accurate and grounded responses.

---

## Key Features
- Adaptive, tokenizer-aware chunking (preserves semantic structure)
- MiniLM embeddings + FAISS vector search
- Cosine similarity reranking for better retrieval
- Agentic RAG using Pydantic AI (tool-based workflow)
- Evaluation using ROUGE and BERTScore

---

## Architecture
1. Document Chunking (Adaptive)
2. Embedding Generation (MiniLM)
3. FAISS Vector Indexing
4. Query Encoding + Retrieval
5. Cosine Similarity Reranking
6. Agentic RAG (Pydantic AI)
7. Response Generation (LLMs)

---

## Models Used
- LLaMA-3 (1B, 3B, 8B)
- DeepSeek-R1
- Qwen2.5-7B
- Phi-3.5-mini
- Flan-T5

---

## Dataset
- :contentReference[oaicite:0]{index=0}  
  https://huggingface.co/datasets/abisee/cnn_dailymail

---

## Results
- Best Model: **Meta-LLaMA-3-8B**
- Metrics: ROUGE-1, ROUGE-2, ROUGE-L, BERTScore

---

## Future Work
- Better embedding models (Instructor, GTE)
- Multi-agent orchestration (CrewAI)
- Advanced reranking (cross-encoders)
- Multi-hop retrieval

---

## Tech Stack
- Python
- PyTorch
- Transformers (HuggingFace)
- FAISS
- Pydantic AI

---

## Benchmarks

<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/cff73c67-d40f-4b75-ae83-3075567d49c7" />

Benchmarks conducted using 200 test samples

## References
- Lewis et al., *Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks*, 2020  
  https://arxiv.org/abs/2005.11401  

- Vaswani et al., *Attention Is All You Need*, 2017  

- FAISS: A Library for Efficient Similarity Search  
  https://engineering.fb.com/2017/03/29/data-infrastructure/faiss-a-library-for-efficient-similarity-search/  

- Adaptive Chunking for RAG  
  https://arxiv.org/pdf/2603.25333  

- Agentic RAG (A-RAG)  
  https://arxiv.org/pdf/2602.03442  

- CrewAI (Multi-Agent Framework)  
  https://www.crewai.com/  

- OpenClaw (Agent Framework)  
  https://openclaw.ai/  

- Pydantic AI Agents  
  https://ai.pydantic.dev/agent/  

- :contentReference[oaicite:0]{index=0}  
  https://huggingface.co/datasets/abisee/cnn_dailymail  
