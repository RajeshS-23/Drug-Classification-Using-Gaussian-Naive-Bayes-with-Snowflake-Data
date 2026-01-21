# Drug Classification Using Gaussian Naive Bayes with Snowflake Data

## Overview
This project implements a machine learning classification model to predict drug categories based on patient and clinical attributes.  
The dataset is retrieved from a Snowflake data warehouse and processed using feature encoding and scaling techniques before training a Gaussian Naive Bayes classifier.

The project demonstrates an end-to-end workflow from database connection to model evaluation.

---

## Technologies Used
- Python
- Pandas, NumPy
- Snowflake Connector for Python
- Scikit-learn
- Gaussian Naive Bayes

---

## Dataset
- Source: Snowflake Data Warehouse
- Target column: **DRUG**
- Input features include both numerical and categorical variables
- Categorical features are encoded using One-Hot Encoding
- Target labels are encoded using Label Encoding

---

## Project Workflow

1. Connect to Snowflake and load the dataset
2. Perform basic data inspection and exploration
3. Separate features (X) and target variable (y)
4. Encode target labels using LabelEncoder
5. Apply One-Hot Encoding for categorical features
6. Combine encoded categorical and numerical features
7. Split data into training and testing sets
8. Train Gaussian Naive Bayes model
9. Evaluate model using multiple performance metrics

---

## Model Used
**Gaussian Naive Bayes**

Gaussian Naive Bayes is suitable for classification problems with numerical features and assumes a normal distribution of data. It is fast, efficient, and works well with encoded categorical variables.

---

## Evaluation Metrics
The model performance is evaluated using:
- Accuracy Score
- Confusion Matrix
- Classification Report
- Matthews Correlation Coefficient (MCC)
- ROC AUC Score
- Balanced Accuracy Score

These metrics help ensure fair evaluation, especially in multi-class classification scenarios.

---

## Results
The trained model successfully classifies drug categories with good accuracy.  
Additional evaluation metrics confirm balanced and reliable performance across classes.

---

## How to Run the Project

1. Install required libraries:
   ```bash
   pip install pandas numpy scikit-learn snowflake-connector-python
