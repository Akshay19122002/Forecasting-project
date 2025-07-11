# Forecasting Model

This project forecasts sales using ARIMA and Linear Regression based on historical sales data from different regions.

## Sample Data
| Date                | Sales | Region |
|---------------------|-------|--------|
| 2023-01-01 00:00:00 | 524   | North  |
| 2023-01-08 00:00:00 | 493   | South  |
...

## 📊 Forecast Graph
![graph](https://github.com/user-attachments/assets/81833a51-344b-4a0d-afc5-03b1077ec90c)

## Installation
pip install pandas openpyxl matplotlib statsmodels scikit-learn



import pandas as pd 
import matplotlib.pyplot as plt
from statsmodels.tsa.arima.model
from sklearn.linear_model

# Load dummy data
df = pd.read_excel('dummy_sales_data.xlsx')
print(df.head())



# Clean and sort data
df['Date'] = pd.to_datetime(df['Date'])
df = df.sort_values('Date')

# Plot sales over time
plt.plot(df['Date'], df['Sales'])
plt.title("Sales Over Time")
plt.xlabel("Date")
plt.ylabel("Sales")
plt.show()





