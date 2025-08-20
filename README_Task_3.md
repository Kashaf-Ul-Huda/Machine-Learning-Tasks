# 🛒 Walmart Sales Forecasting Project  

## Project Overview
This project focuses on **predicting future sales** for Walmart stores using historical sales data. It implements **time series forecasting** with multiple machine learning models, including Linear Regression, XGBoost, and LightGBM. The project demonstrates **feature engineering, regression modeling, evaluation, and interactive deployment** using Gradio.  

---

## 🚀 Objectives
- Forecast sales based on historical data.  
- Create **time-based features** (day, month, week, year).  
- Generate **lag and rolling average features** for trend analysis.  
- Apply **regression models** to predict sales.  
- Visualize **actual vs predicted sales** with clear pastel-themed plots.  
- Deploy an **interactive Gradio interface** for real-time predictions.  

---

## 📂 Dataset
**Recommended Dataset:** [Walmart Store Sales Forecast](https://www.kaggle.com/datasets/kyanyoga/sample-sales-data)  

**Key Columns:**
- `ORDERDATE` – Date of the order  
- `SALES` – Sales amount (target variable)  
- `CITY`, `COUNTRY`, `DEALSIZE` – Categorical features  
- Other features: `QTR_ID`, `MONTH_ID`, `YEAR_ID`  

**Notes:**  
- The dataset contains historical sales for multiple stores and regions.  
- Time-based features are extracted from the `ORDERDATE` column.  

---

## 🧩 Features Engineering
- **Time-based features:** Month, Week, Day, Year  
- **Lag features:** Previous 1–8 weeks sales  
- **Rolling averages:** 3-week and 6-week rolling mean  
- **Categorical encoding:** Numeric codes for CITY, COUNTRY, DEALSIZE  

---

## 🧠 Models Implemented
1. **Linear Regression** – baseline regression model  
2. **XGBoost Regressor** – gradient boosting for non-linear relationships  
3. **LightGBM Regressor** – gradient boosting with log-transform for stability  

**Bonus Features:**  
- Seasonal decomposition of sales  
- Rolling mean visualization  
- Pastel-themed plots for clear interpretation  

---

## ⚡ Evaluation Metrics
- **Mean Squared Error (MSE)**  
- **Mean Absolute Error (MAE)**  
- **R² Score**  

Metrics are computed on a **time-aware train-test split** to respect chronological order.  

---

## 📊 Visualization
- **Actual vs Predicted Sales** – pastel-colored line plots  
- **Rolling Mean Trend** – 3-week and 6-week rolling averages  
- **Seasonal Decomposition** – trend, seasonality, and residual plots  

---

## 🖥️ Gradio Interactive Deployment
- Users can **input a date** and select a model (Linear Regression, XGBoost, or LightGBM)  
- The interface predicts **sales for the given date**  
- Handles **lags, rolling averages, and categorical features** automatically  
- Includes **error handling** for missing or invalid inputs  
- Pastel-themed output for professional presentation  

---

## 🔧 Technologies & Libraries
- Python (3.10+)  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost, LightGBM  
- Statsmodels (for seasonal decomposition)  
- Gradio (interactive deployment)  

---
