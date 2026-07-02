# Mini RAG Chatbot

A lightweight Retrieval-Augmented Generation (RAG) chatbot built using **Python**, **Streamlit**, **LangChain**, **Google Gemini**, **Hugging Face Sentence Transformers**, and **FAISS**.

The application enables users to upload PDF documents, generate vector embeddings, perform semantic search, and receive context-aware responses using Google's Gemini Large Language Model.

---

## Features

- Upload PDF documents
- Extract text using PyPDF
- Split documents into semantic chunks
- Generate embeddings using Hugging Face Sentence Transformers
- Store embeddings using FAISS, ChromaDB
- Perform semantic similarity search
- Generate context-aware answers using Google Gemini
- Interactive Streamlit web interface

---

## Technology Stack

- Python
- Streamlit
- LangChain
- LangChain 
- Google Gemini API
- Hugging Face Sentence Transformers
- FAISS
- ChromaDB
- PyPDF

---

## Project Structure

```text
Mini_RAG_Chatbot/
│
├── app.py
├── requirements.txt
├── README.md
├── .env.example
├── .gitignore
│
├── data/
├── database/
│
├── utils/
│   ├── loader.py
│   ├── splitter.py
│   ├── embeddings.py
│   ├── vectorstore.py
│   └── rag_chain.py
│
├── test_loader.py
├── test_splitter.py
├── test_embedding.py
├── test_vectorstore.py
├── test_faiss.py
├── test_gemini.py
└── test_rag.py
```

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Sehajkaur24/Mini_RAG_Chatbot.git

cd Mini_RAG_Chatbot
```

---

### 2. Create a Virtual Environment

#### Windows

```bash
python -m venv rag_env
```

Activate the environment

```bash
rag_env\Scripts\activate
```

---

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4. Configure the Gemini API

Create a `.env` file in the project root.

```env
GOOGLE_API_KEY=YOUR_GEMINI_API_KEY
```

Generate your API key from:

https://aistudio.google.com/app/apikey

---

### 5. Add PDF Documents

Place the PDF files inside the `data` directory.

Example:

```text
data/
└── sample.pdf
```

---

### 6. Run the Application

```bash
streamlit run app.py
```

Open your browser and navigate to:

```
http://localhost:8501
```

---

## Workflow

1. Upload a PDF document.
2. Extract text from the document.
3. Split the text into manageable chunks.
4. Generate embeddings using Hugging Face Sentence Transformers.
5. Store embeddings in the FAISS vector database.
6. Retrieve relevant document chunks based on the user's query.
7. Generate answers using Google Gemini.
8. Display responses through the Streamlit interface.

---

## Libraries Used

- Streamlit
- LangChain
- LangChain Community
- LangChain Google GenAI
- Hugging Face Sentence Transformers
- FAISS
- PyPDF
- python-dotenv

---

## Learning Outcomes

This project demonstrates practical implementation of:

- Retrieval-Augmented Generation (RAG)
- Vector Databases (FAISS)
- Semantic Search
- Embedding Generation
- Document Question Answering
- Large Language Model Integration
- Streamlit Application Development

---

## Future Enhancements

- Support for multiple PDF documents
- Chat history
- Source citation
- OCR support for scanned documents
- Hybrid search
- ChromaDB support
- User authentication
- Docker deployment
- Cloud deployment

---

## Author

**Sehaj Kaur**

GitHub: https://github.com/Sehajkaur24

---

## License

This project is intended for educational and learning purposes.
