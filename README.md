# 📚 Book Recommender System with LLMs

## 📖 Overview

This project demonstrates how to build a sophisticated recommendation engine that goes beyond simple keyword matching. By leveraging **Large Language Models (LLMs)** and **Vector Search**, this system allows users to find books based on natural language descriptions, emotional tone, and genre classification.

### Key Features
* **Semantic Search:** Find books based on plot descriptions (e.g., "a story about a wizard learning to fly") rather than just titles.
* **Zero-Shot Classification:** Automatically categorize books as "Fiction" or "Non-Fiction" using an LLM.
* **Sentiment Analysis:** Sort books by their emotional tone (Suspenseful, Joyful, Sad, etc.).
* **Interactive Dashboard:** A user-friendly web interface built with Gradio.

---

## 📂 Project Structure & Learning Modules

The project is divided into five distinct components, each contained in a specific notebook or script:

| Component | File | Description |
| :--- | :--- | :--- |
| **1. Data Preparation** | `data_exploration.ipynb` | Cleaning and preprocessing the raw dataset. |
| **2. Vector Search** | `vector_search.ipynb` | Building the Vector Database (ChromaDB) to enable semantic search on book summaries. |
| **3. Text Classification** | `text_classification.ipynb` | Using LLMs for Zero-Shot classification to tag books (Fiction vs. Non-Fiction). |
| **4. Sentiment Analysis** | `sentiment analysis.ipynb` | Extracting emotions from text to allow sorting by tone/mood. |
| **5. Web Application** | `app.py` | The full-stack Python application that brings all components together in a UI. |

---

## 🛠️ Tech Stack

* **Core:** Python 3.11
* **Data Manipulation:** Pandas, KaggleHub
* **Visualization:** Matplotlib, Seaborn
* **AI & LLM:** LangChain, OpenAI (via LangChain), Transformers
* **Vector Database:** ChromaDB
* **Web UI:** Gradio

---

## 🚀 Getting Started

Follow these steps to set up the project locally.

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/semantic-book-recommender.git](https://github.com/your-username/semantic-book-recommender.git)
cd semantic-book-recommender
