# MyRAG
<code>I am lovin' it, fun!</code>

## Key notes on RAG to Building one. 

Model - Gemini
### To run
create a venv

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

### ⚡ Reranking & Query Optimization (Refining Search Results)
- **Hybrid Search**: 
  - Combines BM25 (keyword search) with vector retrieval.
    - *Using both keyword matching (like searching for specific words) and semantic matching (understanding the meaning) to get better results.*
  
- **Reranking**: 
  - Uses tools like Cohere Rerank or cross-encoder models.
    - *After finding potential matches, the system sorts them to put the most relevant ones at the top.*

---

### 💡 Context Injection & Generation (Making the LLM Smarter)
- **Prompt Engineering**: 
  - Injects retrieved text into the LLM prompt while managing token limits.
    - *Giving the LLM the most important pieces of information to work with, like giving a student the key notes for an exam.*
  
- **Fine-Tuning (Optional)**: 
  - Fine-tuning smaller LLMs if retrieval alone isn't sufficient.
    - *Teaching the LLM to be better at specific tasks, like training a chef to specialize in a certain cuisine.*

---

**Well this all is good info, I have lot more to add here, I feel let's start puting some technologies...**

## You need this
- Python 3.7+
- A Pinecone API key
- A GROQ API key (for LLama 3.1 access) {using the free one}
- A GitHub personal access token

## Environment Variables
Create a .env file in the root directory with the following variables:

<code>PINECONE_API_KEY=your_pinecone_api_key
GROQ_API_KEY=your_groq_api_key
GITHUB_TOKEN=your_github_token
</code>

