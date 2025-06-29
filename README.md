# 📞 Time Series Forecasting – Call Volume

## 🧭 Project Overview
This project aims to forecast daily call volumes in a call center using time series analysis techniques. Accurate forecasting helps businesses better manage staffing, reduce customer wait times, and optimize operational costs.

The dataset includes historical call data, and the analysis applies classical and machine learning-based time series models to predict future call volumes.

---

## 📂 Dataset Description
- **Source**: Internal call center logs or simulated daily call volume dataset
- **Features**:
  - `Date`: Timestamp of call activity (daily granularity)
  - `Call_Volume`: Number of calls received per day
- **Size**: 2+ years of daily call volume data

---

## 🎯 Objectives
- Perform exploratory time series analysis (trend, seasonality, outliers)
- Apply and compare multiple forecasting models
- Evaluate model performance using appropriate error metrics
- Visualize predicted vs. actual call volumes

---

## 🛠️ Tools & Libraries
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Statsmodels (ARIMA, SARIMA)
- Facebook Prophet
- Scikit-learn
- XGBoost Regressor (for ML-based time series forecasting)
- Visualization: Plotly, Matplotlib

---

## 📈 Models Applied
| Model             | Description                                     |
|------------------|-------------------------------------------------|
| ARIMA            | Baseline model for trend analysis               |
| SARIMA           | Adds seasonality handling                       |
| Facebook Prophet | Handles trend + seasonality + holiday effects   |
| XGBoost          | Used with lag features to create supervised model |

---

## 📊 Evaluation Metrics
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- Visual inspection of predicted vs actual plots

---

## 📉 Key Insights
- Strong weekly seasonality pattern with higher volumes on weekdays
- SARIMA and Prophet performed well on test data with low RMSE
- Holidays and special events had a measurable effect on call spikes
- XGBoost with lag/rolling features offered competitive results but required careful feature engineering

---

## 📁 Folder Structure
call-volume-forecasting/
├── data/
│ └── call_volume.csv
├── notebooks/
│ ├── eda_forecasting.ipynb
│ ├── arima_model.ipynb
│ ├── prophet_model.ipynb
│ └── xgboost_forecasting.ipynb
├── outputs/
│ ├── forecast_plots/
│ └── evaluation_metrics.csv
├── README.md


---

## 🔮 Future Work
- Add external features (e.g., weather, marketing campaigns, system outages)
- Deploy model as an API for real-time forecasting
- Build an interactive dashboard using Streamlit or Power BI

---

## ⚖️ Ethical Considerations
- Ensure forecasts are not used to justify labor reductions without context
- Periodic retraining required to adjust to recent behavioral changes (e.g., post-pandemic call trends)

---

## 👤 Author
**Pragathi Porawakara Arachchige**  
[GitHub Profile](https://github.com/PragathiM007)  
Bellevue University – Applied Data Science
