# Resume Screening Automation

## 📌 Project Overview
This project automates the process of screening intern resumes by matching them with job descriptions using Natural Language Processing (NLP) techniques. It extracts key skills and experience from resumes and ranks candidates based on both keyword relevance and semantic similarity.

The goal is to reduce manual screening effort while improving accuracy and fairness in intern selection.

---

## 🎯 Objective
- Automate resume filtering
- Extract relevant skills and experience
- Match resumes with job descriptions
- Rank candidates based on relevance

---

## 🧠 Approach
The system uses a **hybrid NLP approach**:

1. **Text Extraction & Cleaning**  
   - Convert resumes into raw text (PDF/DOC)
   - Normalize text by removing noise (symbols, punctuation, stop words)

2. **Skill & Experience Extraction**  
   - Skills extracted using spaCy and predefined skill lists
   - Experience extracted using Regular Expressions (e.g., `2 years`, `6 months`)

3. **Resume–JD Matching**  
   - **TF-IDF + Cosine Similarity** for keyword-based matching
   - **BERT (Sentence Transformers)** for semantic similarity

4. **Score Combination**  
   - Weighted average of TF-IDF and BERT scores for final ranking

---

## 🛠️ Technologies Used
- Python
- spaCy
- NLTK
- Scikit-learn (TF-IDF, Cosine Similarity)
- Sentence-BERT (`sentence-transformers`)
- Regular Expressions

---

## 📂 Project Structure
```
resume-screening-automation/
│
├── data/
│   ├── resumes/
│   └── job_description.txt
│
├── src/
│   ├── text_preprocessing.py
│   ├── skill_extraction.py
│   ├── experience_extraction.py
│   ├── tfidf_matching.py
│   └── bert_matching.py
│
├── results/
│   └── ranked_candidates.csv
│
├── requirements.txt
└── README.md
```

---

## 🔍 Key Features
- Automated resume parsing
- Skill-based and semantic matching
- Hybrid scoring mechanism
- Scalable for large resume databases
- Reduces human bias in screening

---

## 📊 Sample Output
| Candidate | Skills Extracted | TF-IDF Score | BERT Score | Final Score |
|---------|------------------|--------------|------------|-------------|
| Resume_01 | Python, NLP, SQL | 0.45 | 0.82 | 0.67 |
| Resume_02 | ML, TensorFlow | 0.38 | 0.74 | 0.59 |

---

## ✅ Outcome
- Faster resume screening
- Improved matching accuracy
- Efficient intern shortlisting
- Explainable and extensible pipeline

---

## 🚀 Future Improvements
- Named Entity Recognition (NER) for better skill extraction
- Support for multiple job descriptions
- Resume classification by role
- Web-based interface for HR teams

---

## 🏁 Conclusion
This project demonstrates how NLP techniques like TF-IDF and BERT can be combined to build an effective and scalable resume screening system for intern hiring.

---

## 📌 Author
**Zubair Naseer**  
Aspiring AI / ML Engineer

