# Time Series Analysis and Forecasting Report: Champagne Sales

## 1. Project Overview
This project focuses on analyzing and forecasting champagne sales data using time series analysis methods, specifically ARIMA and Seasonal ARIMA models. The goal is to predict future sales patterns based on historical data.

## 2. Data Understanding
- Dataset: Perrin Freres Monthly Champagne Sales
- Time Period: Monthly sales data
- Target Variable: Sales volume
- Initial Data Cleaning:
  - Removed incomplete records
  - Converted date format to datetime
  - Set Month as index
  - Validated data integrity

## 3. Methodology

### 3.1 Time Series Analysis
1. **Stationarity Testing**
   - Performed Augmented Dickey-Fuller (ADF) test
   - Initial data showed non-stationarity
   - Applied first difference and seasonal difference transformations

2. **Differencing Approaches**
   - First-order differencing
   - Seasonal differencing (lag=12)
   - Achieved stationarity after seasonal differencing

### 3.2 Model Development
1. **Model Selection Process**
   - Analyzed ACF and PACF plots
   - Identified significant lags
   - Tested both ARIMA and SARIMA models

2. **Models Evaluated**
   - ARIMA(1,1,1)
   - SARIMA(1,1,1)(1,1,1,12)

## 4. Results

### 4.1 Model Performance
- SARIMA model showed better performance due to:
  - Capture of seasonal patterns
  - Better handling of trend components
  - More accurate predictions

### 4.2 Forecasting
- Generated 24-month future forecast
- Captured seasonal patterns in predictions
- Maintained confidence intervals
- Model successfully captured:
  - Seasonal peaks
  - Overall trend
  - Monthly variations

## 5. Technical Implementation
- Used Python with key libraries:
  - statsmodels for time series analysis
  - pandas for data manipulation
  - matplotlib/seaborn for visualization
- Implementation highlights:
  - Proper data preprocessing
  - Robust model validation
  - Comprehensive diagnostic testing

## 6. Key Findings
1. Strong seasonal pattern in champagne sales
2. Upward trend in overall sales
3. Significant monthly variations
4. Seasonal peaks during specific months

## 7. Limitations and Considerations
1. Limited historical data
2. Assumption of pattern consistency
3. External factors not considered
4. Model sensitivity to seasonal parameters

## 8. Future Improvements
1. Include external variables (holidays, events)
2. Test alternative seasonal models
3. Implement rolling forecasts
4. Develop ensemble approaches

## 9. Conclusion
The SARIMA model effectively captured both trend and seasonal patterns in champagne sales data, providing reliable forecasts for future periods. The model's ability to account for seasonality made it particularly suitable for this business case.