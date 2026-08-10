<img width="1692" height="930" alt="Built a Retrieval-Augmented Generation" src="https://github.com/user-attachments/assets/e23f3ea8-f6c7-4487-8a3e-2b56b2a2ca65" /># Retrieval-Augmented-Generation-RAG-
End-to-end Retrieval-Augmented Generation (RAG) question-answering system using LangChain, Google Gemini, Gemini Embeddings, and ChromaDB.

An end-to-end Retrieval-Augmented Generation (RAG) question-answering system built using AWS documentation as the knowledge source.
# Overview

This project demonstrates how a Retrieval-Augmented Generation (RAG) pipeline can retrieve relevant information from an external knowledge source and provide context-grounded answers using Google Gemini.

The system loads an AWS documentation webpage, splits the content into smaller chunks, converts the chunks into vector embeddings, stores them in ChromaDB, retrieves the most relevant information for a user query, and passes the retrieved context to Google Gemini to generate the final answer.

## 🏗️ Architecture

![RAG Architecture](architecture/rag-architecture.png)

## 🔄 How It Works

```text
AWS Webpage
     ↓
Document Loading
     ↓
Text Splitting
     ↓
Gemini Embeddings
     ↓
ChromaDB
     ↓
Retriever
     ↓
Relevant Context
     ↓
Google Gemini
     ↓
Final Answer
