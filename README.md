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

| Metric | Logistic Regression | XGBoost |
|--------|---------------------|---------|
| ROC-AUC | 0.801 | 0.798 |
| Recall — No Default | 0.86 | 0.90 |
| Recall — Default | 0.58 | 0.45 |

**Logistic Regression is the recommended model.** Despite XGBoost's slightly higher approval rate, it only catches 45% of actual defaulters vs Logistic Regression's 58% — a meaningful gap in a domain where missed defaults translate directly to financial loss. Logistic Regression also wins on ROC-AUC and provides the coefficient-level explainability required by financial regulators (Basel III, ECOA).

## Stack

- Python 3.x
- pandas, numpy, scikit-learn, xgboost
- matplotlib, seaborn
- Jupyter Notebook

## Author

Jadiel Montero — Freelance Data Scientist specializing in predictive models for financial businesses.
[LinkedIn](https://www.linkedin.com/in/jadiel-montero-230814142/) | [Upwork](https://www.upwork.com/freelancers/~01d2e510be92ca3e00?mp_source=share)
