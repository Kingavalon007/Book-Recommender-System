# 📚 AI-Powered Semantic Book Recommender

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![AI](https://img.shields.io/badge/GenAI-Hugging%20Face-yellow)
![Library](https://img.shields.io/badge/Framework-LangChain-green)
![UI](https://img.shields.io/badge/Frontend-Gradio-orange)

## 📖 Overview

This project is a **Retrieval-Augmented Generation (RAG)** recommendation engine that allows users to find books based on natural language descriptions, emotional vibes, and deep semantic meaning.

Unlike traditional search engines that rely on exact keyword matching, this system uses **Vector Search** and **Open Source LLMs** to understand the *intent* behind a query. Users can search for specific feelings like *"a heartbreaking story about a robot who learns to love"* and get highly accurate results.

### ✨ Key Features
* **🧠 Semantic Search:** Uses **Hugging Face Embeddings** to convert text into vectors, allowing the system to understand context and nuance without needing exact keyword matches.
* **🏷️ Zero-Shot Classification:** Automatically tags books with missing genres (e.g., Fiction vs. Non-Fiction) using the `BART` model.
* **🎭 Sentiment Analysis:** Filters books by emotional tone (e.g., *Suspenseful, Joyful, Sad*) using the `DistilRoBERTa` emotion model.
* **💻 Interactive Dashboard:** A clean, responsive web interface built with **Gradio**.

---

## 🛠️ Tech Stack & Models

This project is built entirely on **Open Source** technologies to ensure data privacy and zero API costs. We replaced OpenAI components with high-performance Hugging Face models.

| Component | Technology / Model | Purpose |
| :--- | :--- | :--- |
| **Embeddings** | `sentence-transformers/all-MiniLM-L6-v2` | Converts book descriptions into vectors for semantic search. |
| **Classification** | `facebook/bart-large-mnli` | Performs Zero-Shot Classification to detect genres. |
| **Sentiment** | `j-hartmann/emotion-english-distilroberta-base` | Detects emotional tones (Joy, Fear, Surprise, etc.) in text. |
| **Vector DB** | ChromaDB | Stores and retrieves vector embeddings efficiently. |
| **Orchestration** | LangChain | Connects the data pipeline and models. |
| **UI** | Gradio | Provides the user-friendly web interface. |

---

## 📂 Project Structure

The project is modularized into specific stages of the machine learning pipeline:

```text
├── data_exploration.ipynb      # Step 1: Cleaning raw data & feature engineering
├── vector_search.ipynb         # Step 2: Generating embeddings & building ChromaDB
├── text_classification.ipynb   # Step 3: Using BART for Zero-shot genre classification
├── sentiment_analysis.ipynb    # Step 4: Using DistilRoBERTa for emotion extraction
├── app.py                      # Step 5: Main application script (Gradio UI)
└── README.md                   # Project documentation
