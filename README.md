{\rtf1\ansi\ansicpg1252\cocoartf2822
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # \uc0\u55357 \u56516  LangChain Document QA Bot (RAG with Groq + ChromaDB)\
\
This is a document-based Question Answering (QA) assistant built using Retrieval-Augmented Generation (RAG). Users upload `.pdf` or `.txt` files and ask questions. The bot retrieves relevant content using ChromaDB and responds with context-aware answers from LLaMA3 hosted on Groq.\
\
## \uc0\u55357 \u56960  Features\
\
- \uc0\u9989  Upload and process `.pdf` or `.txt` files\
- \uc0\u55357 \u56589  Document chunking & semantic embeddings\
- \uc0\u55358 \u56800  Contextual Q&A using Groq-hosted LLaMA3\
- \uc0\u10060  Error handling for unsupported file types\
- \uc0\u55357 \u56577  Upload and reprocess new documents at runtime\
\
## \uc0\u55358 \u56800  Technologies Used\
\
- LangChain\
- Groq (LLaMA3-70B)\
- Chroma Vector DB\
- SentenceTransformers (MiniLM)\
- PyPDF\
\
## \uc0\u55357 \u56741 \u65039  How It Works\
\
1. Upload a `.pdf` or `.txt` file\
2. Text is split into chunks\
3. Embeddings are generated and stored in Chroma\
4. Ask any question about the document\
5. Bot retrieves matching chunks and responds using LLM\
\
## \uc0\u55357 \u56550  Installation\
\
```bash\
pip install -r requirements.txt\
python doc_qa_bot.py}