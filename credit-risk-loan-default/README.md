# RMBA Assignment — Debt Drivers & Creditworthiness (Group B9)

**Goal:** Explain household debt drivers and test whether income differs by creditworthiness (L1 vs L2) using the Loan Default dataset.  
**Main notebook:** `notebooks/RMBA_Group_B9.ipynb`

## Highlights
- Built a reproducible cleaning pipeline and created the target variable: **debt = (dtir1/100) * income**
- **OLS Regression (Debt ~ Income + controls)** with diagnostics and robust standard errors (HC3)
- **Welch two-sample t-test** comparing income between **L1 vs L2**, including assumption checks and effect size (Hedges’ g)

## Results (summary)
- Income is a strong predictor of debt in the baseline model and remains significant after adding controls.
- Model diagnostics indicate heteroskedasticity; robust standard errors are used to support inference.
- Income differs between creditworthiness groups (L1 vs L2), but the practical effect is small.

## Dataset
This project uses the **Loan Default Dataset** (Kaggle, author: *yasserh*):  
https://www.kaggle.com/datasets/yasserh/loan-default-dataset/data

The dataset is **not included** in this repository.  
See `data/README.md` for download instructions and the expected local path.

## Project structure
