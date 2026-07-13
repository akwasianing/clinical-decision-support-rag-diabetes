# Clinical Decision Support Assistant Using Retrieval-Augmented Generation (RAG) for Type 2 Diabetes Management

## Project Overview

This project develops a Retrieval-Augmented Generation (RAG) clinical decision support assistant that answers Type 2 Diabetes management questions using the **American Diabetes Association (ADA) Standards of Care in Diabetes—2026** guidelines.

The project began with a baseline implementation using **Qwen2.5-3B-Instruct** and was later improved by upgrading to **Qwen3-14B** and integrating **Cross-Encoder re-ranking** to improve retrieval quality before answer generation. The system retrieves relevant guideline excerpts from a ChromaDB vector database and generates grounded responses with source citations.

---

## Features

- Retrieval-Augmented Generation (RAG)
- Knowledge base built from the ADA Standards of Care in Diabetes—2026
- Semantic retrieval using Sentence Transformer embeddings
- ChromaDB vector database
- Qwen2.5-3B-Instruct (baseline language model)
- Qwen3-14B (improved language model)
- Cross-Encoder (MS MARCO MiniLM-L6-v2) re-ranking
- Source-aware retrieval
- Interactive clinical question-answering chatbot

---

## Technologies Used

- Python
- Hugging Face Transformers
- Sentence Transformers
- ChromaDB
- Qwen2.5-3B-Instruct
- Qwen3-14B
- Cross-Encoder (MS MARCO MiniLM-L6-v2)

---

## Repository Structure

```
notebooks/
    Jupyter notebooks used for development and experimentation

```

---

## Project Progress

- Developed the project proposal.
- Selected the ADA Standards of Care in Diabetes—2026 as the knowledge source.
- Processed the guideline documents.
- Split documents into text chunks.
- Generated embeddings.
- Built the ChromaDB vector database.
- Developed the baseline RAG pipeline.
- Integrated Qwen2.5-3B-Instruct.
- Built an interactive chatbot for question answering.
- Upgraded the language model to Qwen3-14B.
- Improved prompt design and source-aware retrieval.
- Evaluated the updated RAG pipeline using five clinical questions.
- Added Cross-Encoder (MS MARCO MiniLM-L6-v2) re-ranking.
- Evaluated the updated retrieval pipeline using the same five clinical questions.
- Improved retrieval quality before answer generation.

---

## Author

**Obed Akwasi Aning**



