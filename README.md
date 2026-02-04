# Employee Turnover Prediction
Overview:
This project analyzes employee HR data to identify factors associated with employee turnover and builds a logistic regression model to predict whether an employee will leave the company. The goal is to understand key drivers of attrition and evaluate how well an interpretable model captures turnover patterns.

Data:
The dataset used in this project comes from Kaggle and contains employee-level information such as job satisfaction, workload, tenure, performance evaluation, department, and promotion history.

Dataset source:
https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction

Methods:
- Data cleaning and preprocessing, including duplicate handling
- Exploratory data analysis to examine distributions and potential outliers
- One-hot encoding of categorical variables and feature scaling
- Train-test split with stratification
- Logistic regression model
- Model evaluation using accuracy, ROC AUC, confusion matrix, classification report, and false negative/positive rates

Key Results:
- Accuracy: approximately 83%
- ROC AUC: approximately 0.83
- The model performs well at identifying employees who stay, but has lower recall for employees who leave due to class imbalance
- Error rate analysis reveals a high false negative rate, indicating that some employees who left were predicted to stay

Interpretation:
The model is not intended for individual-level decision making but is effective at highlighting broader patterns related to employee satisfaction, workload, tenure, and turnover risk. These insights can support organizational efforts to better understand and address employee retention challenges.

Future Work:
Future improvements could include optimizing recall, adjusting classification thresholds, or testing alternative models to better identify employees at risk of leaving.

Tools Used:
Python, pandas, NumPy, scikit-learn, matplotlib, seaborn
