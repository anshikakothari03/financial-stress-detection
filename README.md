# Financial Stress Detection Using Transaction Patterns
Data mining project for detecting financial stress from personal transaction patterns using clustering, anomaly detection, and classification.

## Dataset link 
https://www.kaggle.com/datasets/ramyapintchy/personal-finance-data/data

## Overview

This project explores how personal financial stress can be detected by analyzing patterns in transaction data. The goal is to identify periods where spending behavior becomes irregular or unusual compared to a normal financial routine.

Instead of comparing multiple individuals, the analysis focuses on a single user's transaction history to understand how financial behavior changes over time.

## Dataset

The dataset contains personal transaction records including:

* Date of the transaction
* Transaction description
* Spending category (Food, Rent, Utilities, etc.)
* Amount of money spent or received
* Transaction type (income or expense)

Source: Kaggle – Personal Finance Dataset

## Project Workflow

The analysis follows a complete data mining pipeline:

1. Data collection and understanding
2. Data cleaning and preprocessing
3. Exploratory data analysis (EDA)
4. Feature engineering
5. Frequent pattern mining
6. Clustering
7. Hybrid anomaly detection
8. Classification

## Exploratory Analysis

Initial analysis was performed to understand transaction behavior over time. Visualizations were used to study spending distributions, category-wise spending, and monthly spending trends.

Outlier detection was also applied to identify unusually large transactions.

## Frequent Pattern Mining

Frequent pattern mining techniques such as **Apriori** and **FP-Growth** were applied to discover common spending combinations.

Transaction data was converted into basket-style format and one-hot encoded before mining frequent itemsets and association rules.

## Clustering Analysis

Unsupervised learning techniques were used to group months with similar financial behavior.

Two clustering algorithms were tested:

* K-Means clustering
* DBSCAN

Principal Component Analysis (PCA) was used for visualization and dimensionality reduction.

## Anomaly Detection

To detect unusual financial events, a hybrid anomaly detection system was implemented using:

* Isolation Forest
* One-Class SVM

These models identify transactions that deviate significantly from normal spending patterns.

## Classification

Finally, classification models were trained to predict whether a financial period represents normal behavior or potential financial stress.

Model performance was evaluated using standard classification metrics such as accuracy, precision, recall, and ROC curves.

## Conclusion

The project demonstrates how transaction data can reveal behavioral patterns related to financial stress. By combining pattern mining, clustering, anomaly detection, and classification, it is possible to identify unusual financial behavior and potentially detect early warning signs of financial difficulty.

## Tools and Libraries

Python was used for the analysis with common data science libraries including:

* pandas
* numpy
* scikit-learn
* mlxtend
* matplotlib
* seaborn

## Author

Anshika Kothari
