# Heart Failure Survival Analysis (Kaplan–Meier + Cox) + Risk Modeling

## Overview
This project analyzes a clinical heart failure dataset to:
- estimate survival probability over time using Kaplan–Meier curves
- identify significant risk factors using Cox Proportional Hazards modeling
- build a complementary ML risk model (Logistic Regression / XGBoost) with explainability (SHAP)

**Goal:** Demonstrate healthcare-oriented ML + survival analysis skills applicable to medical device and clinical analytics use cases.

---

## Dataset
- Heart Failure Clinical Records (299 patients, 13 features)
- Target event: `DEATH_EVENT` (renamed to `event`)
- Duration: `time` (renamed to `duration`)

> Note: Raw dataset files are not committed to the repo (see `.gitignore`). Add your own copy under `data/`.

---

## Methods
- **EDA:** distributions, missing values, outcome rate
- **Survival Analysis:**
  - Kaplan–Meier survival curves (overall + stratified)
  - Cox Proportional Hazards model (hazard ratios)
- **ML Risk Model (planned):**
  - Logistic Regression baseline
  - XGBoost classifier
  - Metrics: ROC-AUC, PR-AUC, calibration
  - Explainability: SHAP

---

## Key Findings (update as you finalize)
- Higher **serum_creatinine** and **age** are associated with increased event risk.
- Higher **ejection_fraction** and **serum_sodium** show protective association.

---

## Repo Structure