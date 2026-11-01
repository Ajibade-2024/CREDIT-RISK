Credit Risk Prediction System

> Predict loan default probability using Machine Learning to help financial institutions make smarter lending decisions.
📌 Problem Statement:
Banks lose billions annually to loan defaults. This project builds a predictive model that assesses a borrower's creditworthiness *before* a loan is approved, reducing risk and improving portfolio health.

We answer: Will this customer default?

📊 Dataset
Source: `LendingClub / Kaggle Credit Risk Dataset`
- 32,000+ loan records
- Features: Loan amount, interest rate, annual income, employment length, credit history, debt-to-income ratio, etc.
- Target: `default` (0 = Non-defaulter, 1 = Defaulter)

- 🧠 Methodology

1. Data Cleaning & EDA
- Handled missing values, outliers, skewed distributions
- Analyzed correlation between Income, Employment length, Age, Amount and credit lenght

2. Feature Engineering
- Encoded categorical variables (employment, home ownership, Intent(loan purpose))
- RANDOM OVER SAMPLING AND RANDOM UNDER SAMPLING to address class imbalance

3. Models Tested

|Model                    | Accuracy |  Precision  | Recall  | F1-Score | ROC-AUC |
|-------------------------|--------- |-------------|--------|-----------|---------|
|Decision Tree Classifier | 0.82     |   0.49       |0.80   |    0.61    |    0.81|
|Random Forest              | 0.80    |    0.47      | 0.95  |     0.63    |    0.88|
|XGBoost   **(Best)**     | **0.80**   | **0.48**  | **0.97**  | **0.64**   | **0.89**|

4. Model Explainability
- Top drivers: Interest Rate, Status, Annual Income, Amount    

🛠️ Tech Stack
- *Language:* Python
- *Libraries:* Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Imbalanced-learn, 
