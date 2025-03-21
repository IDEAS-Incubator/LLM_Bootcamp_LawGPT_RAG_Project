# bootcamp_lawgpt

LAWGPT is a legal assistant chatbot built using Retrieval-Augmented Generation (RAG) technology. This project helps users ask legal questions and get accurate responses based on legal documents and knowledge.

## Project Overview

LAWGPT uses a combination of:

- **Large Language Models** (via Ollama)
- **Vector Embeddings** for document understanding
- **Retrieval-Augmented Generation (RAG)** to provide accurate and sourced legal information

## Prerequisites

- Python 3.8 or higher
- Git
- 8GB+ RAM recommended
- 10GB+ free disk space

## Installation Guide

### Step 1: Clone the Repository

```bash
git clone https://github.com/IDEAS-Incubator/LLM_Bootcamp_LawGPT_RAG_Project.git
```

### Step 2: Set Up Python Environment

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate

```

### Step 3: Install Ollama

#### Ollama is an easy way to run LLMs locally.

```bash

For macOS:
curl -fsSL https://ollama.com/install.sh | sh

For Linux:
curl -fsSL https://ollama.com/install.sh | sh

For Windows:

Download the installer from Ollama's official website
Run the installer and follow the on-screen instructions


```

### Step 4: Download Required Models

```bash
# Pull the llama2 model for text generation
ollama pull llama2

# Pull the embedding model for vector embeddings
ollama pull nomic-embed-text

```

### Step 5: Run the Application

```bash
python code.py
python embedding.py
# Copy your legal documents into this directory
```

### Project Structure you can follow

```bash
lawgpt/
├── app.py                    # Main application file
├── scripts/
│   ├── generate_embeddings.py  # Script to generate document embeddings
│   └── preprocess_docs.py      # Script for document preprocessing
├── modules/
│   ├── embedding.py           # Embedding functionality
│   ├── llm.py                 # LLM interaction code
│   └── retrieval.py           # Vector retrieval functionality
├── data/
│   ├── documents/             # Your legal document files
│   └── embeddings/            # Generated embedding files
├── templates/                 # Web UI templates
└── requirements.txt           # Python dependencies
```
