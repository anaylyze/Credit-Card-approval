# Credit Card Approval Prediction Using Logistic Regression

This project builds a machine learning model to predict credit card application approval based on applicant data such as income, credit history, employment status, and demographic information. The workflow demonstrates end-to-end data preprocessing, feature engineering, and binary classification using logistic regression.

---

### **Project Overview**

- **Goal:** Predict whether a credit card application will be approved or rejected.
- **Techniques:** Data cleaning, handling missing values, encoding categorical variables, feature scaling, merging datasets, and logistic regression.
- **Evaluation:** Model performance is assessed using accuracy and classification metrics.

---

### **Dataset**

- **Application Data:** Includes applicant demographics, financial, and employment details.
- **Credit History Data:** Contains monthly credit status for each applicant.
- **Target Variable:** Created by aggregating credit status—applicants overdue by 60+ days at any point are labeled as "bad" (1), others as "good" (0).

---

### **Workflow**

1. **Data Preprocessing**
    - Handle missing values (mean/mode imputation)
    - Encode categorical variables (one-hot encoding, binary mapping)
    - Feature scaling (standardization of numerical features)
    - Merge application and credit history data on applicant ID
    - Create binary target variable from credit history

2. **Model Training**
    - Split data into training and test sets
    - Train a logistic regression classifier
    - Evaluate performance using accuracy and classification report

3. **Model Evaluation**
    - **Accuracy Achieved:** 

       Accuracy: 0.99998
     
    - **Classification Report:**
      ```
      precision    recall  f1-score   support

           0       1.00      1.00      1.00    155000
           1       1.00      1.00      1.00       543

      accuracy                         1.00    155543
      macro avg                        1.00    155543
      weighted avg                     1.00    155543
      ```

---

### **Key Results**

- **Outstanding accuracy (99.998%)** on the test set.
- Both classes (approved and rejected) are perfectly predicted in this evaluation.
- The model is robust after thorough preprocessing and feature engineering.
