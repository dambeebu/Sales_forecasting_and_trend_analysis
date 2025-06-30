# Sales Forecasting and Trend Analysis

This project analyzes sales data, visualize trends and forecasts future sales using multiple time series models. 

## Key Findings
- **Sales Trends:**
  - Sales generally show a positive trend over the years, with noticeable seasonality in certain months.
  - The highest sales are typically observed in the last quarter of each year, indicating strong end-of-year demand.
   <img src="images/monthly_sales_2018.png" alt="Monthly Sales 2018" width="600">
- **Top States:**
  - The top 10 states contribute a significant portion of total sales, with certain states consistently outperforming others.
  - State-level analysis reveals regional strengths and opportunities for targeted marketing.
- **Category Insights:**
  - Technology, Furniture, and Office Supplies each have distinct sales patterns across states.
  - Technology often leads in total sales, but some states show higher demand for Furniture or Office Supplies.
- **Forecasting Performance:**
  - All four models (SARIMA, ARIMA, Prophet, Exponential Smoothing) provide reasonable forecasts, with SARIMA and Prophet generally achieving the lowest error metrics (MAE, RMSE, MAPE).
  - The models successfully capture both trend and seasonality, with forecasts indicating continued growth in the coming months.
- **Business Implications:**
  - The analysis supports data-driven decision-making for inventory planning, sales strategy, and resource allocation.
  - Forecasts can be used to anticipate demand spikes and optimize supply chain operations.

## Features
- **Data Loading & Preprocessing:**
  - Reads sales data from CSV.
  - Parses date columns and sets up time-based features.
- **Exploratory Data Analysis (EDA):**
  - Visualizes sales trends by month, year, state, and category.
  - Identifies top-performing states and categories (Furniture, Office Supplies, Technology).
- **Time Series Forecasting:**
  - Implements and compares four forecasting models:
    - SARIMA (Seasonal ARIMA)
    - ARIMA
    - Prophet
    - Exponential Smoothing (Holt-Winters)
  - Evaluates models using MAE, RMSE, and MAPE.
  - Visualizes actual vs. predicted sales and forecasts for the next 6–12 months.
- **Model Saving:**
  - Saves all trained models as `.pkl` files for future use or deployment.


## Requirements
- Python 3.7+
- pandas, numpy, matplotlib, seaborn
- statsmodels, scikit-learn, prophet, joblib

Install requirements with:
```bash
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn prophet joblib
```

## Usage
1. Open `model.ipynb` in Jupyter or VS Code.
2. Run all cells sequentially:
   - Data loading and preprocessing
   - EDA and visualization
   - Time series modeling and evaluation
   - Model saving
3. Download the generated model files if needed:
   - `sarima_model.pkl`
   - `arima_model.pkl`
   - `prophet_model.pkl`
   - `exp_smoothing_model.pkl`

## Customization
- Tune model parameters for better accuracy.
- Adapt the workflow for other time series datasets.


