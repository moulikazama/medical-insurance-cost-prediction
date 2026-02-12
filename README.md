**Medical Insurance Cost Prediction**



**Project Overview**



This project predicts medical insurance charges based on demographic and

lifestyle features. The objective is to identify key cost-driving

factors and build regression models for accurate prediction.



**Dataset**



Source: Kaggle - Medical Insurance Dataset



**Features:**

\- Numerical: Age, BMI, Children

\- Categorical: Sex, Smoker, Region

\- Target: Insurance Charges



**Exploratory Data Analysis (EDA)**



\-   Charges are right-skewed

\-   Outliers present in target variable

\-   Smoking has the strongest impact on charges

\-   BMI and Age positively correlate with insurance cost

\-   Log transformation applied to reduce skewness



**Data Preprocessing**



\-   One-hot encoding for categorical variables

\-   Log transformation applied to target

\-   Train-test split performed



**Models Implemented**



\-   Linear Regression

\-   Ridge Regression (L2 Regularization)

\-   Random Forest Regressor

\-   Hyperparameter tuning using GridSearchCV



**Evaluation Metrics**



\-   R² Score

\-   RMSE (Root Mean Squared Error)



**Model Performance Summary**



RF (Tuned + Log) R²: 0.8796 RMSE: 4323

RF (Log) R²: 0.8769 RMSE: 4370

RF R²: 0.8644 RMSE: 4586

Linear R²: 0.7835 RMSE: 5796

Ridge R²: 0.7835RMSE: 5796



**Best Model**



Random Forest (Tuned + Log Transformation)



**Key Insights**



\-   Smoking is the most influential factor.

\-   BMI and Age significantly impact costs.

\-   Random Forest captures non-linear relationships better than linear models.

\-   Log transformation improved performance.



**Project Structure**



medical-insurance-cost-prediction/

│

├── data/

│   └── insurance.csv

│

├── notebooks/

│   ├── 01\_data\_preprocessing.ipynb

│   ├── 02\_eda.ipynb

│   ├── 03\_base\_model\_building.ipynb

│   ├── 04\_improve\_model.ipynb

│

├── results/

│   └── model\_comparison\_results.csv

│

├── README.md

└── requirements.txt



**Conclusion**



This project demonstrates end-to-end regression modeling, preprocessing,

hyperparameter tuning, and evaluation to build a reliable medical

insurance cost prediction system.



