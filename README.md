# Predict-Loan-Payback
In the context of banking risk management, to estimate the probability that a borrower will repay a loan.

Objective: To predict the probability of a borrower paying back their loan using machine learning techniques, focusing on financial risk assessment.

Dataset: Kaggle Playground Series - Loan Payback Prediction (Over 600K records).

Metric: Model performance is evaluated using the ROC AUC score.

**📈 Final Results**
ROC AUC Score:

Initial Baseline (LGBM Default): ~0.9192,
Final Model (LGBM + Optuna): 0.9221 Achieved increase through Bayesian hyperparameter optimization.

**🛠️ Methodology and Workflow**

This project utilized a robust Scikit-learn pipeline focusing on efficiency and data integrity:

Preprocessing & Data Integrity: A custom ColumnTransformer and Pipeline were used to prevent data leakage. Numerical data was Scaled, and categorical data was One-Hot Encoded.

Exploratory Data Analysis (EDA): Identified key features like the debt-to-income ratio (strongest correlation) and credit score, and confirmed the dataset's imbalance (80% vs 20% target split).

Model Optimization: The LightGBM (LGBM) model was selected for its speed on large datasets. Optimal hyperparameters were systematically found using Optuna's Bayesian Optimization.


