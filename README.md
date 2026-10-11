# Enterprise RAG for HR Policy Documents

An AI-powered Retrieval-Augmented Generation (RAG) system that answers questions about HR policies using document retrieval and a local language model.

## Overview

This project demonstrates an end-to-end RAG pipeline for enterprise document question answering.

The system extracts text from an HR policy PDF, divides the text into meaningful chunks, creates embeddings, retrieves relevant information, and uses a local language model to generate answers.

## Key Features

- PDF text extraction using PyMuPDF
- Text cleaning and preprocessing
- Section-aware document chunking
- Semantic embeddings using SentenceTransformers
- Vector storage and retrieval using ChromaDB
- Keyword-enhanced relevance selection
- Local language model inference
- Source section identification
- Question-answering evaluation

## Tech Stack

- Python
- PyMuPDF
- SentenceTransformers
- ChromaDB
- Transformers
- Qwen2.5-1.5B-Instruct
- Google Colab

## Pipeline

1. Extract text from an HR policy PDF.
2. Clean the extracted text.
3. Divide the document into section-aware chunks.
4. Convert chunks into 384-dimensional embeddings.
5. Store embeddings in ChromaDB.
6. Retrieve relevant chunks for a user question.
7. Select relevant context using semantic and keyword matching.
8. Generate an answer using a local language model.
9. Identify the source policy section.

## Privacy

The original HR policy PDF is not included in this repository.

## Limitations

- Evaluation uses a small manually created question set.
- PDF extraction quality can affect retrieval.
- Small language models may produce incomplete answers.
- Some questions may require information from multiple chunks.

## Future Improvements

- Hybrid keyword and vector retrieval
- Better reranking
- Multi-chunk context aggregation
- More extensive evaluation
- A simple web interface
- Support for multiple documents

## Project Structure

```text
enterprise-rag-hr-policy/
├── README.md
├── requirements.txt
├── .gitignore
├── notebooks/
│   └── enterprise_rag.ipynb
├── data/
│   └── README.md
└── images/
```

## Author

Fatima Rahman

BRAC University — Computer Science and Engineering