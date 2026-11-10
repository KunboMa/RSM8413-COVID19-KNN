# RSM8413 — COVID-19 KNN Classification


Machine Learning Analytics — Group Assignment 1

## Project Objective

Predict whether individuals received two doses of a COVID-19 vaccine using demographic, employment, household, and well-being characteristics.

## Data

- Original observations: 6,430
- Baseline predictors: 7
- Target: `vac_binary`
  - 1 = Two doses
  - 0 = Fewer than two doses

## Files

- `Data_Prep&EDA.ipynb`: Data cleaning, preprocessing, and exploratory data analysis.
- `covid_cleaned_baseline.csv`: Cleaned baseline dataset before encoding and scaling.

## Modeling Notes

- Train/test split: 80/20, stratified
- Random state: 42
- One-hot encoding for categorical predictors
- Z-score standardization for numerical predictors
- Preprocessing should be fitted separately within each cross-validation training fold to prevent data leakage.

## Next Steps

KNN modeling, hyperparameter tuning using cross-validation, and final model evaluation.
