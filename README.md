# Multi-City-Transit-Delay-Forecasting
End-to-end ML pipeline to forecast transit delays across multiple cities (Seattle &amp; Boston) using GTFS data, engineered temporal/traffic features, and ML models.

This project builds an end-to-end machine learning pipeline to forecast bus delays across multiple cities using real-world transit data. The current implementation covers **Seattle** and **Boston**, and is designed to be easily extended to additional cities.

## 🔍 Project Overview

- **Goal:** Predict route-level and stop-level delays to support better scheduling, rider information, and operations planning.
- **Cities:** Seattle, Boston
- **Data:** GTFS static + real-time feeds (schedules, trips, stop times, vehicle positions, delays)
- **Tech Stack:** Python, Pandas / PySpark, scikit-learn, Jupyter/Databricks, Git

## 🧩 Key Features

- Reusable pipeline that can be parameterized by city
- Feature engineering for:
  - Time-of-day, day-of-week, peak vs off-peak
  - Route-level congestion and historical delay statistics
  - Weather or calendar features (if included)
- Model comparison:
  - Baseline (mean/last value)
  - Linear Regression / Regularized models
  - Tree-based models (Random Forest, Gradient Boosting, etc.)
- Evaluation:
  - RMSE / MAE for regression
  - R² and error distributions per route / time-of-day
