Credit Card Fraud Detection
This repository contains an end-to-end Credit Card Fraud Detection System built using Machine Learning techniques.
The project demonstrates how ML-based models can significantly outperform traditional rule-based fraud detection systems by adapting to evolving fraud patterns and analyzing transaction behavior intelligently. 

Dataset Source
The dataset used in this project is publicly available on Kaggle:
🔗 Credit Card Fraud Detection Dataset
https://www.kaggle.com/datasets/kartik2112/fraud-detection
This dataset includes PCA-transformed anonymized features (V1–V28), Amount, and Time, making it ideal for experimentation while preserving privacy.

Project Overview
Credit card fraud detection is a critical challenge due to:
Increasing digital payment usage
Highly imbalanced datasets (fraud < 1%)
Evolving fraud patterns that bypass static rule-based systems
This project builds a machine-learning-based pipeline capable of detecting fraudulent transactions with high accuracy using:
Data preprocessing
Exploratory data analysis (EDA)
Feature engineering
Imbalanced data handling (SMOTE + undersampling)
Multiple ML models (Logistic Regression, Random Forest, XGBoost)
SHAP explainability

System Architecture
1. Data Preprocessing
Handling missing values
Outlier detection
Encoding categorical features
Standardization of numerical features
PCA-based feature utilization
Feature engineering (velocity features, spending deviations, etc.)
2. Handling Imbalanced Data
SMOTE (Synthetic Oversampling)
Random undersampling
These improve the model’s ability to identify minority fraud cases.
3. Model Training
Models trained & compared:
Logistic Regression
Random Forest
XGBoost
Performance evaluated via:
Accuracy
Precision
Recall (most important in fraud detection)
F1-score
ROC-AUC
4. Explainability Layer
Using SHAP, analysts can interpret:
Why a transaction was flagged
Which features contributed most
Feature behavior patterns
5. Output Layer
Fraud likelihood predictions
Confusion matrix & ROC-AUC
SHAP plots (summary, force plots)
Transaction-level explanations

Implementation
Language: Python
Libraries:
pandas, numpy, scikit-learn, xgboost, shap, matplotlib, seaborn, plotly
Environment: Jupyter Notebook / Google Colab

Results & Insights
Random Forest and XGBoost delivered the highest performance.
Achieved 99%+ accuracy and high recall, critical for minimizing missed fraud cases.
SMOTE significantly improved fraud detection by balancing the dataset.
SHAP revealed that:
PCA components contribute heavily to model decisions.
Unusual transaction amounts and irregular timings are key fraud indicators.
The system is robust, explainable, and suitable for real-time deployment with continuous retraining.

Challenges
Extreme class imbalance
Evolving fraud patterns (concept drift)
Balancing recall vs. false positives
Need for continuous model updates

Recommendations for Future Work
Add more behavior-based features
Dynamic threshold tuning
Real-time streaming pipeline
Deep learning models (Autoencoders, LSTM, Transformers)
Continuous retraining to reduce concept drift
Human-in-the-loop review for high-risk cases

References
A detailed explanation of the system, methodology, theory, and results is available in the attached project report. 


