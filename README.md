# Bank_customer_churn_prediction

Overview
This project predicts customer churn for a bank using machine learning techniques. Churn prediction helps banks identify customers likely to leave, enabling proactive retention strategies. The project involves comprehensive EDA (Exploratory Data Analysis), feature engineering, and the implementation of several machine learning algorithms, including:

XGBoost
Bagging Boosting
SVM
Random Forest
Decision Tree
Logistic Regression
A comparative analysis of model performance has been conducted to identify the best-performing algorithm.

Dataset
The dataset used for this project was obtained from Kaggle. It contains information about:

Demographics: Age, Gender, Geography
Bank Details: Tenure, Balance, Products, Credit Score
Target Variable: Exited (1 = Customer Churned, 0 = Retained)
Dataset Features
RowNumber: Row index
CustomerId: Unique identifier for a customer
Surname: Customer surname
CreditScore: Credit score of the customer
Geography: Customer's location
Gender: Gender of the customer
Age: Age of the customer
Tenure: Number of years as a customer
Balance: Bank balance
NumOfProducts: Number of bank products
HasCrCard: Whether the customer has a credit card
IsActiveMember: Whether the customer is an active member
EstimatedSalary: Customer's estimated salary
Exited: Whether the customer churned (1) or stayed (0)
Exploratory Data Analysis (EDA)
EDA was conducted to understand the data, clean it, and identify relationships between variables. Key steps include:

Data Cleaning: Handled missing or incorrect values.
Visualization: Used heatmaps, histograms, and boxplots to identify trends.
Feature Correlation: Analyzed relationships between features and the target variable using a correlation heatmap.
Machine Learning Models
Six algorithms were implemented for churn prediction:

Logistic Regression: Simple and interpretable baseline model.
Decision Tree: Captures non-linear relationships.
Random Forest: Combines multiple trees for better performance.
SVM (Support Vector Machine): Handles high-dimensional data well.
Bagging and Boosting (e.g., AdaBoost): Aggregates predictions for improved accuracy.
XGBoost: Advanced gradient boosting technique for handling imbalanced datasets.
Performance Metrics
Each model was evaluated using:

Accuracy
Precision
Recall
F1 Score
AUC-ROC Curve
Results
Best Performing Model
The XGBoost algorithm outperformed other models in terms of:

Accuracy: 89%
Recall: Effectively identified churned customers.
AUC-ROC: Demonstrated excellent ability to separate churned and retained customers.
Why XGBoost performed best:

Handles missing data efficiently.
Mitigates overfitting with regularization techniques.
Works well with tabular data and captures complex patterns.
Conclusion
This project demonstrates how machine learning can effectively predict bank customer churn. By identifying high-risk customers, banks can develop targeted retention strategies, ultimately improving customer satisfaction and reducing losses.

Future Work
Incorporate Deep Learning techniques for further improvement.
Use real-time data for dynamic predictions.
Add explainable AI (XAI) to interpret model decisions better.
How to Run the Project
Clone this repository:
bash
Copy code
git clone https://github.com/your-username/bank-churn-prediction.git
Install required libraries:
bash
Copy code
pip install -r requirements.txt
Run the project:
bash
Copy code
python main.py
Technologies Used
Programming Language: Python
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost
