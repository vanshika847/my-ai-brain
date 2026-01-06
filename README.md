# my-ai-brain
# 🧠 Second Brain
![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red)
![ChromaDB](https://img.shields.io/badge/VectorDB-Chroma-purple)
![RAG](https://img.shields.io/badge/AI-RAG-success)
![License](https://img.shields.io/badge/License-MIT-green)

> **A production-grade personal AI knowledge base that lets you query your documents like an extension of your brain.**

Second Brain transforms PDFs, Word files, PowerPoint decks, Markdown, and text files into a **conversational, source-aware AI assistant** with confidence-scored answers.

---

## 🎥 Demo
> *(Add your demo GIF or video link here)*


---

## 🚀 Why Second Brain?

Students, developers, and professionals accumulate vast amounts of unstructured knowledge—but retrieving insights later is inefficient.

**Traditional search fails because it:**
- Is keyword-based
- Loses semantic context
- Cannot reason across documents

**Second Brain solves this** using Retrieval-Augmented Generation (RAG), vector search, and intelligent chunking to create a true personal knowledge system.

---

## ✨ Key Features

- 📄 Multi-format ingestion (PDF, DOCX, PPTX, MD, TXT)
- ✂️ Token-aware recursive chunking with overlap
- 🧠 Local, production-grade embeddings (BGE-large)
- 💾 Persistent vector storage with ChromaDB
- 🎯 Confidence-scored semantic retrieval
- 📚 Page-level source attribution
- 💬 Conversational memory for follow-ups
- 🌐 Streamlit UI + CLI interface
- 🔒 Privacy-first (runs locally)

---

## 🏗️ Architecture Overview

```text
Documents
   ↓
Ingestion Brain (Parser + Metadata)
   ↓
Chunking Brain (Token-aware Recursive Chunking)
   ↓
Memory Brain (Embeddings + ChromaDB)
   ↓
Reasoning Brain (Retriever + RAG Chain)
   ↓
LLM (OpenAI / Ollama)
   ↓
UI (Streamlit / CLI)

PROJECT STRUCTURE
second-brain/
├── app/
│   ├── ingestion/     # Parsing, preprocessing, chunking
│   ├── memory/        # Embeddings & vector store
│   ├── reasoning/     # Retrieval, LLM, RAG chain
│   ├── utils/
│   └── config.py
├── ui/
│   └── streamlit_app.py
├── main.py
├── requirements.txt
├── .env
└── chroma_db/

```
# Tech Stack
Core

Python 3.10+

LangChain

ChromaDB

Sentence Transformers (BAAI/bge-large-en-v1.5)

OpenAI / Ollama-compatible LLMs

Streamlit

Parsing

PyPDF

python-docx

python-pptx

Unstructured

Tokenization

tiktoken

# Setup & Installation
git clone https://github.com/your-username/second-brain.git
cd second-brain
pip install -r requirements.txt


Create .env:

OPENAI_API_KEY=your_openai_api_key

# ▶️ Usage
Ingest Documents
python main.py ingest --dir ./my_documents

CLI Mode
python main.py query

Streamlit UI
python main.py ui

streamlit run ui/streamlit_app.py

# 🧪 Example Query

“Explain virtual memory using my OS notes”

Response includes:

Context-grounded answer

Source document + page

Confidence score

If information is missing, the system explicitly says so.

# 🎯 Use Cases

Engineering students revising from multiple resources

Researchers navigating large paper collections

Developers building a personal AI knowledge system

Teams querying internal documentation

# 🔮 *Future Enhancements*

Cross-encoder reranking (higher precision)

Hybrid search (BM25 + vector)

Image & table understanding from PDFs

Query expansion using LLMs

Dockerized cloud deployment

Google Drive integration

# 🧠 *Design Philosophy*

Correctness over flash

Transparency over hallucination

Systems thinking over demos

If the system doesn’t know, it says so.


# 🙌 Acknowledgements

Inspired by modern Retrieval-Augmented Generation (RAG) systems and personal knowledge management research.

# FLOWCHART
[PROJECT FLOWCHART](https://diagram-refiner--vanshikashinde.replit.app/)


