# Credit-Card-Fraud-Detection

## Dataset Information

Credit card fraud detection is crucial for ensuring customers are not charged for unauthorized transactions. The dataset contains transactions made by credit cards in September 2013 by European cardholders. Out of 284,807 transactions, there are 492 frauds, making the dataset highly imbalanced with frauds accounting for 0.172% of all transactions.

The dataset includes numerical input variables resulting from a PCA transformation. Features V1, V2, … V28 are principal components from PCA, while 'Time' and 'Amount' remain as non-transformed features. 'Time' indicates seconds elapsed since the first transaction, and 'Amount' denotes the transaction amount. The response variable 'Class' takes the value 1 in cases of fraud and 0 otherwise.

Given the class imbalance, accuracy should be measured using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

**Download the dataset:** [Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)

## Libraries

- pandas
- matplotlib
- seaborn
- scikit-learn

## Algorithms

- Logistic Regression
- Random Forest
- XGBoost

## Project Overview

This repository contains scripts and notebooks for building and evaluating machine learning models to detect credit card fraud. Below is a summary of the project's steps:

### 1. Data Loading and Preprocessing

- Loaded the dataset using `pandas`.
- Checked for and handled any missing values.
- Standardized numerical features using `StandardScaler`.
- Conducted exploratory data analysis (EDA) to understand the distribution of features.

### 2. Exploratory Data Analysis (EDA)

- Visualized the distribution of features using `seaborn` and `matplotlib`.
- Plotted histograms and density plots for each numerical feature.
- Created a correlation matrix heatmap to explore feature correlations.

### 3. Model Training and Evaluation

- Split the data into training and testing sets.
- Trained several classifiers including Logistic Regression, Random Forest, and XGBoost.
- Evaluated models using metrics such as precision, recall, F1-score, and AUPRC.
- Addressed class imbalance using Synthetic Minority Over-sampling Technique (SMOTE).

### 4. Results

- Reported performance metrics for each model.
- Highlighted the importance of handling class imbalance and measuring performance with appropriate metrics.

**Best Model F1 Score:** 87.00

## Conclusion

This project demonstrates the application of machine learning techniques to detect fraud in credit card transactions, emphasizing the importance of handling imbalanced data and using appropriate evaluation metrics.
