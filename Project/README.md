# Laptop Price Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![Machine Learning](https://img.shields.io/badge/ML-Regression-green.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Used-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

---

## Project Overview
This project focuses on predicting laptop prices based on hardware specifications such as RAM, processor type, graphics card, storage, and display features. The goal is to build an accurate regression model using machine learning techniques and feature engineering.

---

## Dataset
The dataset contains laptop specifications including:

- CPU details  
- GPU details  
- RAM size and type  
- Storage capacity  
- Display resolution and size  
- Rating and model information  

---

## Data Preprocessing
- Handled missing values  
- Removed high-cardinality column (Model)  
- Encoded categorical variables (Graphics, Generation)  
- Feature engineering:
  - Extracted `core_count` and `thread_count` from CPU data  
  - Created PPI (Pixels Per Inch) from resolution and screen size  

---

## Exploratory Data Analysis
- Distribution analysis using histograms  
- Correlation heatmap using Pearson correlation  
- Feature relationships with target variable (Price)  

---

## Models Used
- Linear Regression  
- Ridge Regression  
- Bayesian Ridge  
- KNN Regressor  
- Decision Tree  
- Random Forest  
- XGBoost  

---

## Hyperparameter Tuning
- GridSearchCV for KNN  
- RandomizedSearchCV for Random Forest  

---

## Best Model
Random Forest Regressor  
Cross Validation R² Score: ~0.82  

---

## Most Important Features
- RAM Size  
- Graphics Type  
- Processor Threads  
- PPI  
- Core Count  

---

## Key Learnings
- Feature engineering had a larger impact than model selection  
- Random Forest performed more consistently than other models  
- CPU and GPU features strongly influence laptop price  
- Cross validation provided more reliable evaluation than a single train-test split  

---

## Tech Stack
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
