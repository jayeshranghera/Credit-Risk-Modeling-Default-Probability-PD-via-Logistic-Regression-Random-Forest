# Credit Risk Modeling — Default Probability (PD) via Logistic Regression & Random Forest

This project is part of the **JPMorgan Chase & Co. Virtual Job Simulation (Forage Platform)**.  
All code and analysis are written by me based on the tasks provided in the simulation.


## Overview
Builds and compares baseline classifiers (Logistic Regression, Random Forest) to predict loan default (PD). Includes train/test split, metrics (accuracy, confusion matrix, ROC AUC), and model comparison.

## Data
- Example columns include: `default` (0/1), `fico_score`, and other borrower/loan features if available.
- Replace with your dataset path or add instructions in `data/README.md`.

## Methods
- Train/test split
- Feature preprocessing (scaling/selection if used)
- Models: Logistic Regression, Random Forest
- Evaluation: Accuracy, Confusion Matrix, ROC AUC

## Results
- Side-by-side metrics for both models
- ROC AUC to assess ranking quality

## Notes & Limitations
- Imbalanced classes may distort accuracy; prefer ROC AUC, PR AUC, calibration.
- No hyperparameter tuning in the baseline; add Grid/Random/Bayesian search for improvement.

## What make this better...
- Add cross-validation and calibration plots
- Threshold tuning for business objective (minimize expected loss)
- Save trained model (`.pkl`) and provide a scoring function/CLI
