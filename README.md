# 🧠 DocuMind: AI-Powered Document Assistant

**DocuMind** is a Retrieval-Augmented Generation (RAG) platform that allows users to "chat" with their documents. Users can upload PDFs (contracts, research papers, resumes), and the AI will analyze them to answer questions, summarize content, and extract key details.


## 🚀 The Vision

We are building a Full-Stack AI Application:
* **Backend:** FastAPI (High-performance Python API)
* **AI Engine:** LangChain + Vector Database (ChromaDB)
* **Frontend:** React / Streamlit (Planned for Phase 4)
* **Deployment:** Docker (Planned for Phase 5)

## ⚡ Features (Phase 1)

* **FastAPI Server:** A robust REST API skeleton.
* **PDF Ingestion:** Endpoint to upload and store PDF files securely.
* **Text Extraction:** Automated parsing of PDF binary data into machine-readable text using `pypdf`.
* **Automatic Docs:** Interactive API testing UI via Swagger (`/docs`).

## 🛠️ Tech Stack

* **Language:** Python 3.10+
* **Framework:** `FastAPI`
* **Server:** `Uvicorn` (ASGI)
* **Processing:** `pypdf` (PDF Parsing)

## ⚙️ Installation & Setup

### 1. Clone/Setup Project
```bash
# Create project folder
mkdir documind-backend
cd documind-backend

# Windows
python -m venv venv
.\venv\Scripts\activate

# Mac/Linux
python3 -m venv venv
source venv/bin/activate

pip install fastapi uvicorn python-multipart pypdf langchain chromadb sentence-transformers

uvicorn app.main:app --reload