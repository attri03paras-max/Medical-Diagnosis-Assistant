# Medical-Diagnosis-Assistant
Medical Diagnosis Assistant built using Retrieval-Augmented Generation (RAG), LangChain, Llama 2, and ChromaDB. Processes medical PDFs, performs semantic search with vector embeddings, and generates context-aware answers using an LLM.
# 🩺 Medical Diagnosis Assistant using RAG, LangChain & Llama 2

![Python](https://img.shields.io/badge/Python-3.10-blue)
![LangChain](https://img.shields.io/badge/LangChain-RAG-success)
![LLM](https://img.shields.io/badge/LLM-Llama2-orange)
![VectorDB](https://img.shields.io/badge/Vector%20Database-ChromaDB-purple)
![License](https://img.shields.io/badge/License-MIT-green)

---

# 📌 Project Overview

Medical Diagnosis Assistant is a Retrieval-Augmented Generation (RAG) application that answers medical questions using a Large Language Model and a medical diagnosis manual as its knowledge source.

Instead of relying solely on the LLM's internal knowledge, the system retrieves relevant information from a medical PDF, converts it into vector embeddings, performs semantic similarity search, and supplies the retrieved context to the language model before generating an answer.

This approach significantly improves factual grounding and reduces hallucinations while enabling document-specific question answering.

---

# 🚀 Key Features

- 📄 PDF document ingestion
- 📚 Automatic text extraction
- ✂ Intelligent document chunking
- 🧠 Sentence-transformer embeddings
- 🔍 Semantic similarity search
- 🗂 Chroma Vector Database
- 🤖 Llama 2 GGUF integration
- 💬 Context-aware question answering
- 🏥 Medical document retrieval
- ⚡ Retrieval-Augmented Generation (RAG)

---

# 🏗️ System Architecture

```

Medical PDF
│
▼
PyMuPDF
(Text Extraction)
│
▼
Recursive Text Splitter
│
▼
Embeddings
(all-MiniLM-L6-v2)
│
▼
Chroma Vector Database
│
▼
Similarity Search
│
▼
Relevant Context
│
▼
Llama 2 (GGUF)
│
▼
Generated Medical Answer

```

---

# 🧠 Workflow

The project follows the standard Retrieval-Augmented Generation pipeline.

### Step 1

Load the medical diagnosis PDF.

### Step 2

Extract text from every page.

### Step 3

Split the document into overlapping chunks.

### Step 4

Generate semantic embeddings for every chunk.

### Step 5

Store embeddings inside ChromaDB.

### Step 6

Accept a user question.

### Step 7

Retrieve the most relevant document chunks.

### Step 8

Build a prompt using the retrieved context.

### Step 9

Generate the final response using Llama 2.

---

# 💻 Technologies Used

- Python
- LangChain
- LlamaCpp
- HuggingFace Embeddings
- ChromaDB
- Sentence Transformers
- PyMuPDF
- Hugging Face Hub
- Jupyter Notebook

---

# 📦 Libraries

```python
langchain
langchain-community
langchain-text-splitters
chromadb
sentence-transformers
huggingface-hub
llama-cpp-python
PyMuPDF
```

---

# 📂 Repository Structure

```
Medical-Diagnosis-RAG/
│
├── README.md
├── assets/
│
├── docs/
│
├── notebooks/
│   └── natural_language_processing.ipynb
│
└── reports/
```

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Medical-Diagnosis-RAG.git
```

Move into the project

```bash
cd Medical-Diagnosis-RAG
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
natural_language_processing.ipynb
```

Run every notebook cell sequentially.

---

# 📄 Input Document

The project accepts a medical diagnosis PDF as input.

Example:

```
medical_diagnosis_manual.pdf
```

The document is automatically processed through:

- Text Extraction
- Chunk Creation
- Vector Embedding
- Semantic Indexing

---

# 💬 Example Questions

The notebook demonstrates answering questions such as:

- What is the protocol for managing sepsis?
- What are the symptoms of appendicitis?
- What investigations confirm pneumonia?
- How is acute kidney injury diagnosed?
- What treatment is recommended for diabetic ketoacidosis?

---

# 🧠 Retrieval-Augmented Generation (RAG)

Unlike traditional chatbots, this system first retrieves relevant passages before generating an answer.

Benefits include:

- Better factual accuracy
- Reduced hallucinations
- Domain-specific knowledge
- Scalable document search
- Improved response quality

---

# 🔍 Vector Search

The application performs semantic search using sentence embeddings instead of keyword matching.

Advantages include:

- Meaning-based retrieval
- Better context understanding
- Robust search over long medical documents
- Faster information retrieval

---

# 📈 Future Improvements

- Streamlit Web Interface
- Multi-document support
- PDF upload feature
- Conversation memory
- Medical citation generation
- Clinical summarization
- OCR for scanned documents
- Hybrid search
- FAISS support
- API deployment
- Docker support
- Authentication

---

# 📊 Learning Outcomes

This project demonstrates practical experience with:

- Retrieval-Augmented Generation (RAG)
- Large Language Models
- LangChain
- Prompt Engineering
- Semantic Search
- Vector Databases
- Embedding Models
- Medical NLP
- Document Intelligence
- Generative AI Pipelines

---

# 🎯 Skills Demonstrated

- Natural Language Processing
- Large Language Models
- Retrieval-Augmented Generation
- LangChain Framework
- ChromaDB
- HuggingFace
- Python Programming
- AI Application Development
- Prompt Engineering
- Vector Search
- Document Processing

---

# 📜 License

This project is intended for educational and research purposes.

---

# 👨‍💻 Author

**Paras Attri**

AI & Machine Learning Engineer

Skills:
- Python
- Machine Learning
- Deep Learning
- Natural Language Processing
- LangChain
- Large Language Models
- Retrieval-Augmented Generation (RAG)
- Vector Databases
- Prompt Engineering

GitHub: https://github.com/yourusername

LinkedIn: https://linkedin.com/in/yourprofile

---

⭐ If you found this project useful, consider giving it a Star.
