# Customer Churn Analysis and Prediction

This project was developed as part of my **Machine Learning Internship at SaiKet Systems**.

The project focuses on analyzing telecom customer data and building machine learning models to predict whether a customer is likely to churn or not. The main goal is to identify at-risk customers so that businesses can take early retention actions.

## Project Overview

Customer churn means when a customer stops using a company's service. In the telecom industry, predicting churn is important because retaining existing customers is usually more cost-effective than acquiring new ones.

In this project, the Telco Customer Churn dataset was used to analyze customer behavior and predict churn using machine learning models.

## Objectives

* Load and understand the telecom customer churn dataset
* Handle missing values and clean the data
* Encode categorical features for machine learning
* Split the dataset into training and testing sets
* Train multiple machine learning models
* Evaluate models using classification metrics
* Select the best final model for churn prediction

## Dataset

The dataset contains customer information such as:

* Gender
* Senior citizen status
* Partner and dependents
* Tenure
* Phone and internet services
* Contract type
* Payment method
* Monthly charges
* Total charges
* Churn status

The target variable is:

```text
Churn
```

Where:

```text
Yes = Customer churned
No = Customer did not churn
```

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Joblib
* Jupyter Notebook

## Machine Learning Models Used

The following models were trained and compared:

1. Logistic Regression
2. Random Forest Classifier
3. XGBoost Classifier

## Model Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC score
* Confusion Matrix
* ROC Curve

## Final Model Selection

Although Random Forest achieved the highest accuracy, **Logistic Regression** was selected as the final model because it achieved the highest **Recall, F1-score, and ROC-AUC**.

For customer churn prediction, Recall and ROC-AUC are more important than accuracy because the main goal is to correctly identify customers who are likely to leave.

## Final Model Performance

| Model               | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
| ------------------- | -------: | --------: | -----: | -------: | ------: |
| Logistic Regression |    0.738 |     0.504 |  0.783 |    0.614 |   0.841 |
| Random Forest       |    0.784 |     0.623 |  0.473 |    0.538 |   0.819 |
| XGBoost             |    0.752 |     0.526 |  0.668 |    0.589 |   0.819 |

## Final Output

The final trained Logistic Regression model was saved using Joblib as:

```text
customer_churn_logistic_regression_model.pkl
```

This model can be reused later for churn prediction on new customer data.

## Project Conclusion

This project successfully analyzes telecom customer churn and builds predictive machine learning models. Logistic Regression was selected as the final model because it performed best on Recall, F1-score, and ROC-AUC, making it suitable for identifying customers who are likely to churn.

The project can help telecom companies detect high-risk customers early and take retention-focused actions.
