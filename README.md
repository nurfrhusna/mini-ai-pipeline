# Mini AI Pipeline: Text Sentiment Classification  
CAS2105 Homework 6  
Nur Farah Husna binti Junaidi (2024148067)

---

## 📌 Project Summary
This project implements a simple AI pipeline for classifying short English sentences into **positive** or **negative** sentiment.  
I compare a **naïve keyword-based baseline** with a **pretrained transformer model** (`distilbert-base-uncased-finetuned-sst-2-english`) and evaluate their performance on a small custom dataset of 40 sentences.

---

## 🧪 Methods Used
### 1. Naïve Baseline  
A simple keyword rule-based classifier.  
It works on explicit words but fails on subtle context or negation.

### 2. AI Pipeline  
A HuggingFace sentiment-analysis pipeline using DistilBERT.  
It handles context, negation, and more natural phrasing.

---

## 📊 Results
| Model | Accuracy |
|-------|----------|
| Baseline | **0.80** |
| DistilBERT Pipeline | **1.00** |

The AI model correctly identifies subtle emotional tone and handles edge cases where the baseline fails.

---

## 📁 Files in This Repository
- `text_sentiment_pipeline.ipynb` — full notebook with baseline + AI pipeline  
- `report.pdf` — full report using the official Overleaf template (required for HW submission)

---

## ▶️ How to Run the Notebook
1. Install dependencies:
   ```bash
   pip install transformers pandas scikit-learn
