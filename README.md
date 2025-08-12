# RAG-ChildSafety-SongFilter

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
## Files

- **notebooks/RAG-childSafety-songfilter.ipynb**: Full pipeline: embedding, retrieval, similarity, and decision logic.

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
git clone https://github.com/Azihadadi/RAG-ChildSafety-SongFilter.git
cd RAG-ChildSafety-SongFilter
```

2. Install dependencies:
```bash 
pip install -r requirements.txt
jupyter notebook notebooks/RAG-childSafety-songfilter.ipynb
```

---

## Future Work

- Incorporating lightweight LLMs for borderline cases.
- Expanding the knowledge base with more diverse QA pairs.
- Adding multilingual support for global content filtering.

---

## Contact

Feel free to connect if you're interested in this project or want to collaborate:

- GitHub: [Azadeh Hadadi](https://github.com/Azihadadi)
- LinkedIn: _[Azadeh Hadadi](https://www.linkedin.com/in/azadeh-hadadi/)_  
