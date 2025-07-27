# rag-chatbot-loan-data
Implements a context-aware question-answering chatbot using FAISS vector store for semantic search and a transformer-based language model (Mistral) for generating responses.

# 💬 RAG-based Chatbot with Mistral & FAISS

This repository contains a Retrieval-Augmented Generation (RAG) chatbot built using the **Mistral-7B-Instruct** language model and **FAISS** for semantic search. The chatbot can answer user queries based on a custom dataset.

---

## 🔧 Features

- **RAG Architecture**: Retrieves relevant documents using embeddings + FAISS and uses a large language model to generate context-aware answers.
- **Mistral-7B-Instruct**: Open-source LLM from Hugging Face for generating accurate and human-like responses.
- **FAISS**: Efficient similarity search over embedded documents.
- **Colab Compatible**: All steps can be run on Google Colab (free or Pro).

---

## 🧠 Tech Stack

- 🧠 Model: `mistralai/Mistral-7B-Instruct-v0.1`
- 🔎 Retriever: FAISS
- 🧰 Embeddings: `sentence-transformers/all-MiniLM-L6-v2`
- 🔤 Tokenizer & Generator: Hugging Face Transformers
- 📦 Dependencies managed via `requirements.txt`

📦rag-chatbot
┣ 📄 assignment8_chatbot.ipynb # Main notebook
┣ 📄 requirements.txt # List of dependencies
┣ 📄 README.md # Project overview
┗ 📁 data # Your source dataset (CSV, XLSX, etc.)

## 🚀 How to Run

1. **Clone this repository**  
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>

   Install dependencies
pip install -r requirements.txt

Run the notebook
Open assignment8_chatbot.ipynb in Jupyter or Google Colab.

Ask questions!
You can query things like:

"What was the loan status of the applicant with income 3000?"

🔐 Authentication (Hugging Face)
For gated models like Mistral:

Create a Hugging Face account

Accept model terms

Add your token via:
from huggingface_hub import login
login(token="your_huggingface_token")

🛠️ Future Work
Deploy as a Streamlit or Gradio app

Add PDF/HTML ingestion support

Use LangChain or Haystack for pipeline abstraction

🙋‍♀️ Author
Tamanna Aggarwal
🧠 Passionate about Machine Learning
📫 tamanna08aggarwal@gmail.com
