# Foundations of Large Language Models (LLMs): Guided Learning Prompts

## 🧭 Phase 1 — Foundations of Large Language Models (LLMs)

1. How does an LLM work in terms of FLOPs?
2. What does the *N² pairwise relationship* operation mean inside an LLM?
3. What is actually happening in self-attention when tokens compare to one another?
4. Why does attention scale quadratically (N²) instead of N choose 2?
5. What are **Q**, **K**, and **V** in the attention formula? Why are they called *Query*, *Key*, and *Value*?
6. What does the **T** in \( QK^{T} \) mean?
7. What is the **hidden dimension (d)** in LLMs?
8. Are **Q** and **K** the same vector for a token?
9. What does the **softmax** in the attention equation do?
10. In a Transformer, are all the "many layers" inference layers, or do they exist during training too?
11. Why do models have vocabularies of only ~50 000 tokens when languages have so many words?
12. What is an **attention head**, and how is it different from a mixture of experts (MoE)?
13. If subwords can mean different things in context, how can each have a single vector in the vocabulary?

## 🧩 Phase 2 — Embeddings, Context, and Retrieval

1. When two dense vectors represent two tokens, how does the model represent a whole phrase using them?
2. Should we worry about how token vectors are mixed to create a sentence vector when storing embeddings in a vector DB?
3. What does the *hidden dimension* mean when using a vector database for RAG? How do we control it?
4. What is a **dense vector**, and what does "dense" actually mean?
5. How does retrieval-augmented generation (RAG) relate to model reasoning? Why might a pure vector-DB RAG perform worse than a long-context model?
6. In RAG, are we relying on the *default meaning* of embeddings? Does that limit performance?

## ⚙️ Phase 3 — Model Architecture & Training Mechanics

1. What are **model kernels**, and what does **quantizing** mean?
2. Are the *weights* mentioned in quantization the same as the *weights* used in attention (Q, K, V matrices)?
3. When companies open-source a model but not the weights, how do they separate the two?
4. What is a **neural network** in simple terms, and how do layers of neurons form deep models?
5. In LLM inference, is the **prefill** stage the same as the attention computation and **decoding** the same as generation?
6. In multi-turn or agent-based use cases, is reusing the KV cache across calls what's meant by **prompt caching**?

## 🧠 Phase 4 — Context Engineering & Agent Orchestration

1. What are the techniques we can control to optimize LLM calls and agent orchestration — what's widely adopted across companies like Manus?
2. What is meant by **LangChain/LangGraph orchestration-level caching**?
3. How does **LangChain's LLM output cache** work, and does it require the LLM call to be pure and deterministic?
4. If an LLM call that triggers a tool call is cached, how can the tool still execute and use its own cache?
5. Can you create an architecture diagram for an **Agent Core** system with the recommended context-engineering layers (Input, Execution, Memory)?

## 🧮 Phase 5 — Learning the Math Behind It All

1. What is **gradient descent**, and how does it fit with attention, feed-forward layers, and training?
2. What is **entropy** — intuitively, mathematically, and in the context of LLMs?
3. What is **model collapse**, and why does it happen when models train on their own outputs?
