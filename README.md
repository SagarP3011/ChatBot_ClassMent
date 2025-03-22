# ChatBot_ClassMent

# RAG-Based Chatbot for Job Role Learning
This project implements a Retrieval-Augmented Generation (RAG) chatbot that helps users retrieve relevant learning resources for different job roles based on a PDF document. It uses FAISS for vector search, LLM (Mistral) for response generation, and LangChain for retrieval and processing.

# Features
1. Loads a structured PDF containing job role learning resources
2. Uses FAISS to store and search document embeddings
3. Retrieves relevant information based on user queries
4. Uses LLM (Mistral) to generate refined responses
5. Built with LangChain, FAISS, and OpenAI/HuggingFace APIs

# How It Works
1.Loads PDF Documents (data/) and extracts text

2.Splits text into chunks using RecursiveCharacterTextSplitter

3.Embeds text using Hugging Face's sentence-transformers

4.Stores embeddings in FAISS for fast retrieval

5.Queries the FAISS index to retrieve the most relevant text

6.Sends retrieved context to LLM to generate responses

7.Returns a refined, contextual answer

# Example Queries
Try asking:
 "What are the best courses for becoming a Data Scientist?"
 "Which books should I read to become a Software Engineer?"
 "What communities are useful for Product Managers?"
