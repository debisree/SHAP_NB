# SHAP Tutorial: Interpreting a Boston Housing Regression Model

This repository contains a hands-on lab for **SHAP (SHapley Additive exPlanations)** using the classic **Boston Housing** dataset. The goal is to demonstrate how to interpret a tree-based regression model at both global and local levels using Shapley-value-based explanations.

## Contents

- `Boston_SHAP_Lab_Colab.ipynb`  
  Colab-friendly notebook that:
  - Loads the Boston Housing data from `HousingData.csv` or a GitHub URL.
  - Trains a `RandomForestRegressor` to predict `MEDV` (median home value).
  - Uses **SHAP** to compute feature-level contributions for each prediction.
  - Generates and interprets:
    - SHAP summary (beeswarm) plot
    - SHAP bar plot (mean |SHAP|)
    - SHAP dependence plot (e.g., for `LSTAT`)
    - SHAP waterfall plot (single prediction)
    - SHAP decision plot (multiple predictions)
  - Computes a quantitative feature ranking based on mean absolute SHAP values.
  - Discusses common pitfalls and best practices when using SHAP.

- `HousingData.csv`  
  Boston Housing dataset with `MEDV` as the target column.

## Running the Notebook in Colab

1. Open the notebook in Colab using the badge below (update the URL to match this repository):

   ```markdown
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/<USER>/<REPO>/blob/main/Boston_SHAP_Lab_Colab.ipynb)
