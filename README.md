# RAG-ChildSafety-SongFilter

An efficient and scalable solution for content moderation of songs shared on social media using Retrieval-Augmented Generation (RAG).

## 🎯 Project Overview

This project presents a scalable and cost-efficient approach to content moderation of song lyrics shared on social media platforms, with a specific focus on child safety. Instead of relying on computationally expensive large language models (LLMs) for real-time analysis of every input, we leverage a Retrieval-Augmented Generation (RAG) pipeline to perform semantic evaluation.

The system retrieves pre-embedded question-answer pairs related to content appropriateness and compares them against new song inputs via vector similarity search. This enables efficient classification without compromising moderation quality, significantly reducing inference time and resource consumption.

---

## 🔧 Technologies & Tools Used

- **Python**
- **PyTorch**
- **Hugging Face Transformers**
- **SentenceTransformers**
- **Retrieval-Augmented Generation (RAG)**
- **Dot Product Similarity for Embedding Matching**
- **Jupyter Notebook**

---

## 📂 Files

- `RAG_with_PyTorch.ipynb`: Main notebook that implements the embedding generation, retrieval logic, similarity computation, and decision mechanism.

---

## 🚀 How It Works

1. **Pre-defined QA Embeddings**: A set of child-appropriateness questions and their corresponding “safe” or “not safe” answers are embedded.
2. **Song Embedding**: Lyrics of a new song are embedded using the same model.
3. **Retrieval**: Similarity (via dot product) is computed between the song and the QA embeddings.
4. **Decision**: Based on the top similar matches, a decision is made on whether the song is child-friendly.

---

## 🧠 Future Work

- Incorporating lightweight LLMs for borderline cases.
- Expanding the knowledge base with more diverse QA pairs.
- Adding multilingual support for global content filtering.

---

## 💬 Feedback

Feel free to fork this repo, raise issues, or suggest improvements via pull requests. Your feedback is welcome!
