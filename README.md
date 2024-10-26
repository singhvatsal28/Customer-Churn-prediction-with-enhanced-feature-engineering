# Project Overview

This project aims to predict customer churn in a banking context by analyzing customer demographics, account information, and behavioral data. Churn prediction is critical for banks as it helps them proactively retain valuable customers who might otherwise leave. By accurately identifying potential churners, the bank can implement targeted retention strategies and reduce revenue loss.

The project leverages a neural network model to classify customers as likely to churn or not. Initially, the model achieved an accuracy of **84%**. However, through feature engineering, we introduced new key performance indicators (KPIs) that significantly improved the model's predictive power, ultimately increasing accuracy to **88%**.

## Objectives
- **Predict Customer Churn**: Use machine learning to classify customers as likely to churn or retain.
- **Improve Prediction Accuracy**: Employ feature engineering to create new features that provide additional insights into customer behavior.
- **Data-Driven Decision Making**: Equip the bank with insights to design retention strategies based on data.

## Approach
The workflow for this project included the following steps:

- **Data Preprocessing**: 
  - Cleaned and prepared the data by handling missing values and converting categorical variables into a usable format.
  - Standardized numerical features to ensure all data is on a comparable scale, which is especially important for neural networks.

- **Feature Engineering**:
  - Created additional features to better capture customer behavior and risk of churn. Examples include:
    - **Tenure-to-Age Ratio**: Measures customer loyalty relative to their age.
    - **Balance-to-Salary Ratio**: Indicates financial stability, showing how much of their salary customers typically retain in their balance.
    - **Average Product Holding per Tenure**: Shows engagement by quantifying the average number of products held over the tenure period.
    - **Credit-to-Age Ratio**: Highlights customers who achieved high credit scores at a younger age, which may correlate with responsible behavior.
    - **High Balance Indicator**: Flags high-value customers by identifying those with a balance above a set threshold.
  - These KPIs improved the model's ability to identify patterns linked to customer churn.

- **Modeling**:
  - Used a neural network model built with TensorFlow and Keras. The model architecture includes multiple dense layers with ReLU activation functions, optimizing the network’s ability to capture complex relationships in the data.
  - Implemented training and evaluation metrics to assess model performance, using accuracy and a confusion matrix to understand the true positive, true negative, false positive, and false negative rates.

- **Evaluation**:
  - After feature engineering, the model's accuracy improved from **84% to 88%**. This improvement highlights the importance of carefully engineered features in making machine learning models more accurate.
  - Visualizations, including churn distribution, feature correlations, and training/validation accuracy plots, were used to further understand the data and model performance.

- **Interpretability and Usage**:
  - The model can now be used to predict churn for new customers by feeding in their demographic and account data. Predictions allow the bank to proactively address high-risk customers, offering personalized retention offers and improved service.

## Key Takeaways
This project demonstrates the importance of feature engineering in improving machine learning models, especially for classification tasks like churn prediction. By carefully examining and creating additional features, the model can capture complex customer behaviors, leading to better accuracy and more actionable insights.
