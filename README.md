# Clinical Decision Support Assistant Using Retrieval-Augmented Generation (RAG) for Type 2 Diabetes Management

## Project Overview

This project develops a Retrieval-Augmented Generation (RAG) clinical decision support assistant that answers Type 2 Diabetes management questions using the **American Diabetes Association (ADA) Standards of Care in Diabetes—2026** guidelines.

The project began with a baseline implementation using **Qwen2.5-3B-Instruct** and was later improved by upgrading to **Qwen3-14B** and integrating **Cross-Encoder (MS MARCO MiniLM-L6-v2)** re-ranking to improve retrieval quality before answer generation. The system retrieves relevant guideline excerpts from a ChromaDB vector database and generates grounded responses with source citations. The final system was evaluated using quantitative retrieval metrics, citation evaluation, manual assessment of answer quality, and qualitative analysis.

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
- Quantitative and qualitative evaluation framework

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

```text
notebooks/
    Jupyter notebook used for development and experimentation
```

---

## Project Progress

- Developed the project proposal.
- Selected the ADA Standards of Care in Diabetes—2026 as the knowledge source.
- Processed the guideline documents.
- Split documents into text chunks.
- Generated document embeddings.
- Built the ChromaDB vector database.
- Developed the baseline RAG pipeline.
- Integrated Qwen2.5-3B-Instruct.
- Built an interactive chatbot for clinical question answering.
- Upgraded the language model to Qwen3-14B.
- Improved prompt design and source-aware retrieval.
- Added Cross-Encoder (MS MARCO MiniLM-L6-v2) re-ranking to improve document retrieval.
- Developed a structured evaluation dataset consisting of 15 Type 2 Diabetes management questions covering diagnosis, glycemic targets, lifestyle management, medication selection, and cardiovascular risk.
- Compared the baseline retrieval pipeline with the Cross-Encoder re-ranked pipeline.
- Evaluated retrieval performance using Mean Precision@3 and Hit Rate@3.
- Evaluated citation accuracy and hallucinated citation rate for both systems.
- Performed manual evaluation of answer relevance, faithfulness, and clarity.
- Conducted a qualitative analysis to identify the strengths and limitations of the final RAG system.
- Improved Mean Precision@3 from **0.800** to **0.844** while maintaining a Hit Rate@3 of **1.000**.
- Achieved **100% citation accuracy** with **no hallucinated citations** under the evaluation metric for both systems.
- Completed the evaluation and assessment of the final RAG system.

---

## Author

**Obed Akwasi Aning**
