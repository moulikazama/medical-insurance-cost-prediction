🏥 Medical Insurance Cost Prediction

📌 Project Overview



This project aims to predict medical insurance charges based on customer demographic and lifestyle features. The objective is to identify the most influential factors affecting insurance costs and build regression models to support pricing and risk assessment decisions.



📂 Dataset



Public Medical Insurance Dataset sourced from Kaggle.



Features:



Numerical: Age, BMI, Children



Categorical: Sex, Smoker, Region



Target Variable: Insurance Charges



🔍 Exploratory Data Analysis (EDA)



Insurance charges are highly right-skewed



Significant outliers detected in target variable



Smoking status has the strongest impact on charges



Higher BMI and age increase medical costs



Log transformation applied to stabilize variance and reduce skewness



⚙️ Data Preprocessing



One-hot encoding for categorical variables



Log transformation applied on target variable



Train-test split for model evaluation



🤖 Models Implemented



Linear Regression (Baseline Model)



Ridge Regression (L2 Regularization)



Random Forest Regressor



Hyperparameter tuning using GridSearchCV



📊 Evaluation Metrics



R² Score – Measures explained variance



RMSE (Root Mean Squared Error) – Measures average prediction error



🏆 Model Performance Summary

Model	R² Score	RMSE

RF (Tuned + Log)	0.8796	4323

RF (Log)	0.8769	4370

RF	0.8644	4586

Linear	0.7835	5796

Ridge	0.7835	5796

✅ Best Model:



Random Forest (Tuned + Log Transformation)



💡 Key Insights



Smoking is the most influential factor affecting insurance costs.



BMI and age significantly impact medical expenses.



Random Forest captures non-linear relationships better than linear models.



Log transformation improved model performance by handling skewness.



📁 Project Structure

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



🚀 Future Improvements



Deploy model using Streamlit or Flask



Add SHAP analysis for interpretability



Experiment with XGBoost



🧠 Conclusion



This project demonstrates end-to-end regression modeling, feature engineering, hyperparameter tuning, and performance evaluation to build a reliable medical insurance cost prediction model.

