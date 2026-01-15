# Credit Risk — Debt Burden Modeling (OLS) | Loan Default Dataset


## Overview
This project models **debt burden** using borrower income and loan characteristics to support **credit-risk understanding** (affordability / borrower profiling) with an interpretable, diagnostics-driven approach.

## Quick links
- **Report (ipynb):** [Open](https://github.com/antonioncmsantos-hue/projects/blob/main/credit-risk-loan-default/notebooks/RMBA_Group_B9.ipynb)
- **Dataset:** [Open](https://github.com/antonioncmsantos-hue/projects/tree/main/credit-risk-loan-default/data)

## Problem
**How strongly is borrower income associated with debt burden, and do loan/product characteristics improve explanatory power?**  
Business context: lenders evaluate affordability and risk by understanding how debt levels move with borrower capacity and loan conditions.

## Data
- **Source:** [Loan Default dataset (CSV)](https://www.kaggle.com/datasets/yasserh/loan-default-dataset/data)
- **Scope:** Individual loan applications (cross-sectional)
- **Key variables**
  - Borrower: `income`
  - Debt burden: `dtir1` (DTI ratio), `debt` (derived)
  - Loan terms: `loan_amount`, `rate_of_interest`, `interest_rate_spread`, `term`, `status`
  - Categorical: `loan_type`, `loan_purpose`, `occupancy_type`

## Method
1. **Data preparation:** missing values, outliers, encoding of categorical variables
2. **Baseline OLS:** `debt ~ income`
3. **Extended OLS:** add loan terms + borrower/loan characteristics
4. **Diagnostics:** heteroscedasticity, residual normality, multicollinearity (VIF)
5. **Robustness:** robust SE and log specifications (where appropriate)

## Results (Key Findings)
- Income shows a **strong positive association** with debt burden (baseline explains a large share of variation).
- Adding loan characteristics **improves fit** and reveals additional drivers (e.g., loan amount and rate-related variables).
- Diagnostics indicate **heteroscedasticity** and non-normal residuals; robustness checks help validate conclusions.

## Outputs
- **Report (HTML):** `reports/RMBA_Group_B9.html`
- **Notebook:** `notebooks/RMBA_Group_B9.ipynb`
- **Data:** `data/Loan_Default.csv`
- **Preview image:** `assets/preview.png`

## Repo structure
- `data/` — dataset(s)
- `notebooks/` — analysis notebook(s)
- `reports/` — HTML/PDF outputs
- `assets/` — screenshots for previews

## Notes & limitations
- `debt` is derived from `income` and `dtir1`, so a strong baseline relationship is expected **by construction**.
- This project prioritizes **interpretability** (OLS + diagnostics), not default classification.
- Next steps (if you want “credit scoring”): add **logit/XGBoost** default prediction + **ROC/AUC** + feature importance.

