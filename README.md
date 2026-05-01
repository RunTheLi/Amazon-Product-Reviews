# Explainable AI: Sentiment Analysis (LIME vs SHAP)

## Project Overview

This project builds a **sentiment analysis model** using Amazon product reviews and explains predictions using **Explainable AI (XAI)** techniques.

The model classifies reviews into:
-  Positive sentiment  
-  Negative sentiment  

---

## Machine Learning Pipeline

- Data: Amazon Product Reviews
- Feature Extraction: TF-IDF
- Model: Logistic Regression
- Evaluation: Accuracy, Precision, Recall, F1-score

---

## Explainable AI

### LIME (Local Explanation)
- Explains individual predictions
- Shows which words influence a single prediction
- Uses perturbation (removing words and observing changes)

### SHAP (Global + Local Explanation)
- Based on Game Theory (Shapley Values)
- Measures contribution of each feature
- More stable but computationally heavier than LIME

---

## LIME vs SHAP

| Feature | LIME | SHAP |
|----------|------|------|
| Type | Local explanation | Local + Global explanation |
| Method | Feature perturbation | Game theory |
| Speed | Fast | Slower |
| Stability | Medium | High |

---

## Workflow

Text → TF-IDF → Logistic Regression → Prediction → LIME / SHAP Explanation

---

## Tech Stack

- Python
- Pandas
- Scikit-learn
- Matplotlib
- LIME
- SHAP

---

## Goal

To build a machine learning model that not only predicts sentiment but also explains why the prediction was made.

---

ML & NLP Explainability Project


## Kaggle source

- File = Review.csv
https://www.kaggle.com/datasets/arhamrumi/amazon-product-reviews
