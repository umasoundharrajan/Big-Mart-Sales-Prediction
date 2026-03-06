# Big Mart Sales Prediction

## Project Overview
This project predicts the sales of products across various Big Mart outlets using 2013 historical data. The goal is to identify properties of products and stores that play a key role in increasing sales.

## Approach
**Data Cleaning:** Handled missing values for `Item_Weight` and `Outlet_Size`. Imputed `Item_Visibility` zeros as missing data.
**Feature Engineering:** * Created `Outlet_Years` to measure store maturity.
  * Extracted `Item_Type_Combined` from Product IDs.
  * Corrected `Item_Fat_Content` for non-consumable items.
**Model:** XGBoost Regressor with 5-Fold Cross-Validation.
**Performance:** Achieved an Average RMSE of **1120**

## How to Run
1. Ensure `pandas`, `numpy`, `xgboost`, and `scikit-learn` are installed.
2. Keep the train and test CSVs in the same folder as the script.
3. Run the notebook/script to generate `final_submission.csv`.
