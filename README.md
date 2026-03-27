# LocalAI
Local AI Question-Answering System (RAG) 

**A local Retrieval-Augmented Generation (RAG) system built with LangChain and Ollama. This project allows users to query a custom dataset of restaurant reviews privately on their own machine, ensuring data privacy while leveraging large language models.**

### 🛠 Technologies

**Framework:** LangChain (LangChain-Ollama, LangChain-Core)
**LLM Engine:** Ollama (running Llama 3.2)
**Vector Database:** ChromaDB (for efficient document retrieval)
**Language:** Python
**Data Format:** CSV (Realistic Restaurant Reviews)

### 🚀 Features

**100% Data Sovereignty:** Operates entirely on local hardware, ensuring sensitive data never leaves the organization's network.
**Intelligent Retrieval:** Implemented semantic search to provide the AI with specific context, significantly reducing "hallucinations" and increasing answer accuracy.
**Automated Data Pipeline:** Built a custom ingestion engine that transforms raw CSV data into structured, searchable vector intelligence.
**User-Centric Interface:** A responsive command-line interface designed for seamless user interaction.

### ⚙️ The Process

**Requirement Analysis**: Identified the need for a low-latency, private alternative to cloud-based AI for analyzing proprietary restaurant data.
**Architecture Design**: Developed a multi-stage pipeline: Data Ingestion → Vector Embedding → Contextual Retrieval → LLM Synthesis.
**Optimization**: Engineered a "Database-First" logic that detects existing vector stores to minimize computational overhead and startup time.
**Testing & Refinement**: Iteratively tuned system prompts to ensure the AI maintains a professional, expert-level persona during interactions.

### 🧠 What I Learned

**RAG Architecture**: Understanding the flow between a user query, a vector database, and an LLM to provide grounded answers.
**Local LLM Deployment:** Gained experience managing model parameters and performance using Ollama.
**Prompt Optimization:** Learning how to structure templates to effectively use retrieved context ({reviews}) and user input ({question}).
**Environment Management:** Setting up local virtual environments (.venv) to manage specialized AI libraries.
**Metadata Engineering:** I learned how to attach structured data (like ratings and dates) to vector embeddings, which allows for more complex filtering in a RAG pipeline.
**Idempotent Code Design:** I implemented logic to check if the database already exists (os.path.exists) before adding documents, preventing duplicate data and saving computational resources.
**Embedding Models:** Gained experience with mxbai-embed-large, understanding how different embedding models affect the accuracy of semantic search.

### 🏃 Running the Project

To run this project locally, ensure you have Ollama installed and the Llama 3.2 model pulled.

1. Install & Set Up Ollama
This project requires Ollama to serve the LLM and the Embedding model locally. Pull the Models.
2. Create a Virtual Environment
3. Install Dependencies.
4. Initialize & Run to begin querying the knowledge base.
