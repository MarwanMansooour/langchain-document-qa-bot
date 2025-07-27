# LangChain Document QA Bot (RAG with Groq + ChromaDB)

This is a document-based Question Answering (QA) assistant built using Retrieval-Augmented Generation (RAG). Upload a `.pdf` or `.txt` file, ask any question about its content, and get accurate, context-aware answers from an LLM.

The project is implemented in a Jupyter Notebook: [`doc_qa_bot.ipynb`](./doc_qa_bot.ipynb)

---

## Features

- Upload `.pdf` or `.txt` files
- Automatic text extraction, chunking, and embedding
- Contextual Q&A powered by Groq-hosted LLaMA3
- Natural-language question interface
- Validates file types with error handling
- Option to upload and reprocess new documents anytime

---

## Technologies Used

- LangChain – chains, prompts, retrievers
- Groq – ultra-fast LLaMA3 inference
- LLaMA3-70B – for generating answers
- ChromaDB – in-memory vector database
- sentence-transformers – MiniLM embedding model
- PyPDF – for PDF parsing

---

## How It Works

1. Upload a `.pdf` or `.txt` document
2. The text is split into overlapping chunks
3. Each chunk is embedded with `all-MiniLM-L6-v2`
4. ChromaDB stores the vectorized chunks
5. You enter a question → the top relevant chunks are retrieved
6. LLaMA3 (via Groq) answers the question based on context

---

## Installation and Launch

Install the required dependencies:

```bash
pip install -r requirements.txt
```
Then Run the app
```bash
jupyter notebook doc_qa_bot.ipynb
```
File Structure 
langchain-document-qa-bot/
├── doc_qa_bot.ipynb       # Main Jupyter Notebook
├── requirements.txt       # Dependency list
└── README.md              # Project overview (this file)
