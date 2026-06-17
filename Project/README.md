Laptop Price Prediction using Machine Learning

Project Overview
This project focuses on predicting laptop prices based on hardware specifications such as RAM, processor type, graphics card, storage, and display features. The goal is to build an accurate regression model using machine learning techniques and feature engineering.

Dataset
The dataset contains laptop specifications including:
CPU details
GPU details
RAM size and type
Storage capacity
Display resolution and size
Rating and model information

Data Preprocessing
Handled missing values
Removed high-cardinality column (Model)
Encoded categorical variables (Graphics, Generation)
Feature engineering:
Extracted core_count and thread_count from CPU data
Created PPI (Pixels Per Inch) from resolution and screen size

Exploratory Data Analysis
Distribution analysis using histograms
Correlation heatmap using Pearson correlation
Feature relationship with target variable (Price)


Models Used
The following models were trained and evaluated:
Linear Regression
Ridge Regression
Bayesian Ridge
KNN Regressor
Decision Tree
Random Forest
XGBoost

Hyperparameter Tuning
GridSearchCV (KNN)
RandomizedSearchCV (Random Forest)

Best Model
Random Forest Regressor
Cross Validation R² Score: ~0.82

Most important features:
RAM Size
Graphics Type
Processor Threads
PPI
Core Count

Key Learnings
Feature engineering had a bigger impact than model selection
Random Forest performed more consistently than other models
CPU and GPU features strongly influence laptop price
Cross-validation gave more reliable performance than a single train-test split

Tech Stack
Python
Pandas, NumPy
Scikit-learn
Matplotlib, Seaborn
Scikit-learn
Matplotlib, Seaborn
