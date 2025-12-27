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

## Use Cases
```
New hires learn company tech stack via chatbot.

Employees query company policies instead of searching multiple PDFs.

Customer asks a question, bot answers strictly from product documentations.(Customer Support)

Students upload textbooks and ask conceptual questions.

Lawyers query contracts without manually scanning documents.

Researcher uploads multiple papers and asks comparative questions.

```
---
## why not just use chat gpt?
```
“ChatGPT may hallucinate. RAG ensures answers come only from trusted documents.”
```

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


