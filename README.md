# AI-Churn-Prediction-Model

Telecom Churn Prediction System

Project Overview

This repository contains the source code for the "AI-Driven Retention" project. The goal of this system is to predict customer churn in the premium subscriber segment of a telecommunications company. By identifying at-risk customers with a 30-day intervention window, the business aims to reduce premium churn by 10% and recover estimated annual revenues of $500,000.

Methodology

The solution utilizes a Machine Learning pipeline designed for high recall (minimizing false negatives).

Data Preprocessing: Cleaning, One-Hot Encoding for categorical variables, and Standardization for numerical variables.

Feature Engineering: Creation of Usage_Trend to detect drops in subscriber activity.

Handling Imbalance: Implementation of SMOTE (Synthetic Minority Over-sampling Technique) to address the 15% churn rate class imbalance.

Modeling: Comparison of Logistic Regression, Random Forest, and XGBoost.

Selection: XGBoost was selected as the champion model due to superior performance in Recall and AUC-ROC metrics.

Installation & Usage

Prerequisites

Python 3.8+

Pip package manager

Setup

Clone the repository:

git clone [https://github.com/yourusername/telecom-churn-prediction.git](https://github.com/yourusername/telecom-churn-prediction.git)


Install dependencies:

pip install -r requirements.txt


Running the Analysis

Execute the main script to generate synthetic data, train the models, and view performance metrics:

python churn_model.py


Results Summary

Selected Model: XGBoost Classifier

Primary Metric: Recall (Sensitivity) - Optimized to ensure at-risk customers are not missed.

Key Drivers: Contract Type (Month-to-month), Customer Service Interaction Frequency, and Monthly Charge Volatility.

Author

Tyler O'Keefe
Artificial Intelligence & Business Analytics Course
