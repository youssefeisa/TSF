
# 🥑 Avocado Price Forecasting using Time Series

This project predicts the **average price of avocados** over time using time series forecasting methods. The analysis is done in Python with exploratory data analysis (EDA), preprocessing, and model training to forecast future prices.

## 📊 Dataset

The dataset includes historical data on avocado prices, volumes, regions, and types from the U.S. market. Key fields:

- `Date`
- `AveragePrice`
- `Total Volume`
- `type` (conventional/organic)
- `region`

## 🛠️ Workflow Summary

1. **Data Preprocessing**
   - Convert date column to datetime
   - Filter by a specific region (`TotalUS`)
   - Group and average prices per month

2. **Exploratory Data Analysis**
   - Visualize trends and seasonality in avocado prices
   - Check autocorrelation plots

3. **Train-Test Split**
   - Use ~80% of the data for training
   - The rest for validation

4. **Modeling (ARIMA)**
   - Use `auto_arima` for model selection
   - Fit model and make predictions
   - Evaluate performance (e.g., MAE, MSE)

5. **Forecasting**
   - Predict future prices for the next 12 months
   - Visualize actual vs. predicted values

## 📈 Sample Plot

The notebook includes visualizations for:

- Monthly average price trends
- Residual diagnostics
- Forecast for upcoming months

## 🧰 Libraries Used

```bash
pandas
numpy
matplotlib
seaborn
Prophet
```

## 📦 How to Run

1. Clone the repo or download the notebook.
2. Install dependencies (preferably in a virtual environment):

```bash
pip install pandas numpy matplotlib seaborn Prophet
```

3. Run `TSF_For_Avocado.ipynb` in Jupyter Notebook or VS Code.

## 📌 Notes

- The model currently focuses on **Total US** region only.
- Can be extended to regional predictions or multivariate forecasting.

## 📉 Example Forecast Output

The model predicts the next 12 months of average avocado prices with confidence intervals, shown in a time-series plot.

