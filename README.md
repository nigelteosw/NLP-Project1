# Job Recommendation System – NLP Project (1120-DS000-MSA-0234)

A modern AI-powered job matching system that bridges the gap between resumes and job descriptions using **Natural Language Processing** and **deep learning**. Built with a **Two-Tower Embedding Model**, this project enables accurate, scalable, and semantically rich candidate-job matching for the future of recruitment.

---

## Overview

This project develops a **job recommendation system** that efficiently matches resumes to job descriptions using:

- **Two-Tower Embedding Model**
- **Contrastive Learning**
- **Sentence-BERT (Transformer-based embeddings)**
- **TF-IDF keyword features**
- **FAISS** for fast similarity search
- **Cosine Similarity** for match scoring

The system encodes job descriptions and resumes into a **shared high-dimensional space**, allowing for semantic similarity comparison beyond keyword matching.

---

## How It Works

1. **Data Preprocessing**  
   - Clean and tokenize job descriptions and resumes  
   - Apply Named Entity Recognition (NER) to extract key skills  
   - Generate embeddings using **Sentence-BERT** and **TF-IDF**

2. **Model Architecture**  
   - Two independent towers:
     - **Job Tower**: Encodes job descriptions
     - **Resume Tower**: Encodes resumes
   - Both towers map inputs into a **shared vector space**
   - Trained using **contrastive loss** to distinguish good matches from poor ones

3. **Similarity Scoring**  
   - **FAISS** performs fast nearest-neighbor search in embedding space  
   - **Cosine similarity** calculates match scores  
   - Top resumes are ranked by **semantic and skill-based relevance**

4. **User Query Support**  
   - Input: job description or personal resume text  
   - Output: Ranked list of resumes (or jobs) with **match percentage**

---

## Features

✅ Deep learning-powered resume-job matching  
✅ Semantic understanding using Sentence-BERT  
✅ Keyword importance with TF-IDF  
✅ Real-time search with FAISS  
✅ Custom resume input supported  
✅ Cosine similarity score for transparency  

---

## Use Cases

- **Recruiters**: Quickly find the best candidate for a job  
- **Job Seekers**: See which job descriptions fit their resumes  
- **HR Tech Platforms**: Build smarter job search engines and match systems  
- **Educational Institutions**: Help students find suitable internships or job roles  

---

## Future Work

- Fine-tuning transformer embeddings on domain-specific resume/job corpora  
- Incorporating additional metadata such as years of experience, education level  
- Exploring alternative loss functions (e.g., triplet loss, batch hard mining)  
- Adding bias detection and fairness auditing  
- Expanding support for multilingual job markets  

---

## 🙌 Acknowledgements

This project was developed as part of the **Natural Language Processing (1120-DS000-MSA-0234)** module. Special thanks to all instructors and peers who provided valuable feedback.

