# MEDIBOT - Your Personal AI Assistant for Medical Queries

## Overview
MEDIBOT is an intelligent medical chatbot designed to assist users by providing answers to their medical queries. Utilizing advanced natural language processing techniques and a rich medical database, MEDIBOT aims to deliver accurate and concise information based on a vast medical textbook, "The Gale Encyclopedia of Medicine." 

## How It Works
MEDIBOT employs the LLaMA-2-7b model to process user inputs and retrieve relevant information from the indexed medical data. The application works as follows:

1. **Data Extraction**: Medical data is extracted from a PDF textbook using LangChain's PDF loader.
2. **Text Splitting**: The extracted data is split into manageable text chunks for efficient processing.
3. **Embeddings**: Hugging Face embeddings are generated for each text chunk to enable semantic search.
4. **Indexing**: The embeddings are stored in a Pinecone vector database for quick retrieval.
5. **Question Answering**: When a user submits a query, MEDIBOT retrieves relevant text chunks based on similarity and formulates a concise answer using the LLaMA model.

## Features
- **Interactive Chat Interface**: Users can easily interact with the chatbot through a user-friendly web interface.
- **Semantic Search**: MEDIBOT utilizes embeddings to perform similarity searches on the medical data, ensuring accurate results.
- **Concise Answers**: The bot is designed to provide responses within three sentences, ensuring clarity and brevity.
- **Scalability**: The use of Pinecone allows for scalable storage and retrieval of medical information.
- **Extensibility**: The codebase can be easily extended to include more features, such as additional datasets or improved NLP models.

## Tools Used
- **Programming Language**: Python
- **Frameworks**:
  - **Flask**: For building the web application.
  - **LangChain**: For document processing and embedding generation.
- **Model**: 
  - **LLaMA-2-7b**: A state-of-the-art language model for natural language understanding.
- **Data Storage**: 
  - **Pinecone**: For storing and retrieving vector embeddings.
- **Libraries**:
  - **sentence-transformers**: For generating embeddings.
  - **pypdf**: For loading PDF documents.
  - **python-dotenv**: For environment variable management.

## Conclusion

MEDIBOT serves as a powerful tool for users seeking quick and reliable answers to medical queries. By leveraging advanced machine learning techniques and a robust architecture, it bridges the gap between medical knowledge and user accessibility.
