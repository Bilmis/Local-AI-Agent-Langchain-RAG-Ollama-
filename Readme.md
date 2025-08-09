# LocalAIAgentWithRAG

This project demonstrates how to build a **local AI-powered agent** capable of retrieving and reasoning over custom data using **LangChain**, **RAG (Retrieval-Augmented Generation)**, and **Ollama** as the local LLM backend.

## 🚀 Features
- **Local-first**: No dependency on external APIs for inference.
- **RAG Pipeline**: Retrieve relevant context from documents before generating responses.
- **LangChain Integration**: Orchestrates prompts, retrieval, and LLM responses.
- **Customizable Data Source**: Easily plug in your own documents.
- **Modular Design**: Easy to extend with more tools and agents.

## 🛠️ Tech Stack
- **[LangChain](https://www.langchain.com/)** – for prompt orchestration & chaining.
- **[Ollama](https://ollama.ai/)** – run LLMs locally.
- **[Python](https://www.python.org/)** – backend scripting and orchestration.
- **Vector Database** (e.g., FAISS, Chroma) – for storing document embeddings.

## ⚡ Getting Started

### 1️⃣ Prerequisites
- Install **Python 3.9+**
- Install [Ollama](https://ollama.ai/download) locally
- Install project dependencies: pip install -r requirements.txt

### 2️⃣ Pull a Model with Ollama (example: mistral model)
ollama pull mistral 

### 3️⃣ Run the Agent
python main.py

## How it Works

1. Document Ingestion – Load your local files.
2. Embedding & Storage – Convert text to embeddings and store in a vector DB.
3. Query Processing – On a user query, retrieve the most relevant chunks.
4. LLM Response – Pass the retrieved chunks + query to the LLM via LangChain.

## Future Improvements
Web-based UI
More LLM options
Multi-document & multi-modal support
Agent tools for executing code or web search