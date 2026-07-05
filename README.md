# 📚 Intelligent Research Paper Discovery System

## Overview

Finding relevant research papers from a large collection of publications can be difficult, especially when traditional search methods rely only on exact keywords. This project aims to make the process more efficient by combining semantic search with Natural Language Processing (NLP) techniques.

The system understands the meaning of a user's query, retrieves the most relevant research papers, extracts important keywords and entities, and generates a concise summary of each paper. This helps users quickly identify papers that are closely related to their research interests.

The system combines dense semantic retrieval with keyword evidence and enriches the retrieved papers using Named Entity Recognition, keyphrase extraction, abstractive summarization, and explainable relevance information.
---

## Project Objectives

* Build a semantic search system for research papers.
* Retrieve relevant papers using vector similarity search.
* Improve search quality through hybrid ranking.
* Extract important keywords from research papers.
* Identify useful entities such as organizations, technologies, and researchers.
* Generate short summaries for quick understanding.

---

## Features

* 🔍 Semantic search using Sentence Transformers
* ⚡ Fast similarity search with FAISS
* 🏷 Keyword extraction using KeyBERT
* 🧠 Named Entity Recognition (NER) with spaCy
* 📝 Automatic paper summarization using BART
* 📄 Displays title, abstract, keywords, entities, and summary for each retrieved paper

---

## 🛠️ Tech Stack

| Layer | Tool |
|---|---|
| Dataset | [CShorten/ML-ArXiv-Papers](https://huggingface.co/datasets/CShorten/ML-ArXiv-Papers) (Hugging Face) |
| Embeddings | `sentence-transformers` — `all-MiniLM-L6-v2` (384-dim) |
| Vector Search | `faiss-cpu` — `IndexFlatIP` (cosine similarity via L2-normalized inner product) |
| Summarization | `transformers` — `sshleifer/distilbart-cnn-12-6` |
| Keyword Extraction | `keybert` |
| Data handling | `pandas`, `numpy` |
| Web App | `streamlit` |

---

## Project Workflow

1. Load the research paper dataset.
2. Perform basic preprocessing and data cleaning.
3. Generate sentence embeddings for paper abstracts.
4. Build a FAISS index for efficient similarity search.
5. Search papers based on semantic similarity.
6. Apply hybrid ranking to improve search relevance.
7. Extract keywords from the retrieved papers.
8. Perform Named Entity Recognition (NER).
9. Generate concise summaries of the selected papers.
10. Display the final results in an organized format.

---

## Sample Output

For a given research query, the system provides:

* Paper Title
* Similarity Score
* Important Keywords
* Named Entities
* AI-Generated Summary

This allows users to understand the relevance of a paper before reading the complete document.

---

## Future Improvements

Some possible enhancements for this project include:

* Integrating the Semantic Scholar or arXiv API for live paper search.
* Building a simple web interface using Streamlit.
* Adding filters based on publication year, author, or research domain.
* Supporting multilingual research paper search.

---

## Learning Outcomes

Through this project, I gained practical experience with:

* Natural Language Processing (NLP)
* Semantic Search
* Sentence Embeddings
* Vector Databases using FAISS
* Keyword Extraction
* Named Entity Recognition
* Transformer-based Text Summarization

---


## Author

**Sameer Ahmad**

B.Tech – Information Technology

This project was developed as part of a Machine Learning & NLP internship to explore practical applications of semantic search and modern NLP techniques for research paper discovery.
