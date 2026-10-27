# TP01 — Choosing and Interpreting the Right Chart, then Learning from Data to Make Decisions

**Module:** 05 AI Engineer — Faculty of Sciences
**Supervisor:** Prof. DRIF Ahlem
**Student:** <your name>

## Objective
Explore the Pima Indians Diabetes dataset with the appropriate visualisations, prepare the data, then train and compare tree-based classifiers to predict whether a patient is diabetic.

## Dataset
[Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database): 768 patients, 8 diagnostic attributes (Glucose, BMI, Age, Insulin, ...) and a binary target `Outcome` (1 = diabetic).

## Contents
| File | Description |
|---|---|
| `TP01_Diabetes_<YourName>.ipynb` | Jupyter notebook: code, charts and written answers |
| `TP01_Diabetes_<YourName>.pdf` | PDF export of the notebook |
| `TP01.pdf` | Lab subject |
| `diabetes.csv` | Dataset |

## Work done
1. **Understanding the data:** attribute description; detection of impossible zeros (missing values).
2. **Missing values:** visualisation, then two imputations (median/mode and KNN).
3. **Exploration:** histograms, box plots, violin plots, density plots, scatter plots, correlation heatmap, pair plot, faceting, and a chart critique.
4. **Models:** decision tree (Gini/entropy, decision boundaries, pruning), Bagging, XGBoost.
5. **Evaluation:** confusion matrices, accuracy, precision, recall, F1, ROC/AUC, and the effect of the imputation method.

## Main results
- Glucose is the strongest predictor, followed by BMI and Age.
- KNN imputation preserves the distributions better than median imputation.
- A single decision tree overfits beyond depth 4.
- XGBoost gives the best and most stable AUC (≈ 0.83).

## How to run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost ipywidgets
```
Open the notebook with `diabetes.csv` in the same folder, then **Run All**.