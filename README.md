# Diabetes Progression Prediction using Machine Learning

This repository contains a comparative analysis of Machine Learning regression models used to predict disease progression in diabetes patients, based on clinical metrics. This project was developed as part of the Machine Learning course at the University of Macedonia.

## Models Evaluated
* **Random Forest Regressor**
* **Gaussian Process Regressor (GPR)**
* **Support Vector Regression (SVR)**
* **K-Nearest Neighbors (KNN)**

## Key Features
* Implementation of **6-Fold Cross Validation** for robust evaluation.
* Hyperparameter tuning using `RandomizedSearchCV`.
* Extensive evaluation using metrics: **RMSE, MAE, Max Error, and MAPE**.
* Model interpretability and feature importance analysis using **SHAP (Summary and Waterfall plots)**.

## Files in this Repository
* `diabetes_regression_models.ipynb`: The Google Colab notebook containing all the Python code, training loops, and visualizations.
* `diabetes_regression_models.py`: The standalone Python script version of the analysis, suitable for production environments.
* `regression_results.csv`: The exported evaluation metrics for all models across all folds.
* `Report.pdf`: The comprehensive final report (in Greek) detailing the methodology, comparative analysis, and clinical relevance of the findings.

## Conclusion
The **Gaussian Process Regressor** yielded the most stable and reliable predictions (RMSE ~55), successfully avoiding the severe overfitting observed in the KNN model. SHAP analysis confirmed that BMI and the s5 serum marker were the most critical features in driving model predictions.
