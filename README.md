# Credit Card Fraud Detection Project 🌐 💳 🚫

## Overview

This project focuses on building a machine-learning model to detect credit card fraud. The dataset used contains anonymized features, including transaction amounts and principal components obtained through dimensionality reduction.

## Objective:

Develop a credit card fraud detection system that compares the effectiveness of various under-sampling and over-sampling techniques when paired with different machine learning algorithms. The primary goals include:

1. **Explore and preprocess the credit card transaction dataset.**
2. **Implement multiple under-sampling and over-sampling techniques to handle class imbalance.**
3. **Experiment with diverse classification algorithms, such as Random Forest, Logistic Regression, and Support Vector Machines.**
4. **Evaluate the models using metrics like accuracy, precision, recall, F1 score, and AUC-ROC.**
5. **Identify the most effective combination of sampling technique and algorithm for optimal fraud detection performance.**

## Deliverables:

- Comparative analysis of under-sampling and over-sampling methods.
- Model performance metrics for each combination of technique and algorithm.
- Recommendations for the most suitable approach for credit card fraud detection based on the experiment results.


## Features

The dataset includes the following features:

- **Time:** Elapsed time since the first transaction (in seconds).
- **V1 to V28:** Anonymized and transformed features resulting from a PCA.
- **Amount:** Transaction amount.
- **Class:** Binary target variable indicating fraudulent (1) or non-fraudulent (0) transactions.

## Methods Used

- Exploratory Data Analysis (EDA) 📊
- Data Preprocessing and Feature Scaling 🔄
- Handling Class Imbalance ⚖️
- Using different Over-sampling and Under-sampling Methods to Handle Imbalanced Data 
- Building and Tuning Machine Learning Models (e.g., Decision Trees, Random Forests) 🛠️
- Evaluation Metrics: Precision, Recall, F1 Score 📏

## Project Approach 

 - ## Approach

### 1. Data Splitting
- Split the dataset into training and testing sets.

### 2. Resampling on Training Set
- Apply resampling techniques (Over Sampling, Under Sampling, or a combination like SMOTE and Tomek Links) exclusively on the training set.
- Techniques like SMOTE generate synthetic instances, while others may undersample the majority class to address the class imbalance.

### 3. Model Training
- Train a machine learning model on the resampled training set.
- For example, use a RandomForestClassifier.

### 4. Validation Set Evaluation
- Evaluate the model on the validation set to monitor its performance during training.
- Calculate and print the F1 score as the primary evaluation metric.

### 6. Test Set Evaluation
- Evaluate the trained model on the original, unmodified test set.
- Calculate and print the F1 score for the test set to assess the model's generalization to unseen data.

By following this approach, we aim to test different resampling methods to handle imbalanced data and compare their effectiveness for the specific problem of credit card fraud detection. The emphasis is on the F1 score as an evaluation metric to balance precision and recall in the classification task. Adjustments can be made based on the requirements and characteristics of the dataset.

