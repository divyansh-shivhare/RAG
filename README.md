# RAG

Overview
This repository contains a Python script that demonstrates the use of various large language models (LLMs) for a question-answering chatbot interface using Gradio. The models used in the script include Ollama and Groq. The chatbot is designed to assist with robot customer support by retrieving and using relevant context to answer questions concisely.

Requirements
Ensure you have conda installed. The required Python packages are listed in the requirements.txt file.

Installation
Follow these steps to create a conda environment and install the required packages:

bash
Copy code
# Create a new conda environment
conda create --name RAG python=3.11 --file requirements.txt

# Activate the environment
conda activate RAG
Usage
Script: Mitra Robot RAG Chatbot
This script demonstrates how to use the Ollama and Groq models to create a chatbot for robot customer support. The chatbot uses Gradio for the user interface and retrieves context from a pre-loaded document database to answer questions.

How It Works
Load the Document Database: The script uses OllamaEmbeddings to create embeddings for the documents and stores them in a Chroma vector store.
Set Up the Chatbot: The chatbot is set up using Gradio's ChatInterface and uses the ChatGroq model for generating responses.
Answering Questions: When a user sends a message, the chatbot retrieves relevant context from the document database and generates a concise response using the Groq model.

Acknowledgements
Langchain
Gradio
Anthropic
Groq
Feel free to contribute to this project by opening issues or submitting pull requests.
