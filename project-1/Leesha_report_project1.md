# Customer Churn Prediction Project Report

## 1. Project Overview
This project focuses on developing a predictive model for customer churn using the Telco Customer Churn dataset. The goal is to help businesses identify customers likely to churn and take proactive retention measures.

## 2. Data Understanding
- Dataset: Telco Customer Dataset (`WA_Fn-UseC_-Telco-Customer-Churn.csv`)
- Shape: Multiple customer features including demographics and service usage 
- Target Variable: Churn (Binary - Yes/No)

## 3. Methodology

### 3.1 Data Preprocessing
- Removed CustomerID as it's not relevant for modeling
- Handled missing values in TotalCharges column by replacing with 0
- Performed Label Encoding on categorical variables
- Features include:
  - Demographics: gender, SeniorCitizen, Partner, Dependents
  - Services: PhoneService, InternetService, OnlineSecurity, etc.
  - Billing: Contract, PaperlessBilling, PaymentMethod
  - Numerical: tenure, MonthlyCharges, TotalCharges

### 3.2 Exploratory Data Analysis (EDA)
- Analyzed distribution of numerical features
  - tenure: Relatively uniform distribution
  - MonthlyCharges: Right-skewed distribution
  - TotalCharges: Right-skewed distribution
- Examined categorical variables through count plots
- Identified class imbalance in target variable (Churn)

### 3.3 Model Development
1. **Data Split**:
   - Training set: 80%
   - Test set: 20%

2. **Class Imbalance Handling**:
   - Applied SMOTE (Synthetic Minority Over-sampling Technique)
   - Balanced the classes in training data

3. **Models Evaluated**:
   - Decision Tree
   - Random Forest
   - XGBoost

4. **Model Selection**:
   - Random Forest chosen as final model based on cross-validation results

## 4. Results

### 4.1 Model Performance
- Accuracy Score: ~80%
- Balanced performance on both churn and non-churn predictions
- Cross-validation used to ensure robust performance

### 4.2 Key Findings
1. Model successfully identifies potential churners
2. Important predictors include:
   - Contract type
   - Monthly charges
   - Tenure
   - Internet service type

## 5. Technical Implementation
- Used Python with key libraries:
  - scikit-learn for modeling
  - pandas for data manipulation
  - matplotlib/seaborn for visualization
  - imblearn for SMOTE
- Model and encoders saved for future use:
  - `customer_churn_model.pkl`
  - `encoders.pkl`

## 6. Business Implications
1. **Proactive Customer Retention**:
   - Early identification of at-risk customers
   - Targeted retention strategies

2. **Cost Efficiency**:
   - Better resource allocation for retention efforts
   - Reduced customer acquisition costs

## 7. Recommendations
1. Focus on long-term contracts to reduce churn
2. Monitor monthly charges and their impact on churn
3. Improve service quality in identified high-risk areas
4. Implement regular model updates with new data

## 8. Future Improvements
1. Hyperparameter tuning for better model performance
2. Feature engineering for more predictive power
3. Testing alternative modeling approaches
4. Incorporating more customer interaction data

## 9. Conclusion
The project successfully developed a reliable churn prediction model that can be used for proactive customer retention strategies. The model's performance and insights provide valuable tools for business decision-making.