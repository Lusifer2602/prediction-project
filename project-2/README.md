# Project Title : Finacial Time Series Forecasting Project 

## Decription
This project demonstrates the use of time series analysis techniques for financial forecasting. The goal is to analyze historical data, make it stationary, and build predictive models to forecast future values.

## How To Run The Project

1. In your terminal copy and paste this command to download all the required dependencies altogether

```bash
pip install pandas numpy matplotlib seaborn xgboost scikit-learn
```
2. Open the Jupyter notebook
3. Choose your working environment
4. Run all cells using 'Run All' button (press it 2 times atleast to ensure data is filtered correctly as per the notebook's instructions.)

### Reference Material:
####  https://www.mlq.ai/python-for-finance-time-series-analysis/
####  https://christianmartinezfinancialfox.medium.comlearning-python-for-finance-how-to-get-started-with-advanced-financial-forecasting-in-python-43553dac9d69
####  https://www.kaggle.com/code/prashant111/complete-guide-on-time-series-analysis-in-python

## Features

- **Data Loading and Preprocessing**:
  - Load historical sales data from a CSV file.
  - Handle missing values and clean the dataset.
  - Convert date columns to datetime format and set them as the index.

- **Exploratory Data Analysis (EDA)**:
  - Visualize the time series data to identify trends and seasonality.
  - Test for stationarity using the Augmented Dickey-Fuller (ADF) test.

- **Data Transformation**:
  - Apply differencing to make the data stationary.
  - Perform seasonal differencing to account for seasonality.

- **Autocorrelation and Partial Autocorrelation**:
  - Plot autocorrelation (ACF) and partial autocorrelation (PACF) to identify ARIMA model parameters.

- **Model Building**:
  - Build ARIMA and SARIMA models for time series forecasting.
  - Train the models on the historical data.

- **Forecasting**:
  - Generate forecasts for future time periods.
  - Visualize the actual vs. forecasted values.

- **Future Predictions**:
  - Extend the time series to predict future values for additional months.

## Libraries Used

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical computations.
- `matplotlib`: For data visualization.
- `statsmodels`: For statistical modeling and time series analysis.

#### Submitted By : Leesha Goel