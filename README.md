# Youtube_Chatboat_Using_RAG

This is a small Retrieval-Augmented Generation (RAG) project built using LangChain and Hugging Face.
It takes a YouTube video ID, extracts its transcript, splits it into smaller chunks, and creates a vector database using sentence-transformer embeddings.
When you ask a question, it retrieves the most relevant transcript parts and uses a TinyLlama model to generate an answer.

1) Extracts transcript of a given YouTube video using youtube-transcript-api.
2) Splits transcript into smaller chunks using RecursiveCharacterTextSplitter.
3) Creates embeddings for these chunks using sentence-transformers/all-MiniLM-L6-v2.
4) Stores embeddings in a Chroma vector database.
5) Performs similarity search to find relevant chunks for your question.
6) Generates an answer using "TinyLlama" through HuggingFacePipeline.
