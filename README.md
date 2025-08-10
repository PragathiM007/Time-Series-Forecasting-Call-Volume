# 📞 Time Series Forecasting – Call Volume

## 📌 Project Overview
This project forecasts daily call volumes for a call center using historical call data, reservation trends, and seasonal indicators.  
The goal is to build reliable time series models to understand call volume fluctuations and measure the impact of reservations and special days on demand.

---

## 📊 Dataset

**Sources:**
- `case_data_calls.csv` – Daily call volume data
- `case_data_reservations.csv` – Reservation data with potential impact on call volumes

**Time Period:**
- January 1, 2013 – February 29, 2016 (3+ years of daily data)

**Key Features:**
- Date (day-month-year)
- Calls received daily
- Reservation counts (total and 2 months in advance)
- Binary indicators for summer break, Christmas break, and special holidays
- Weekday encoded as integer and name

---

## 🎯 Objectives
- Clean and preprocess time series and related features
- Explore relationships between call volumes, reservations, and seasonal patterns
- Forecast daily call volumes
- Evaluate performance using RMSE and cross-validation
- Analyze holiday and special day impacts on call demand

---

## 🧠 Models & Techniques
- Linear Regression
- Random Forest Regression
- Time-aware train-test splitting
- Cross-validation for stability checks
- Hypothesis testing to measure operational impacts

---

## 📈 Performance Metrics
- **RMSE** – model accuracy
- **Cross-validated RMSE** – generalization
- **T-test** – significance of abandonment rate differences

---

## 🔍 Key Findings
- Linear regression slightly outperformed random forest
- Performance varied across folds — seasonal or behavioral shifts likely
- Significant abandonment rate differences linked to call volume
- Reservations and holidays strongly influence call demand

---

## 📊 Visualizations
- Time series plots (calls vs. reservations)
- Correlation heatmaps
- Train-test split visualizations
- Prediction vs. actual call volume plots

---

## 📂 Folder Structure
call-volume-forecast/
├── data/
│ ├── case_data_calls.csv
│ ├── case_data_reservations.csv
├── notebooks/
│ ├── call_volume_forecast_analysis.ipynb
├── models/
│ ├── saved_models.pkl
├── outputs/
│ ├── visuals/
│ ├── metrics/
├── README.md

---

## 🔮 Future Enhancements
- Use **SARIMA** or **LSTM** for better time series modeling
- Add peak hours, rolling averages, and lag features
- Build automated forecasting pipeline
- Deploy results in real-time dashboards

---

## 👤 Author
**Pragathi Porawakara Arachchige**  
📎 [GitHub Profile](https://github.com/PragathiM007)  
Bellevue University – DSC680 Applied Data Science

---

## 📜 License
This project is licensed under the **PAPM License**.
