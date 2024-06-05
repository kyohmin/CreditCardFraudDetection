# [Meta Code M] - Credit Card Fraud Detection Project

## Table of Contents

1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Models](#models)
5. [Evaluation](#evaluation)
6. [Conclusion](#conclusion)
7. [References](#references)

## Overview
Meta Code M is an education platform focused on AI and IT in South Korea. Enrolled in "Credit Card Fraud Detection Project - Cohort 8" to...
- Learn the basics of ML and data analysis.
- Learn how to effectively approach and analyze data.
- Get practical help from professionals.
- Make a small project for portfolio.

## Dataset
The dataset used in this project is the [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) from Kaggle. It contains transactions made by credit cards by European cardholders in September 2013. The dataset contains 31 columns with 28 PCA-transformed features. It has 284,807 transactions, but only 492 of them are frauds, showing a highly imbalanced rate of 0.00173.

## Installation
```bash
git clone https://github.com/kyohmin/CreditCardFraudDetection
.git
cd CreditCardFraudDetection
```

## Models
- Deep Neural Network (16,16,8,8,1)
- Weighted Deep Neural Network (16,16,8,8,1)
- XGBoost
- Logistic Regression
- Support Vector Machine Classifier
- **Ensemble Voting Model (Deep NN, XGBoost, SVC)**

  
## Evaluation
- Binary Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC Curve

## Conclusion
Through the evaluation of six different models, I have found out that the "suitable" model depends on the criteria and purpose of the project, meaning that the best model can vary according to perspectives. In this project, I set the F1 score as the primary evaluation metric. Among neural networks, weighted neural networks, XGboost, logistic regression, support vector machines, and ensemble voting models, XGBoost and ensemble voting models showed the best performance. Considering the computation cost and insignificant increase in performance, I believe that XGBoost is the best-performing model for detecting fraud in credit card transactions. Below are the evaluation scores of the XGBoost model.

![download](https://github.com/kyohmin/CreditCardFraudDetection/assets/71572502/67e803b2-891d-4874-a0da-6784c0cbb1b7)

<img src="https://github.com/kyohmin/CreditCardFraudDetection/assets/71572502/3eccf879-43c5-4f77-b74f-74bb2ee2b44e" alt="drawing" width="400"/>

## References
1. Greg Hogg, Credit Card Fraud Detection - Dealing with Imbalanced Datasets in Machine Learning [https://www.youtube.com/watch?v=M_Cu7r9gik4]
2. TensorFlow, Classification on imbalanced data [https://www.tensorflow.org/tutorials/structured_data/imbalanced_data]
3. Geron Aurelien, Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition
