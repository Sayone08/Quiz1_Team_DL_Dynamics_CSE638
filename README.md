# 🌧️ Rainfall Forecasting Using Deep Learning

A comparative study of **BiLSTM, BiLSTM-PINN, and Transformer** models for next-day rainfall prediction across weather stations in India.

## 📌 Overview

This project explores daily rainfall forecasting using exploratory data analysis (EDA), feature engineering, and deep-learning-based time-series modelling. The models are evaluated against climatology, persistence, and gradient-boosting baselines using a chronological train-validation-test split.

## 📊 Dataset

- **Source:** https://www.kaggle.com/datasets/ameydilipmorye/indian-rainfall-and-weather-data
- **Original period:** 2015–2025
- **Cleaned dataset:** 597,294 station-day records from 414 stations
- **Input:** 30 days of historical weather data with 21 features
- **Target:** Next-day rainfall in millimetres

## 🧠 Models

- BiLSTM
- BiLSTM-PINN (Physics-Informed BiLSTM)
- Transformer Encoder
- Baselines: Climatology, Persistence, and Gradient Boosting

## 📈 Key Results

| Model | RMSE (mm) | MAE (mm) | R² | Rainy-Day F1 |
|---|---:|---:|---:|---:|
| BiLSTM | 10.521 | 4.072 | 0.365 | 0.809 |
| **BiLSTM-PINN** | **10.491** | 4.070 | **0.369** | 0.809 |
| Transformer | 10.529 | 3.940 | 0.364 | **0.811** |

*Results are from the held-out test set. Neural-model rainfall estimates use validation-based calibration.*

BiLSTM-PINN achieved the lowest RMSE among the neural models, while the Transformer achieved the highest rainy-day F1 score. The performance differences between the neural models were small.

## 🛠️ Technologies

Python · PyTorch · Pandas · NumPy · Scikit-learn · Jupyter Notebook

## 📄 Project Report

The complete project report, including the research methodology, exploratory data analysis, model architectures, detailed results, visualizations, limitations, and references, is available in the repository.

**Report:** `Quiz1_Report_Team_DL_Dynamics.pdf`

