# Credit Card Fraud Detection

## About
Our team's objective is to identify common characteristics of fraudulent credit transactions. We hope that our findings would allow for early detection and prevention, and also strengthen existing security measures to stay ahead of evolving fraudulent tactics. 
(can insert a pic here of our proj lol)

## Problem Definition
### How can we detect fraudulent e-commerce transactions using machine learning models based on transaction data?
- Are we able to identify patterns in fraudulent transactions?

- Which aspect of credit transactions did these patterns arise?

- Which model would be best to predict if a credit transaction was fraudulent based on the identified factors?

## Dataset Used
[Credit Card Data](https://raw.githubusercontent.com/alow023/ECDS_Team4/refs/heads/main/CreditCardData.csv?token=GHSAT0AAAAAADBQ7CU26HRDLZ4PX22NIPCU2ACNNXA)

## Models Used
- Lasso Regression
- XGBoost

## 1. Data Extraction and Exploratory Analysis
Data cleaning was carried out by removing null rows and irrelevant aspects of credit transactions. Pandas was used to visualise raw data, allowing us to identify the imbalance in the dataset, which we balanced using undersampling. 

## 2. Machine Learning 
Lasso regression was used to identify numeric features in our dataset which were important in identifying fraud cases. We then used XGBoost to identify both categorical and numeric variables which were the more influential features in the train set. The more important features are used higher up in the decision tree of the model and is prioritised in subsequent tree-building steps. The decision tree is then used to predict if transactions in the test set are fraudulent. 

## 3. Pattern Identification
We decided to choose the top 5 features to identify patterns to predict if a transaction was fraudulent. Each of the top 5 features had obvious categories that were targetted by scammers. 

## Conclusion
We are able to identify fraudulent credit card transactions using machine learning models. 
- The top 5 most influential features include: Time of transaction, Merchant Group, Transaction Entry mode, whether the Country of Residence of the transactor was the same as the Country of Transaction, Amount transacted.
- Fraudulent transactions were more likely to happen from 12am to 6am
- Merchant groups: Children, Electronics and Fashion were more susceptible to frauds.
- Credit Verification Code entry mode was the most common entry mode for frauds
- There is a higher probability of the transaction being fraudulent if the country of residence of the transactor was different from the country of transaction
- A significant proportion of fraudulent transactions involved only small amounts of money from about 5 to 30 pounds. 

## Contributions
- Data Cleaning, Initial Exploratory Data Analysis, Analysis of Model: Reina @reinachye
- Training of XGBoost, Training of Lasso Regression, Secondary Exploratory Data Analysis: Arissa @alow023
- Data-driven Insights: Both

## References
- https://www.kaggle.com/datasets/anurag629/credit-card-fraud-transaction-data?resource=download
- https://scikit-learn.org/stable/api/sklearn.linear_model.html
- https://www.nvidia.com/en-sg/glossary/xgboost/

  
