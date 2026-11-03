# Customer Churn Prediction

A machine learning project that analyses customer data to identify churn patterns and predict whether a customer is likely to leave a telecommunications service.

## Project Overview

The project involves data cleaning, exploratory data analysis, model building, and evaluation to predict customer churn.

## Technologies Used

* Python
* Pandas and NumPy
* Matplotlib and Seaborn
* Scikit-learn
* XGBoost
* Imbalanced-learn
* Joblib
* Jupyter Notebook

## Machine Learning Models

The following classification algorithms were implemented and compared:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

SMOTE, cross-validation, and RandomizedSearchCV were used to handle class imbalance and optimize model performance.

## Results

The tuned XGBoost model achieved the following results:

| Metric    |  Score |
| --------- | -----: |
| Accuracy  | 76.72% |
| Precision | 54.46% |
| Recall    | 75.13% |
| F1-Score  | 63.15% |
| ROC-AUC   | 84.14% |

## How to Run

1. Clone this repository.

2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost joblib jupyter
   ```

3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `customer_churn_analysis.ipynb` and run the cells.

## Dataset

IBM Telco Customer Churn dataset.
