# RockyBot: News Research Tool 📈

RockyBot is an AI-powered tool designed to search and retrieve insights from news articles. Utilizing advanced Natural Language Processing (NLP) techniques, FAISS for vector storage, and OpenAI's language models, RockyBot can quickly answer user queries based on news articles while providing source references.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
- [Usage](#usage)
- [License](#license)
- [Contributing](#contributing)

## Overview
**RockyBot** is designed for researching and answering queries based on news articles. Users can input the URLs of the news articles, and RockyBot processes the text, stores embeddings in a FAISS index, and retrieves answers to user questions with references to the source articles.

This project leverages various state-of-the-art machine learning and NLP techniques, making it a powerful tool for researchers, journalists, or anyone looking to analyze and extract information from news articles.

## Features
- **Article Processing**: Input URLs of news articles and automatically extract content.
- **Question Answering**: Ask questions based on the content of the news articles.
- **Source References**: Get references for the sources used in generating the answers.
- **FAISS Index**: Uses FAISS for efficient vector storage and retrieval.
- **OpenAI LLM**: Integrates OpenAI for generating embeddings and processing natural language queries.
- **Web Interface**: Streamlit-powered simple, user-friendly interface.

## Tech Stack
- **Programming Language**: Python
- **Libraries**:
  - [Langchain](https://github.com/hwchase17/langchain): For creating retrieval chains.
  - [Streamlit](https://streamlit.io/): For building the web interface.
  - [Sentence-Transformers](https://www.sbert.net/): For generating sentence embeddings.
  - [FAISS (Facebook AI Similarity Search)](https://github.com/facebookresearch/faiss): For vector storage and similarity search.
  - [Unstructured](https://unstructured-io.github.io/unstructured/): For processing and loading unstructured data from URLs.
  - [OpenAI API](https://openai.com/): For embeddings and LLM-powered query processing.
  - [Pickle](https://docs.python.org/3/library/pickle.html): For saving and loading the FAISS index.
  - [Dotenv](https://pypi.org/project/python-dotenv/): For environment variable management.

- **Database**: FAISS Vector Database for storing and retrieving embeddings.

## Installation

### Prerequisites
- Python 3.8 or higher
- [OpenAI API Key](https://beta.openai.com/signup/)
- [FAISS](https://github.com/facebookresearch/faiss) installed
- [Anaconda](https://www.anaconda.com/products/distribution) (recommended)

### Setup
Follow the steps below to set up the project:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/kru2710shna/RockyBot-News-Research-Tool-
   cd RockyBot-News-Research-Tool-
   ```
2. ** Create a Virtual Environment (using conda or venv):
   ```bash
   conda create --name rockybot python=3.8
    conda activate rockybot
   ```
3. **Install the Dependencies:

```bash
pip install -r requirements.txt
```

4. **Install Additional Dependencies:

```bash
pip install langchain
pip install unstructured
pip install python-magic
conda install -c conda-forge libmagic -y
```

### Usage

Once the app is running, follow these steps:

Enter News Article URLs: Use the sidebar to input up to three URLs of news articles.
Process the Articles: Click on the "Process URLs" button to fetch and load the content from the articles.
Ask a Question: After processing the articles, enter your question in the text input field and hit enter. The tool will generate an answer based on the content of the articles, along with the sources.
