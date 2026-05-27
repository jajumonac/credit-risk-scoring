# Credit Risk Scoring Model

A predictive model that estimates the probability of loan default using applicant financial and demographic data. Built for lenders and financial institutions that need to make faster, more consistent credit decisions.

## Business Problem

Lenders face a core trade-off: approving too many risky applicants increases default losses, while being too conservative leaves revenue on the table. This model gives loan officers a data-driven probability of default for each applicant — turning a subjective decision into a measurable, auditable one.

## What This Model Does

- Predicts the probability that a loan applicant will default
- Ranks applicants by risk level so lenders can set approval thresholds
- Identifies the features that drive default risk most strongly (interpretable output)

## Dataset

[German Credit Dataset](https://www.openml.org/d/31) — 1,000 loan applicants with 20 features (credit history, loan amount, employment status, etc.) and a binary default label. A classic benchmark dataset used in credit risk research.

## Approach

1. **Exploratory Data Analysis** — understand the data, identify class imbalance, spot key risk signals
2. **Feature Engineering** — encode categoricals, handle missing values, create derived features
3. **Baseline Model** — Logistic Regression (interpretable, auditable, industry standard)
4. **Improved Model** — XGBoost (higher accuracy, captures nonlinear interactions)
5. **Business Evaluation** — not just accuracy, but: at a given approval threshold, what is the expected default rate and what revenue does the lender capture?

## Key Results

*(To be updated as model is built)*

## Stack

- Python 3.x
- pandas, numpy, scikit-learn, xgboost
- matplotlib, seaborn
- Jupyter Notebook

## Author

Jadiel Montero — Freelance Data Scientist specializing in predictive models for financial businesses.
[LinkedIn](#) | [Upwork](#)
