# MyRAG
<code>I am lovin' it, fun!</code>

## Key notes on RAG to Building one. 
*Down here I'm gonna have some of my notes before I actually cook :)*

<code>
a. Retrieval System (First Step: Getting the Right Data)
Embedding Models: I’d use OpenAI’s text-embedding-ada-002 or Sentence-BERT.
Vector Database: FAISS or Pinecone for efficient similarity search.
Chunking Strategy: Fixed-length chunks with some overlap to maintain context. 
b. Reranking & Query Optimization (Refining Search)
Hybrid Search: BM25 (keyword-based) + vector search for improved recall.
Reranking: Cohere Rerank or Cross-Encoder models to prioritize relevant results.
c. Context Injection & Generation (Making the LLM Smarter)
Prompt Engineering: Insert retrieved text efficiently to stay within token limits.
Fine-Tuning (Optional): If retrieval isn’t enough, fine-tune a smaller LLM.
</code>
