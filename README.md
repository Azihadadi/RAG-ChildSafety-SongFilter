# RAG-childsafety-songfilter

Efficient, scalable content moderation for song lyrics ensuring child safety—built using a **Retrieval‑Augmented Generation (RAG)** pipeline instead of heavy LLM inference.

## Overview

- **Context**: Moderating song lyrics on social media for child safety.
- **Approach**: Use pre-built QA embeddings, similarity search, and retrieval to classify songs as safe or not.
- **Benefit**: Fast, resource-light, and effective moderation.

---
## Tech Stack
- PyTorch                    
- Hugging Face Transformers  
- SentenceTransformers       
- Transformers               
- NumPy                      
- Python / Jupyter Notebook 

---

##  Workflow Overview

1. **Embed QA pairs** (child-safety questions/answers)  
2. **Embed song lyrics**  
3. **Compute similarity** (dot product / cosine over top-N)  
4. **Decide safety** based on retrieved top pairs  

---

## Setup Instructions

1. Clone the repo:
```bash
git clone https://github.com/Azihadadi/RAG-childsafety-songfilter.git
cd RAG-ChildSafety-SongFilter
```

2. Install dependencies:
```bash 
pip install -r requirements.txt
jupyter notebook notebooks/RAG-childsafety-songfilter.ipynb
```

---

## Future Work

- Incorporating lightweight LLMs for borderline cases.
- Expanding the knowledge base with more diverse QA pairs.
- Adding multilingual support for global content filtering.

---

