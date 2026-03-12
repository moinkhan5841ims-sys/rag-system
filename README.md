# RAG Question-Answering System

A Retrieval-Augmented Generation (RAG) system built from scratch in Python.

## What it does
- Takes a question from the user
- Searches through a knowledge base to find the most relevant documents
- Uses an LLM (Llama 3.3 via Groq) to answer based only on those documents

## How it works
1. Documents are converted into vectors using Sentence Transformers
2. The question is also converted into a vector
3. Cosine similarity finds the most relevant documents
4. The LLM answers using only those documents as context

## Tech used
- Python
- Sentence Transformers (all-MiniLM-L6-v2)
- NumPy
- Groq API (Llama 3.3 70b)

## How to run
pip install sentence-transformers numpy groq
python rag.py
