ML RAG Assistant:

A production-focused Retrieval-Augmented Generation system built over technical ML blogs (D2L, Karpathy, Ruder, Colah). Demonstrates practical RAG engineering: retrieval, evaluation, hallucination control, and API deployment.

Overview

What it does: Semantic search + grounded answer generation over curated ML content

Scrapes and chunks technical blog content with token-aware splitting

FAISS similarity search with all-MiniLM-L6-v2 embeddings

Grounded generation using TinyLlama (1.1B, CPU-friendly)

Quantitative evaluation: Recall@5 ≈ 0.75, MRR@5 ≈ 0.62

Hallucination mitigation via similarity thresholding

FastAPI + Gradio interface


Evaluation

Recall@5: 0.75 | MRR@5: 0.62

Tested on chunk-level labeled queries. 75% of relevant chunks retrieved in top-5; relevant chunks typically rank ~2nd.



Content sources: D2L · Karpathy · Ruder · Colah
