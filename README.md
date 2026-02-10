# Medical Insurance Cost Prediction

## Problem Statement

Predict medical insurance charges based on customer demographic and lifestyle data to support pricing and risk assessment.

## Dataset

Public medical insurance dataset from Kaggle.

## Features

**•**   Numerical: Age, BMI, Children

**•**   Categorical: Sex, Smoking Status, Region

**•**   Target Variable: Insurance Charges

## Approach

•   Data cleaning and preprocessing

•   One-hot encoding for categorical variables

•   Exploratory Data Analysis (EDA)

•   Outlier detection and skewness analysis

•   Log transformation applied to target variable to handle right skewness

•   Feature relevance analysis using correlation and domain insights

•   Regression modeling:

 	•  Linear Regression (baseline)

 	•  Ridge Regression (regularization)

 	•  Random Forest Regressor (non-linear modeling)

## Model Evaluation Metrics

**•   R² Score** – to measure goodness of fit

**•   RMSE** – to measure average prediction error magnitude

## Key Insights 

•   Smoking status is the most influential factor driving insurance charges.

•   BMI and age show strong positive relationships with medical costs.

•   Insurance charges are highly right-skewed, and log transformation improves model stability.

•   Random Forest captures non-linear relationships better than linear models.

•   Log-transformed target improves performance for linear and ridge regression.

## Current Status

✔ Data preprocessing completed

✔ Exploratory Data Analysis completed

✔ Feature engineering \& log transformation completed

🔄 Model building and comparison (normal vs log target) in progress

🔄 Hyperparameter tuning in progress











