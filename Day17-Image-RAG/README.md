# Day17 – Intelligent Image Search using RAG

This project implements a Retrieval-Augmented Generation (RAG) system
for semantic image search using a personal dataset.

## 📌 Features
- Personal dataset (17 images)
- CLIP model used for image + text embeddings
- FAISS vector database for similarity search
- Natural language query support
- Retrieves relevant images based on meaning (not filename)

## 🛠️ Tech Stack
- Python
- OpenAI CLIP
- FAISS
- Google Colab
- Matplotlib


## 🚀 How It Works
1. Images converted into embeddings using CLIP.
2. Embeddings stored in FAISS vector DB.
3. User enters text query.
4. System retrieves most semantically similar images.

## ✅ Example Queries
- "study table"
- "working on laptop"
- "books and notes"
- "personal workspace"

This demonstrates Multimodal RAG applied to intelligent visual search.
