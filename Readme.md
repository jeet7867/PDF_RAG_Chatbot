# PDF RAG Chatbot

A Retrieval-Augmented Generation (RAG) system that allows users to upload **PDF documents**
and ask questions based strictly on their content using **Google Gemini** and **Pinecone**.

---

## Features
- Upload and process PDF documents
- Semantic search using vector embeddings
- Context-aware answers (no hallucinations)
- Single-document support(free pincone index used)
- Secure API key handling

---

## Tech Stack
- Node.js
- Google Gemini API
- LangChain
- Pinecone Vector Database
- PDF parsing tools

---

## Project Structure
```
├── ingest.js # PDF ingestion & embedding
├── query.js # Question answering
├── pdfs/ # Uploaded documents
├── .env.example
├── .gitignore
├── package.json
└── README.md
```


---

## Setup Instructions

### 1️⃣ Clone Repository
```bash
git clone https://github.com/<your-username>/pdf-rag-chatbot.git
cd pdf-rag-chatbot
```

### 2️⃣ Install Dependencies
npm install

### 3️⃣ Environment Variables

Create .env file:
```
GEMINI_API_KEY=
PINECONE_API_KEY=
PINECONE_INDEX_NAME=
```

## Run the Project
### Ingest PDFs
node ingest.js

### Ask Questions
node query.js


## Use Cases
```
Study notes Q&A

Research paper analysis

Interview preparation

Company document search
```