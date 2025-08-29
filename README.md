# Conversational-PDF-Q & A-with-RAG-Chat-History
This project is a Streamlit-based conversational chatbot that allows users to upload multiple PDFs and interact with their content. It uses Retrieval-Augmented Generation (RAG) to retrieve relevant information from the uploaded documents and provide precise answers. The chatbot also maintains chat history of previous conversation.


# 📘 RAG Q&A Chatbot with PDF Upload & Chat History

A **Streamlit-based conversational chatbot** that lets you:
- Upload multiple PDFs 📄
- Ask questions about their content ❓
- Get AI-powered answers using **RAG (Retrieval-Augmented Generation)**
- Maintain **chat history** so follow-up questions make sense 🔄

---

## 🚀 Features
- Upload one or more PDFs.
- Splits PDF content into chunks and stores embeddings in **Chroma vector database**.
- Uses **HuggingFace embeddings (`all-MiniLM-L6-v2`)** for semantic search.
- Uses **Groq LLM (Gemma2-9b-It)** for answering questions.
- Maintains **session-based chat history** with memory.
- Built with **Streamlit** for an easy-to-use interface.

---

## 🏗️ Project Structure
project-folder/
│── app.py # Main Streamlit app
│── requirements.txt # Dependencies
│── .env # API keys (do not upload)
│── venv/ # Virtual environment (ignored)




---

## ⚙️ Installation & Setup

### 1️ Clone the repository
    ```bash
    git clone  https://github.com/SnehalSolawala/Conversational-PDF-Q-A-with-RAG-Chat-History.git
    cd Conversational-PDF-Q-A-with-RAG-Chat-History.git

### 2 Create Virtual Environment
    python -m venv venv
    source venv/bin/activate   # for Linux/Mac
    venv\Scripts\activate      # for Windows

### 3 Install dependencies
    pip install -r requirements.txt

### 4 Add environment variables
    Create a .env file in the root folder and add:
    LANGCHAIN_API_KEY=your_langchain_api_key
    HF_TOKEN=your_huggingface_token
### 5 Running the App
    streamlit run app.py



# Usage
  
  Enter your Groq API key in the input box.
  
  Upload one or more PDF files.
  
  Type a question related to the PDFs.
  
  Get concise answers with context-aware memory.

# Tech Stack

  Streamlit – UI
  
  LangChain – RAG pipeline & chat memory
  
  HuggingFace – Embeddings
  
  Chroma – Vector store
  
  Groq (Gemma2-9b-It) – LLM
