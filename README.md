## Customer Churn Prediction with Enhanced Feature Engineering
This project aims to predict customer churn for a bank using a neural network model. The initial model achieved an accuracy of 84%, which was further improved to 88% through feature engineering. This project demonstrates the impact of data preprocessing and feature engineering on model performance in machine learning.

# Project Overview
The objective of this project is to identify customers likely to churn, providing insights for retention strategies. Feature engineering techniques were applied to create new KPIs (Key Performance Indicators) that improved model accuracy.

#Dataset
The dataset includes customer information such as:

Credit Score
Geography (country)
Gender
Age
Tenure
Balance
Number of Products
Has Credit Card
Is Active Member
Estimated Salary
Exited (target variable indicating churn)

#Feature Engineering
To enhance predictive power, the following new features were created:

Tenure-to-Age Ratio: Indicates how long a customer has stayed relative to their age.
Balance-to-Salary Ratio: Gives insights into a customer’s financial stability.
Average Product Holding per Tenure: Shows the average number of products held per year of tenure.
Credit-to-Age Ratio: Highlights customers with higher credit scores at a younger age.
High Balance Indicator: Flags customers with a balance above a certain threshold.
These KPIs improved the model's ability to detect patterns associated with churn.

#Tools and Techniques
Python Libraries:
Pandas and NumPy for data manipulation.
Matplotlib and Seaborn for data visualization.
TensorFlow (Keras) for building and training the neural network.
scikit-learn for data preprocessing and evaluation metrics.

#Machine Learning Techniques:
Data Preprocessing: One-hot encoding for categorical features and standardization of numerical features.
Feature Engineering: Adding KPIs for improved model accuracy.
Neural Network Model: Built with TensorFlow, using multiple dense layers with ReLU activations.

#Project Results
The model's accuracy increased from 84% to 88% after implementing feature engineering. This demonstrates the value of additional feature insights in enhancing predictive accuracy.