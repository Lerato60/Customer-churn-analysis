# Customer Churn Analysis

## Overview
Analysis of customer churn for a telecom company using the IBM Telco Customer Churn dataset.
The goal is to identify the key drivers of churn and build models to predict which customers are at risk of leaving.

## Dataset
- **Source:** [IBM Telco Customer Churn – Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Size:** 7,043 customers, 21 features
- **Target variable:** `Churn` (Yes/No)

## Key Findings
- Customers on **month-to-month contracts** churn at ~43%, vs ~3% on two-year contracts
- **Churned customers** have an average tenure of 18 months vs 38 months for retained customers
- **Higher monthly charges** are associated with higher churn (avg R74 vs R61)
- Contract type, tenure, and monthly charges are the strongest predictors of churn

## Models Used
| Model | Accuracy | F1-Score | ROC-AUC |
|---|---|---|---|
| Logistic Regression | 0.806 | 0.604 | 0.842 |
| Random Forest | 0.782 | 0.544 | 0.826 |

## How to Run
1. Clone the repo
2. Install dependencies: `pip install -r requirements.txt`
3. Download the dataset from Kaggle and place it in a `dataset/` folder
4. Open and run `Customer_churn_analysis.ipynb`

## Requirements
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
