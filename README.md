# Smart-City-Traffic-Volume-Prediction
Time-series traffic volume prediction at urban junctions using feature engineering and Random Forest regression.
<br>
📌 Problem Statement

Urban traffic congestion is a major challenge for smart cities.
Accurate short-term traffic volume prediction helps city planners optimize:

traffic signal control

congestion management

infrastructure planning

This project focuses on predicting hourly traffic volume at city junctions
using historical time-series data.

📊 Dataset

Training Data: ~48,000 hourly records (2015–2017)

Features: DateTime, Junction ID, Vehicles

Target: Vehicles (traffic volume)

Data includes 4 junctions with distinct traffic behavior.

🧠 Approach
1. Exploratory Data Analysis (EDA)

Hourly traffic patterns

Weekday vs weekend comparison

Junction-wise trends

Seasonal and temporal behavior

2. Feature Engineering

Time-based features:

Hour

Day of Week

Month

Weekend indicator

Junction-specific lag features:

Vehicles (lag 1 hour)

Vehicles (lag 24 hours)

3. Model Development

Baseline: Linear Regression (R² ≈ 0.50)

Advanced Model: Random Forest Regressor

Time-aware train–test split to avoid data leakage

4. Model Diagnostics

Actual vs Predicted visualization

Residual analysis

Feature importance analysis

📈 Results
Metric	Value
R² Score	~0.70
MAE	~3.1
RMSE	~5.5

Key Insight:
Recent traffic history (lag features) is the strongest predictor of traffic volume.

🏁 Conclusion

Lag-based features significantly improve time-series regression performance

Junction-specific modeling captures local traffic dynamics effectively

Random Forest balances performance and interpretability for this task

This project demonstrates a full ML lifecycle, from EDA to deployment-ready predictions.
