#  Local AI Agent using Python, Ollama, LangChain & RAG

A fully local, offline AI agent powered by **Python**, **Ollama**, **LangChain**, and **RAG (Retrieval-Augmented Generation)**.  
This repository contains the working demo of how the agent retrieves data from a vector store and answers questions using **LLaMA 3.2** — completely offline.

---

##  YouTube Demo

👉 https://youtu.be/ZPaL432dTYE

---

##  Project Overview

This project demonstrates the working of a **local AI Agent** that:

- Loads restaurant reviews from a CSV file  
- Converts them into embeddings  
- Stores them in a **Chroma vector database**  
- Retrieves relevant data when a user asks a question  
- Uses **LLaMA (Ollama)** to generate responses with context  

This video and repository showcase **only the working demo**, not a full tutorial.

---

## ✔ Features

-  **100% offline** (no API keys or cloud services)  
-  Fast retrieval using **ChromaDB**  
-  Embeddings generated using **mxbai-embed-large**  
-  Answer generation using **LLaMA 3.2 (via Ollama)**  
-  Simple and clean Python scripts  
-  RAG pipeline (Retrieve → Inject into Prompt → LLM Answer)

---

##  Tech Stack

| Technology          | Usage                       |
|---------------------|-----------------------------|
| **Python**          | Core logic & scripting       |
| **Ollama**          | Running LLaMA locally        |
| **LangChain**       | Prompting, chains, retrievers|
| **ChromaDB**        | Local embedding vector DB    |
| **mxbai-embed-large** | Embedding model            |
| **Pandas**          | CSV handling                |

---

##  Project Structure

.
├── main.py # Runs the AI Agent interaction loop
├── vector.py # Embeddings + Chroma vector store setup
├── realistic_restaurant_reviews.csv
├── requirements.txt
├── chrome_langchain_db/ # Auto-created persistent database
└── README.md

---

##  Installation & Setup

### 1️⃣ Install dependencies
pip install -r requirements.txt

### 2️⃣ Install Ollama
Download here: [https://ollama.com](https://ollama.com)

Then pull required models:
ollama pull llama3.2
ollama pull mxbai-embed-large

### 3️⃣ Run the Agent
python main.py

On first run, the system will:

- Load your CSV  
- Generate embeddings  
- Save them in Chroma  
- Begin answering questions  

---

##  How the System Works

1. **Load Data**  
The CSV contains restaurant titles, reviews, dates, and ratings.

2. **Embedding Creation**  
Each text entry is converted to a high-dimensional vector using mxbai embeddings.

3. **Store in ChromaDB**  
Documents and metadata are stored in a local folder (`chrome_langchain_db`).

4. **RAG Pipeline**  
User Question → Retriever → Relevant Reviews → LLM → Final Answer

5. **LLM Response**  
LLaMA reads the retrieved reviews and generates a clean, contextual answer.

---

##  Video Overview

Watch the full working demonstration:  

👉 https://youtu.be/ZPaL432dTYE

---

##  Future Enhancements

- Web UI using Streamlit / FastAPI  
- Chat-style UI  
- Multi-agent or tool-using agent  
- Support for larger datasets  
- Add memory to agent  
- Add voice input/output  

---

##  Contributing

Contributions are welcome!  
Feel free to submit an issue or pull request.

---

##  License

This project is licensed under the MIT License.

---

##  Support the Project

If this project helped you, please star the repository ⭐ to support more open-source work!

---

If you want, I can also generate:

- ✅ `requirements.txt`  
- ✅ A professional GitHub project icon/logo  
- ✅ A shorter README version  
Just tell me!


