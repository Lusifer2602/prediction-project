# Customer Churn Prediction

## Dataset
The dataset used for this project is `WA_Fn-UseC_-Telco-Customer-Churn.csv`, which contains customer demographics, account information, and churn labels.

## How to Run the Project
   1. **Run the Jupyter Notebook**:
   Open and execute the `Customer_Churn_Prediction_using_ML.ipynb` file in Jupyter Notebook or any compatible IDE.

   Type this command in the terminal after opening the project
   ```
   pip install -r requirements.txt
   ```
   2. Run the Jupyter file's cells after installing neccessary libraries

   3. **Make Predictions**:
   - Load the saved model (`customer_churn_model.pkl`) and encoders (`encoders.pkl`).
   - Prepare input data in the same format as the dataset.
   - Use the model to predict churn and probabilities.


## Subject
Business Analytics Project on Predictive Modeling for Customer Churn.

## Problem Description
The task is to develop a predictive model to identify the likelihood of customer churn for a business or service. This involves:
- Analyzing customer data.
- Identifying key predictors of churn.
- Building a model that can forecast potential customer attrition.

## Steps Followed for Model Development

### 1. Data Collection and Preparation
- Gather historical customer data, including demographics, purchase history, service usage patterns, customer service interactions, and other relevant data.
- Clean and preprocess the data for analysis, handling missing values, and ensuring data quality.

### 2. Exploratory Data Analysis (EDA)
- Conduct an initial analysis to understand the data’s characteristics and identify patterns and trends.
- Use visualizations to uncover insights and relationships between variables.

### 3. Feature Selection and Engineering
- Identify which features are most predictive of customer churn.
- Consider creating new features that might improve the model's performance.

### 4. Model Selection
- Choose appropriate predictive modeling techniques (e.g., logistic regression, decision trees, random forests, or neural networks) based on the data and the problem’s nature.
- Experiment with different models to determine which performs best.

### 5. Model Training and Validation
- Split the data into training and testing sets.
- Train the model on the training set and validate its performance on the test set using appropriate metrics (e.g., accuracy, precision, recall, F1-score).

### 6. Model Evaluation and Tuning
- Evaluate the model’s performance and adjust parameters as needed to improve accuracy.
- Use techniques like cross-validation for more robust model evaluation.

### 7. Interpretation of Results and Insights
- Analyze the model’s findings to draw meaningful insights about customer churn.
- Identify key factors contributing to churn and suggest potential strategies to retain customers.

### 8. Report and Presentation
- Prepare a comprehensive report detailing your methodology, findings, and business insights.
- Develop a presentation to communicate the results to stakeholders, focusing on actionable recommendations.

## Reference Material
The following resources provide foundational knowledge and advanced techniques in predictive modeling and customer churn analysis:
- [How to Build a Customer Churn Prediction Model in Python](https://365datascience.com/tutorials/python-tutorials/how-to-build-a-customer-churn-prediction-model-in-python/)
- [Churn Modeling: A Detailed Step-by-Step Guide in Python](https://medium.com/@lucapetriconi/churn-modeling-a-detailed-step-by-step-guide-in-python-1e96d51c7523)
- [Customer Churn Detection Using Sklearn in Python](https://thepythoncode.com/article/customer-churn-detection-using-sklearn-in-python)



## Dataset
The dataset used for this project is `WA_Fn-UseC_-Telco-Customer-Churn.csv`, which contains customer demographics, account information, and churn labels.

## How to Run the Project

## Key Insights
- Customer churn prediction helps businesses identify at-risk customers and take proactive measures to retain them.
- The project demonstrates the use of machine learning techniques like Random Forest and SMOTE for handling class imbalance.

This project offers a great opportunity to showcase analytical skills in a practical business context, providing valuable insights for customer retention strategies.