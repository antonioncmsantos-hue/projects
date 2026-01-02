# RMBA Assignment — Debt Drivers & Creditworthiness (Group B9)

**Goal:** Explain household debt drivers and test whether income differs by creditworthiness (L1 vs L2) using the Loan Default dataset.  
**Deliverable:** `RMBA_Group_B9.ipynb`

## Highlights
- Built a reproducible cleaning pipeline and created the target variable: **debt = (dtir1/100) * income**
- **OLS Regression (Debt ~ Income + controls)** with diagnostics and robust standard errors
- **Two-sample t-test (Welch)** comparing income between **L1 vs L2**, including assumption checks and effect size

## Methods
- **Method 1:** OLS (baseline + expanded model with loan/borrower controls and categorical effects)
- **Diagnostics:** heteroskedasticity test, residual checks, VIF, robust SE (HC3)
- **Method 2:** Welch t-test (income by creditworthiness), normality/variance checks, effect size (Hedges’ g)

## Dataset
This project uses the **Loan Default Dataset** from Kaggle (author: *yasserh*):  
- Source: https://www.kaggle.com/datasets/yasserh/loan-default-dataset/data

**Local path expected:** after downloading and extracting, place the CSV here:  
- `data/Loan_Default.csv`

## Files
- `RMBA_Group_B9.ipynb` — main analysis
- Dataset: https://www.kaggle.com/code/zoezoe123/loan-default — download from Kaggle (link above)
- `RMBA_GroupAssignment_GradingCriteria.pdf` — assignment requirements

## How to run (local)
1. Download the dataset from Kaggle and place it in:
   - `data/Loan_Default.csv`
2. Install dependencies and start Jupyter:
   ```bash
   pip install -r requirements.txt
   jupyter notebook RMBA_Group_B9.ipynb
