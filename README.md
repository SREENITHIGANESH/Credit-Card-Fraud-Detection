# Credit-Card-Fraud-Detection

# Fraud Detection Using Machine Learning

# Project Overview
The goal of this project is to build a machine learning model that can effectively distinguish between fraudulent and legitimate transactions.  
The dataset contains details such as transaction amount, user ID, merchant information, timestamps, and more, which were carefully preprocessed and analyzed.

# Objective
- Build a fraud detection system that **minimizes false positives** while **maximizing fraud detection accuracy**.
- Carefully preprocess and analyze the dataset.
- Identify key transactional features that contribute to distinguishing fraudulent behavior.
- Evaluate model performance with **accuracy**, **classification report**, and **confusion matrix**.
- Provide an explanation for misclassifications.

# Data Preprocessing
- Handled missing values (none found in this dataset).
- Label-encoded categorical columns like `merchant`, `category`, and `gender`.
- Scaled numerical features using **StandardScaler**.
- Split the dataset into **training** and **testing** sets.

#  Model Building
- Built two models:  
  - Logistic Regression (baseline)
  - Random Forest Classifier (final best model)
- **Random Forest** with hyperparameter tuning achieved the best results.

# Results
- **Final Model:** Random Forest Classifier
- **Accuracy:** 99.75%
- **Classification Report:**
  - Class 0 (Legitimate Transactions): Precision = 1.00, Recall = 1.00
  - Class 1 (Fraudulent Transactions): Precision = 0.87, Recall = 0.67
  
# Conclusion
- The model is highly accurate at detecting legitimate transactions.
- For fraudulent transactions, while precision is high (fewer false positives), recall is slightly lower, means a few fraudulent transactions are still being missed.
- Misclassifications mainly occur due to the extreme **class imbalance** (very few fraud cases compared to legitimate ones).
- Future work can include any methods to further improve fraud capture rates.
