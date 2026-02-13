#  RAG Chatbot

This project implements a Retrieval-Augmented Generation (RAG) Chatbot
that answers questions using custom knowledge instead of relying only on LLM memory.

## 📌 Objective
To build an AI chatbot that retrieves relevant information from a dataset
and generates context-aware answers.

## 🛠️ Tech Stack
- Python
- LangChain
- FAISS (Vector Database)
- Sentence Transformers (Embeddings)
- Google Colab

## 🚀 How RAG Works
1. Documents are converted into embeddings.
2. Stored in FAISS vector database.
3. User asks a question.
4. System retrieves most relevant context.
5. LLM generates an answer using retrieved data.

## 📂 Use Case
This chatbot can be used for:
- Personal knowledge assistant
- Company document search
- Academic research help
- Offline Q&A system

## 🔎 Example Questions
- "What is Retrieval-Augmented Generation?"
- "Explain how FAISS works."
- "Summarize the dataset."

## ✅ Outcome
The chatbot produces more accurate and context-aware responses
by combining retrieval + generation.
