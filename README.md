# DatasheetRAG
**DatasheetRAG** is a Retrieval-Augmented Generation system for embedded engineers that enables intelligent querying of hardware datasheets. It retrieves relevant sections using vector search and generates context-aware answers, helping users quickly understand registers, protocols, and configurations without manual search.

**Problem Statement**
Microcontroller datasheets are:
1.Large and complex
2.Difficult for beginners to understand
3.Contain dense technical information
Traditional search methods fail to provide contextual explanations.

**Solution**

This project implements a Traditional RAG pipeline that:
Parses datasheet PDFs
Splits content into chunks
Generates embeddings
Retrieves relevant sections
Uses an LLM to answer queries

**Architecture**

User Query --> Retriever (FAISS) --> Relevant Datasheet Chunks --? LLM (FLAN-T5 Large) -->Generated Answer

**Tech Stack**
Python
LangChain
FAISS (Vector Database)
HuggingFace Transformers
FLAN-T5 Large (LLM)
Sentence Transformers (Embeddings)
Google Colab
