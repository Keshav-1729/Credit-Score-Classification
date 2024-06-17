# Credit Score Classification Model

This repository contains the implementation of a machine learning project aimed at classifying credit scores. The project involves data cleaning, feature selection, handling class imbalance, model training, and evaluation using various classification algorithms.

## Table of Contents

- [Project Description](#project-description)
- [Business Use Case](#business-use-case)
- [Data Preprocessing](#data-preprocessing)
  - [Data Cleaning](#data-cleaning)
  - [Feature Selection](#feature-selection)
- [Handling Class Imbalance](#handling-class-imbalance)
  - [Sampling Techniques](#sampling-techniques)
- [Model Training](#model-training)
  - [Experimentation](#experimentation)
  - [Best Model](#best-model)

## Project Description

This project aims to develop a credit score classification model to help financial institutions assess the creditworthiness of individuals. The model classifies credit scores into different categories, enabling better decision-making for loan approvals, credit limits, and interest rates.

## Business Use Case

Credit scoring is a critical process in the financial industry. It helps lenders evaluate the risk associated with lending money to potential borrowers. A reliable credit score classification model can:
- Reduce the risk of default by identifying high-risk borrowers.
- Enable personalized credit offerings based on an individual's credit score.
- Improve the efficiency of the credit approval process.
- Enhance customer satisfaction by providing faster and fairer credit decisions.

## Data Preprocessing

### Data Cleaning

Data cleaning was performed to ensure the dataset was free from inconsistencies, missing values, and irrelevant information. This step is crucial for maintaining the quality and accuracy of the model.

### Feature Selection

Feature selection was carried out using:
- **Mutual Information**: Measures the dependency between features and the target variable.
- **Multivariate Analysis**: Examines relationships between multiple features to select the most significant ones.

## Handling Class Imbalance

### Sampling Techniques

To address the issue of class imbalance in the dataset, the following techniques were employed:
- **SMOTE (Synthetic Minority Over-sampling Technique)**: Generates synthetic samples for the minority class to balance the dataset.
- **SMOTE + ENN (Edited Nearest Neighbors)**: Combines SMOTE with ENN to remove noisy samples and refine the dataset.
- **SMOTE + Tomek Links**: Combines SMOTE with Tomek Links to eliminate overlapping samples from different classes and enhance class separation.

## Model Training

### Experimentation

Various classification models were experimented with, including:
- **Logistic Regression**: A statistical model that uses a logistic function to model a binary dependent variable.
- **Decision Trees**: A non-parametric model that predicts the value of a target variable by learning simple decision rules from data features.
- **Random Forest**: An ensemble learning method that uses multiple decision trees to improve classification accuracy.
- **Support Vector Machines (SVM)**: A supervised learning model that finds the hyperplane that best separates different classes in the feature space.
- **Boosting Algorithms**: Ensemble methods like XGBoost and AdaBoost that combine weak classifiers to create a strong classifier.

### Best Model

After extensive experimentation, Random Forest was found to be the best-performing model. It outperformed even the boosting algorithms in terms of accuracy and other evaluation metrics.
