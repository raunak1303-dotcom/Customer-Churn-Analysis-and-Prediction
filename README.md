# 📊 Customer Churn Analysis and Prediction

A Machine Learning internship project developed as part of my Machine Learning Internship at SaiKet Systems.

This project predicts whether a telecom customer is likely to churn using customer service, billing, and contract-related data. The final model is also deployed as an interactive Streamlit web app.

## 🚀 Live Demo

Streamlit App:
https://customer-churn-analysis-and-prediction-raunak.streamlit.app

## 📌 Project Overview

Customer churn means when a customer stops using a company’s service. For telecom companies, predicting churn is important because it helps identify at-risk customers early and take retention actions before they leave.

In this project, I analyzed the Telco Customer Churn dataset, trained multiple machine learning models, compared their performance, selected the final model, and deployed it as a working web application.

## 🎯 Internship Task Requirements

The task given by SaiKet Systems was to complete a Customer Churn Analysis and Prediction project covering:

- Data preparation and preprocessing
- Missing value handling
- Categorical variable encoding
- 80:20 train-test split
- Feature selection
- Model selection
- Model training
- Model evaluation using Accuracy, Precision, Recall, F1-score, and ROC-AUC

## ✅ Tasks Performed for Project Development

Along with completing the assigned internship requirements, I also performed additional development work to make the project more complete and practical:

- Cleaned and prepared the Telco Customer Churn dataset
- Converted TotalCharges into numeric format and handled missing values
- Removed unnecessary columns like customerID
- Encoded categorical features using OneHotEncoder
- Scaled numerical features using StandardScaler
- Trained and compared Logistic Regression, Random Forest, and XGBoost
- Evaluated models using Accuracy, Precision, Recall, F1-score, and ROC-AUC
- Selected Logistic Regression as the final model based on Recall, F1-score, and ROC-AUC
- Saved the trained model using Joblib
- Built an interactive Streamlit web app
- Deployed the app using Streamlit Community Cloud
- Added GitHub documentation for better project presentation

## 🧠 Models Used and Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 0.738 | 0.504 | 0.783 | 0.614 | 0.841 |
| Random Forest | 0.784 | 0.623 | 0.473 | 0.538 | 0.819 |
| XGBoost | 0.752 | 0.526 | 0.668 | 0.589 | 0.819 |

## 🏆 Final Model

Logistic Regression was selected as the final model.

Although Random Forest achieved the highest accuracy, Logistic Regression performed better in Recall, F1-score, and ROC-AUC. For churn prediction, Recall is especially important because the goal is to correctly identify customers who are likely to leave.

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Streamlit

## 📁 Repository Files

- sks_intern_project.ipynb
- app.py
- requirements.txt
- runtime.txt
- README.md
- Telco_Customer_Churn_Dataset.csv
- customer_churn_logistic_regression_model.pkl

## ▶️ How to Run Locally

Clone the repository:

git clone https://github.com/raunak1303-dotcom/Customer-Churn-Analysis-and-Prediction.git

Move into the project folder:

cd Customer-Churn-Analysis-and-Prediction

Install dependencies:

pip install -r requirements.txt

Run the Streamlit app:

streamlit run app.py

## 📌 Conclusion

This project successfully predicts telecom customer churn using machine learning. Logistic Regression was chosen as the final model because it performed best on the most important churn-focused metrics: Recall, F1-score, and ROC-AUC.

The project was further improved by deploying it as a live Streamlit web app, making the churn prediction system interactive and easy to use.