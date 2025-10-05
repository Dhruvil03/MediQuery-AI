# MediQuery-AI: Conversational Medical Assistant Using LLMs

**MediQuery-AI** is an intelligent conversational agent built to answer medical questions by combining the power of **Large Language Models (LLMs)**, **vector-based document retrieval**, **Retrieval-Augmented Generation (RAG)** and **session-aware memory**. Users can interact through a responsive frontend powered by HTML, CSS, JavaScript, and Flask, making complex medical information accessible through a natural chat interface.

## 📌 Project Objective

MediQuery-AI aims to assist users—patients, medical professionals, or curious learners—in retrieving reliable, context-aware answers to health-related queries by drawing upon a curated set of medical literature and employing modern natural language understanding techniques.

## 🔁 System Flow

1. **User Input**: User submits a medical query
2. **Memory Module**: Maintains conversational context (chat history + current query)
3. **Vector Database**: Stores embedded medical documents for retrieval
4. **Document Retrieval**: Top-K relevant documents retrieved using vector similarity search
5. **LLM Processing**: LLM synthesizes an answer based on retrieved documents and current query
6. **Output**: Response returned to user via Flask-based frontend

## ⚙️ Tech Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python, Flask
- **Embedding & Retrieval**:
  - `sentence-transformers` for semantic vector generation
  - FAISS for efficient vector search
- **LLM Integration**: OpenAI GPT API
- **Session Memory**: Chat history for enhanced context retention

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- OpenAI API key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/MediQuery-AI.git
   cd MediQuery-AI
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   ```bash
   export OPENAI_API_KEY="your_openai_api_key_here"
   ```

4. **Run the application**
   ```bash
   python app.py
   ```

5. **Access the web interface**
   Open your browser and navigate to `http://localhost:5000`

## 💡 Key Features

- ✅ **Memory-aware QA**: Handles follow-ups and ongoing context using session history
- 📄 **Medical Document Parsing**: Upload domain-specific PDFs
- 🔍 **Semantic Search**: Matches queries to documents using dense vector representations
- 🤖 **LLM Answer Generation**: Uses top-k retrieved chunks to generate precise responses
- 🌐 **Web Interface**: Built with Flask for user interaction via browser

![MediQuery](https://github.com/user-attachments/assets/49d62728-f83d-4445-9b01-4cfe9df57920)

---
