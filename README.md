
# Daily Temperature Forecasting using Time Series Analysis

**Status**: Work In Progress  
**Last Updated**: March 29th 2025

This project focuses on time series forecasting of daily minimum temperatures using statistical models such as ARIMA, SARIMA, Holt-Winters, and Regression with seasonality. The dataset consists of daily minimum temperature data recorded in Melbourne, Australia.

---

## 📂 Project Overview

The goal of this project is to:
- Understand and prepare the time series dataset.
- Perform exploratory data analysis (EDA) and check for stationarity.
- Apply different forecasting models to predict temperature of next one weeks and for 365 days and evaluate their performance.
- Visualize predictions and compare results.

---

## 📊 Dataset

- **Name**: Daily Minimum Temperatures in Melbourne
- **Description**: Contains daily minimum temperatures (in Celsius) from 1981 to 1990.
- **Source**: https://www.kaggle.com/datasets/shenba/time-series-datasets?select=daily-minimum-temperatures-in-me.csv
- **Records**: 3650 daily observations
- **Columns**:
  - `Date`: Date of the observation
  - `Daily minimum temperatures`: Temperature in °C

---

## ✅ Project Steps

1. **Data Exploration and Visualization**
   - Inspecting the dataset and identifying missing values.
   - Visualizing the time series to understand seasonality and trends.

2. **Stationarity Testing**
   - Applied **ADF (Augmented Dickey-Fuller)** Test to check stationarity.

3. **Time Series Decomposition**
   - Decomposed the series into **Trend**, **Seasonality**, and **Residuals**.

4. **Forecasting Models Applied**
   - **Seasonal Naiva**: Completed
   - **Simple Exponential Smoothening** (Completed)
   - **ARIMA / SARIMA** (Seasonal ARIMA): Suitable for stationary data with seasonal patterns. (Completed) 
   - **Holt-Winters Exponential Smoothing**: Modeled seasonality and trend components explicitly. (In-Progress)
   - **Regression with Quadratic Trend & Seasonality**: (In Progress)
     - Modeled time and time squared with seasonal dummy variables or Fourier terms.

6. **Evaluation Metrics**
   - RMSE (Root Mean Square Error)
   - MAE (Mean Absolute Error)
   - MAPE (Mean Absolute Percentage Error)
   - Visual comparison of actual vs. forecasted values.

7. **Forecasting & Visualization**
   - Forecasted next 365 days of minimum temperatures.
   - Visualized forecasts along with confidence intervals.
   - Compared model predictions on validation data.

---

## 🔧 Technologies & Libraries Used

| Library        | Purpose                           |
|----------------|-----------------------------------|
| **Python**     | Core programming language        |
| **pandas**     | Data manipulation & preparation  |
| **numpy**      | Numerical computations           |
| **matplotlib** | Visualization                    |
| **statsmodels**| Time series decomposition & modeling |
| **pmdarima**   | Auto ARIMA modeling (SARIMA)     |
| **prophet**    | Advanced time series forecasting (optional extension) |

---

## 🚀 Results

- **Seasonality**: Strong yearly seasonal pattern observed.
- **Trend**: No significant long-term trend post differencing.
- **Best Performing Model**: *WIP*
- **Forecast**: *WIP*

---

## Repository Structure
📁 Temperature-Forecasting/ ├── data/ │ └── daily-minimum-temperatures-in-me.csv ├── notebooks/ │ └── Temperature Forecasting.html (Jupyter Notebook exported as HTML) ├── images/ │ └── plots.png (optional for visuals) ├── README.md └── requirements.txt

---

##  How to Run This Project

 Clone the repo:
   git clone https://github.com/yourusername/Temperature-Forecasting.git
   cd Temperature-Forecasting

   pip install -r requirements.txt

---

👨‍💻 Author

Shivani Kanodia




