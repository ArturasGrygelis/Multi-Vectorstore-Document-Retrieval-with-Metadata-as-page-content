# Multi-Vectorstore-Document-Retrieval-with-Metadata-as-page-content
 Data Preprocess for Multi-Vectorstore Document Retrieval with Metadata as page content in the smallest vectostore

## Overview

This project demonstrates an effective method for preprocessing documents and creating multiple metadata-enriched vector stores to optimize document retrieval and grading workflows. The focus is on minimizing text size per vector entry while maximizing useful information, enabling faster and more accurate retrieval downstream.

This is a **demonstration project** for learning and experimentation purposes, showcasing how to preprocess document data effectively and build efficient vector stores—not a complete application.

The approach resembles LangChain’s multi-vectorstore technique but offers advantages in memory usage and speed, while reducing hallucination risks in language model tasks by limiting the amount of text per vector entry. The project leverages well-structured document naming conventions for easy metadata extraction and supports flexible filtering for improved retrieval.

## Features

- Load and preprocess PDF documents with structured metadata extraction
- Build multiple vector stores containing different levels of detail (full content vs. concise metadata)
- Demonstrate efficient retrieval and reranking using base and instruct retrievers
- Enable filtering by metadata such as application deadlines and city
- Show how minimal text per vector entry reduces hallucination and improves retrieval speed

## Project Structure

- **Jupyter Notebook:** Main exploratory workflow illustrating step-by-step data preprocessing, metadata extraction, vectorstore creation, and retrieval testing
- **Data:** Example documents with extracted metadata
- **Vector Stores:** Multiple vector stores initialized for different retrieval scenarios

## Usage

1. Clone the repository
2. Install required packages (`langchain`, `pandas`, `seaborn`, `matplotlib`, etc.)
3. Run the Jupyter Notebook to follow the data preprocessing and vector store creation process
4. Experiment with retrieval queries and filtering using the notebook cells

## Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab
- `langchain`
- `pandas`
- `seaborn`
- `matplotlib`
- Access to LLM APIs such as ChatGroq for metadata extraction and embeddings

## Notes

- Document filenames with consistent structure improve metadata extraction accuracy
- Metadata filtering supports project-specific queries such as application deadlines or city-based document retrieval
- The focus on concise document text reduces large language model hallucinations and boosts retrieval performance

## Future Directions

- Explore agentic retrieval methods that dynamically select metadata fields using LLMs
- Adapt the approach for less-structured documents by automating metadata identification
- Develop backend services for scalable document search and grading based on these vector stores

## License

This project is provided for educational and exploratory purposes under the MIT License.
