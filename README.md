# Sales Forecasting using Machine Learning

## Project Overview

This project focuses on predicting future sales using historical retail transaction data. It demonstrates how machine learning can be used to analyze trends, identify patterns, and support business decision-making.

---

## Problem Statement 

The objective of this project is to forecast future sales based on historical data. Accurate forecasting helps businesses manage inventory, reduce losses, and improve operational efficiency.

---

## Dataset

* Dataset: Online Retail Dataset (UCI)
* Description: Transaction-level data from an online retail store

### Key Features:

* InvoiceDate → Date of transaction
* Quantity → Number of items purchased
* UnitPrice → Price per item
* Sales → Total sales (Quantity × UnitPrice)

---

## Data Preprocessing

* Removed missing values from important columns
* Converted date column to datetime format
* Removed invalid transactions (negative or zero values)
* Created a new Sales column

---

## Feature Engineering

* Extracted time-based features:

  * Year
  * Month
  * Day
  * Day of Week
* Created rolling mean (7-day average) to capture trends

---

## Exploratory Data Analysis (EDA)

The following visualizations were used to understand the data:

* Sales trend over time
* Monthly and weekly sales patterns
* Histogram for distribution analysis
* Boxplot for detecting outliers
* Heatmaps for:

  * Seasonal patterns
  * Feature correlations
* Pairplot to analyze relationships between variables

---

## Seasonality Analysis

Time series decomposition was performed to analyze:

* Trend → long-term movement in sales
* Seasonality → repeating patterns
* Residual → random variations

---

## Model Building

* Model Used: Random Forest Regressor
* Features Used:

  * Year, Month, Day, Day of Week
  * Rolling Mean (7-day)

---

## Model Evaluation

The model performance was evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

These metrics help measure prediction accuracy.

---

## Forecasting

The model predicts future sales for the next 30 days based on historical patterns.

---

## Output

* Forecasted sales values
* Visual comparison of historical vs predicted sales
* Optional export of forecast results as CSV

---

## Business Insights

* Sales show clear seasonal and weekly patterns
* Rolling average strongly influences predictions
* Demand varies across time periods

### Business Value:

* Helps in inventory planning
* Reduces overstocking and shortages
* Supports data-driven decision-making

---

## Limitations

* Does not include external factors (holidays, promotions)
* Uses basic time-based features
* Forecast accuracy may vary for long-term predictions

---

## Conclusion

This project demonstrates how machine learning can be used to forecast sales using historical data. The model provides valuable insights that can help businesses improve planning and efficiency.

---

## Tech Stack

| Category | Tools |
|---------|------|
| Language | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Time Series | Statsmodels |
| Environment | Jupyter Notebook |
---

## How to Run

1. Clone the repository
2. Install dependencies:

   ```
   pip install -r requirements.txt
   ```
3. Open the notebook:

   ```
   jupyter notebook
   ```
4. Run all cells

---

## Future Improvements

* Use advanced time-series models (ARIMA, LSTM)
* Include external factors (holidays, promotions)
* Build an interactive dashboard

---

## Acknowledgement

This project was completed as part of a Machine Learning Internship task.

---

## Connect
linkedin - https://www.linkedin.com/in/ankit-kumar-150ab12a6/

