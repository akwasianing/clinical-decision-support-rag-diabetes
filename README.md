# Clinical Decision Support Assistant Using Retrieval-Augmented Generation (RAG) for Type 2 Diabetes Management

## Project Overview

This project develops a Retrieval-Augmented Generation (RAG) clinical decision support assistant that answers Type 2 Diabetes management questions using the **American Diabetes Association (ADA) Standards of Care in Diabetes—2026** guidelines.

The project began with a baseline implementation using **Qwen2.5-3B-Instruct** and was later improved by upgrading to **Qwen3-14B** and integrating **Cross-Encoder (MS MARCO MiniLM-L6-v2)** re-ranking to improve retrieval quality before answer generation.

The system retrieves relevant guideline excerpts from a ChromaDB vector database and generates grounded responses with source citations. The final system was evaluated using quantitative retrieval metrics, citation evaluation, manual assessment of answer quality, and qualitative analysis.

## Features

- Retrieval-Augmented Generation (RAG)
- Knowledge base built from the ADA Standards of Care in Diabetes—2026
- Semantic retrieval using Sentence Transformer embeddings
- ChromaDB vector database
- Qwen2.5-3B-Instruct baseline model
- Qwen3-14B improved language model
- Cross-Encoder (MS MARCO MiniLM-L6-v2) re-ranking
- Source-aware retrieval
- Interactive clinical question-answering chatbot
- Grounded answers with source citations

## Technologies Used

- Python
- Jupyter Notebook
- Google Colab
- Hugging Face Transformers
- Sentence Transformers
- ChromaDB
- LangChain
- Qwen Models
- Cross-Encoder (MS MARCO MiniLM-L6-v2)

## Installation

```bash
git clone https://github.com/akwasianing/clinical-decision-support-rag-diabetes.git
cd clinical-decision-support-rag-diabetes
```
## Install Dependencies

```bash
pip install -r requirements.txt
```

## Data Files

The ADA guideline PDF documents are **not included** in this repository because they are copyrighted by the American Diabetes Association.

When running the notebook, you will be prompted to upload the required ADA guideline PDF files before they are processed.

## Usage

### Local

```bash
jupyter notebook
```

Open the notebook and run all cells. When prompted, upload the required ADA guideline PDF files.

### Google Colab

Open the notebook in Google Colab and run all cells. When prompted, upload the required ADA guideline PDF files.

## Evaluation

The system was evaluated using the following metrics:

- Mean Precision@3
- Hit Rate@3
- Citation Accuracy
- Hallucinated Citation Rate
- Manual evaluation of relevance, faithfulness, and clarity

## Results

The final system achieved the following results:

- Mean Precision@3 improved from **0.800** to **0.844**
- Hit Rate@3: **1.000**
- Citation Accuracy: **100%**
- Hallucinated Citation Rate: **0%**

## Disclaimer

This project was developed for educational and research purposes only. It is **not** intended to replace professional medical advice, diagnosis, or treatment.

## Author

**Obed Akwasi Aning**
