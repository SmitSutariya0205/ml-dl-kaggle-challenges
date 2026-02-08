# Playground Series S6E2 – Predicting Heart Disease

This project contains my solution for the Kaggle Playground Series Season 6 Episode 2 competition, focused on predicting the presence of heart disease using tabular medical data.

## Problem
Binary classification task to predict whether a patient has heart disease.  
Evaluation metric: **ROC-AUC**.

## Approach
- Performed feature engineering to capture medical risk interactions
- Used a stratified train/validation split for fair evaluation
- Trained and tuned tree-based models:
  - **LightGBM**
  - **CatBoost**
- Applied early stopping and cross-validation–guided hyperparameter tuning
- Final predictions generated using an **ensemble of LightGBM and CatBoost**

## Models Used
- LightGBM (GBDT, tuned)
- CatBoost (tuned using RandomizedSearchCV)

## Key Techniques
- Feature engineering
- Hyperparameter tuning
- Early stopping
- Model ensembling

## Files
- `lgbm_catboost_ensemble.ipynb` — Full training, tuning, and submission pipeline

## Notes
This notebook is designed to be run directly on Kaggle without external dependencies or data downloads.
