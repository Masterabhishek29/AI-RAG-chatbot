# RAG Chatbot using LangChain, OpenAI, Gemini, and Hugging Face

## Overview

This project is a Retrieval-Augmented Generation (RAG) chatbot built using LangChain. It allows users to upload documents such as PDF, TXT, CSV, and DOCX files and ask questions about their content.

The chatbot retrieves relevant information from the uploaded documents and provides accurate answers using Large Language Models (LLMs) from OpenAI, Google Gemini, or Hugging Face.

## Features

* Upload PDF, TXT, CSV, and DOCX files
* Chat with your documents
* Supports OpenAI, Gemini, and Hugging Face models
* Uses ChromaDB as a vector database
* Retrieves relevant document chunks before generating answers
* Simple web interface built with Streamlit

## Tech Stack

* Python
* LangChain
* OpenAI API
* Google Gemini API
* Hugging Face
* ChromaDB
* Streamlit

## How It Works

1. Upload a document.
2. The document is split into smaller chunks.
3. Text embeddings are created for each chunk.
4. Embeddings are stored in ChromaDB.
5. When a user asks a question, the most relevant chunks are retrieved.
6. The retrieved context is sent to the LLM.
7. The chatbot generates an accurate response based on the document content.

## Installation

1. Create a virtual environment:

```bash
python -m venv langchain_env
```

2. Activate the environment:

```bash
.\langchain_env\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the application:

```bash
streamlit run RAG_app.py
```

## Usage

1. Select an LLM provider (OpenAI, Gemini, or Hugging Face).
2. Enter the required API key.
3. Upload your documents.
4. Create or load a ChromaDB vector store.
5. Start asking questions about your documents.

## Project Goal

The goal of this project is to improve the accuracy of LLM responses by combining document retrieval with text generation. This helps reduce hallucinations and allows the chatbot to answer questions using user-provided data.





