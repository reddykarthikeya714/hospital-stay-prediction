# Hospital Stay Duration Prediction

A machine-learning project that predicts a patient's hospital-stay **category** from structured hospital and patient-related data.

## Objective
Build and compare classification models to predict the stay-duration category represented by the `Stay` target.

## Data preparation
- Explore target distribution and feature relationships.
- Remove duplicate records.
- Impute missing numeric values with the median and categorical values with the most frequent value.
- One-hot encode categorical features.
- Scale numeric features for Logistic Regression.
- Exclude identifier columns from model inputs.

## Models
- Logistic Regression
- Decision Tree
- Random Forest

## Evaluation
Compare models using accuracy and weighted F1-score. Use a classification report and confusion matrix to inspect class-level performance. A DummyClassifier baseline is also included in the notebook workflow.

## Technologies
Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Jupyter Notebook

## Key concepts
Exploratory Data Analysis · Missing-Value Handling · Encoding · Feature Scaling · Classification · Model Comparison · Model Evaluation

*The target represents stay-duration ranges, not an exact number of days. This educational project is not intended for clinical decision-making.*
