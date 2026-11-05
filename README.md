# Fraud Detection in Mobile Money Transactions – Ghana (Power BI + Machine Learning)

## Business Problem
Mobile money is widely used in Ghana, but fraud remains a major challenge that causes financial losses for both users and providers. This project aims to detect fraudulent transaction patterns and identify the most effective machine learning model for flagging suspicious activity.

## Approach
- Used the PaySim dataset (~6 million transactions)
- Compared three models: Logistic Regression, Random Forest, and XGBoost
- Evaluated models using Precision, Recall, F1-Score, and AUC-ROC
- Built an interactive Power BI dashboard to visualize fraud patterns and model performance

## Key Results
| Model              | Precision | Recall | F1-Score | AUC-ROC |
|--------------------|-----------|--------|----------|---------|
| Random Forest      | 0.63      | **0.96** | **0.76** | **0.99** |
| XGBoost            | 0.41      | **0.99** | **0.58** | **0.99** |
| Logistic Regression| 0.03      | **0.87** | **0.05** | **0.97** |

**Best Model:** Random Forest  
It provided the best balance, catching 96% of fraudulent transactions while maintaining a strong AUC-ROC of 0.99 and a higher precision.

## Key Insights 
- Fraudulent transactions occured mostly during CASH_OUT and Transfers as to other types of transactions such as Payment and Debit.
- The important feature for detecting fraud were Origin Old balance, Transaction amount, origin new balance and Transaction type
## Dashboard
![Power BI Dashboard Overview]("https://github.com/user-attachments/assets/640b550f-1367-4c8a-bb9d-d3da68eaaa03")

![Fraud Patterns by Amount](<img width="1548" height="682" alt="avg tran vs amount" src="https://github.com/user-attachments/assets/95f65b7c-6f84-449c-8497-6614fbd64c5a" />)


## Tools & Technologies
- Python (pandas, scikit-learn, XGBoost)
- Power BI
- Jupyter Notebook

## Project Files
- `fraud_detection_models.ipynb` — Model training and comparison
- `mobile_money_fraud_dashboard.pbix` — Interactive Power BI dashboard

## Author
Raymond Opoku  
MBA (Business Intelligence & Data Analytics)  
[LinkedIn] | [@ROpoku2](https://github.com/ROpoku2)
