# Credit Card Fraud Detection Project 🌐 💳 🚫

## Overview

This project focuses on building a machine-learning model to detect credit card fraud. The dataset used contains anonymized features, including transaction amounts and principal components obtained through dimensionality reduction.

### Motivation

Credit card fraud is a prevalent issue, and effective fraud detection is crucial to mitigate financial losses. This project aims to explore and implement methods for identifying fraudulent transactions using machine learning techniques.

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

### 2. Further Splitting for Validation
- Further split the training set into training and validation sets.

### 3. Resampling on Training Set
- Apply resampling techniques (Over Sampling, Under Sampling, or a combination like SMOTE and Tomek Links) exclusively on the training set.
- Techniques like SMOTE generate synthetic instances, while others may undersample the majority class to address the class imbalance.

### 4. Model Training
- Train a machine learning model on the resampled training set.
- For example, use a RandomForestClassifier.

### 5. Validation Set Evaluation
- Evaluate the model on the validation set to monitor its performance during training.
- Calculate and print the F1 score as the primary evaluation metric.

### 6. Test Set Evaluation
- Evaluate the trained model on the original, unmodified test set.
- Calculate and print the F1 score for the test set to assess the model's generalization to unseen data.

By following this approach, we aim to test different resampling methods to handle imbalanced data and compare their effectiveness for the specific problem of credit card fraud detection. The emphasis is on the F1 score as an evaluation metric to balance precision and recall in the classification task. Adjustments can be made based on the requirements and characteristics of the dataset.

