# Fake News Detection using NLP and Machine Learning
![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![Machine Learning](https://img.shields.io/badge/ML-Regression-green.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Used-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

A complete Fake News Detection project built using **Natural Language Processing (NLP)** and **Classical Machine Learning**. 
This project classifies news articles as **Real** or **Fake** using TF-IDF feature extraction and multiple machine learning algorithms.

---

## Project Overview

The objective of this project is to build a robust fake news classifier while following a complete machine learning workflow, including:

- Data Exploration (EDA)
- Data Cleaning
- Data Leakage Detection
- Duplicate Analysis
- Text Preprocessing
- TF-IDF Feature Extraction
- Model Training
- Cross Validation
- Model Evaluation
- Error Analysis

---

## Dataset

Dataset Source:
- Fake.csv
- True.csv

Both datasets were merged into a single binary classification dataset.

---

## Data Preprocessing

The following preprocessing steps were performed:

- Merged title and article text
- Converted text to lowercase
- Removed punctuation
- Removed emojis and non-ASCII characters
- Removed extra spaces
- Removed stopwords
- Applied verb lemmatization
- Converted text into TF-IDF vectors

---

##  Data Quality Checks

Several important issues were identified before training:

- Data leakage detected in the `subject` column
- Conflicting duplicate articles removed
- Duplicate records removed
- Source-specific word analysis performed

---

##  Models Used

- Multinomial Naive Bayes
- Logistic Regression
- Linear Support Vector Machine (SVM)

---

## Model Performance

| Model | Accuracy |
|--------|----------|
| Naive Bayes | 92.99% |
| Logistic Regression | 98.72% |
| Linear SVM | **99.41%** |

Linear SVM achieved the highest accuracy and the most consistent cross-validation performance.

---

##  Additional Experiment

Feature importance analysis revealed that words such as **"Reuters"** and **"say"** strongly influenced model predictions.

An additional experiment removed these words and retrained all models.

The models experienced only a small decrease in accuracy (0.24–0.52%), indicating that they learned broader linguistic patterns rather than relying solely on source-specific information.

---

##  Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- 5-Fold Cross Validation
- ROC Curve
- Confusion Matrix
- Feature Importance
- Error Analysis

---

##  Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib

---

##  Future Improvements

- Word Embeddings (Word2Vec / GloVe)
- LSTM-based models
- Transformer models (BERT)
- Real-time fake news prediction
- Model deployment using Flask or FastAPI

---

##  Key Learning Outcomes

This project demonstrates:

- End-to-end NLP pipeline development
- Detection and handling of data leakage
- Classical machine learning for text classification
- Model comparison and evaluation
- Feature importance analysis
- Practical experimentation to improve model generalization

---

##  Best Model

**Linear SVM**
- Accuracy: **99.41%**
- Excellent cross-validation stability
- Best overall performance among the evaluated models
