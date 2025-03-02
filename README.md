# MyRAG
<code>I am lovin' it, fun!</code>

## Key notes on RAG to Building one. 
*Down here I'm gonna have some of my notes before I actually cook :)*

## Core Concept
RAG combines two main approaches:
- **Retrieval-based methods**: Fetching relevant documents using vector search.
  - *Think of this like a librarian finding the right books for your question.*
- **Generation-based methods**: Using a Large Language Model (LLM) like GPT-4 or Llama to generate responses based on the retrieved data.
  - *Once the librarian finds the books, the LLM reads them and writes a summary or answer for you.*

---

## Key Components

### 🔍 Retrieval System (Fetching the Right Data)
- **Embedding Models**: 
  - Examples: `text-embedding-ada-002` (OpenAI) or Sentence-BERT.
  - Purpose: Convert text into numerical vectors for similarity search.
    - *Imagine turning sentences into unique "fingerprints" that a computer can compare to find similar ones.*
  
- **Vector Database**: 
  - Examples: FAISS, Pinecone, or ChromaDB.
  - Purpose: Store and perform similarity searches on embeddings.
    - *This is like a library that stores all the "fingerprints" and helps find the closest matches to your query.*
  
- **Chunking Strategy**: 
  - Fixed-length or semantic chunking to maintain context.
    - *Breaking down a big book into smaller chapters or sections so the system can focus on the most relevant parts.*

---
