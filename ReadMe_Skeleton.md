# Hybrid AI Fraud Detection System

A hybrid banking fraud detection system that combines machine learning, anomaly detection, and explainable AI techniques to identify suspicious financial transactions.

---

## Project Overview

This project was designed as a prototype of a real-world banking fraud detection architecture.

The system combines:

- XGBoost fraud classification
- Autoencoder anomaly detection
- Hybrid risk scoring
- SHAP explainability

The goal of the project is to simulate how modern financial institutions detect fraudulent transactions using layered AI systems.

---

# Architecture

```text
Transaction Data
       ↓
Preprocessing
       ↓
XGBoost Fraud Classifier
       ↓
Autoencoder Anomaly Detector
       ↓
Hybrid Risk Engine
       ↓
SHAP Explainability
       ↓
Fraud Decision
```

---

# Technologies Used

- Python
- XGBoost
- TensorFlow / Keras
- SHAP
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Google Colab

---

# Features

## XGBoost Fraud Detection

Main supervised machine learning model used for transaction fraud classification.

---

## Autoencoder Anomaly Detection

Deep learning anomaly detection model trained only on normal transactions to identify unusual behavior patterns.

---

## Hybrid Risk Scoring

Final fraud score generated using both:
- XGBoost probability
- Autoencoder reconstruction anomaly score

Formula used:

```python
final_risk_score = (
    0.7 * xgb_scores +
    0.3 * reconstruction_norm
)
```

---

# Model Performance

## XGBoost Results

- ROC-AUC: 0.983
- Precision: 0.577
- Recall: 0.877
- F1-score: 0.696

---

## Hybrid System Results

- Precision: 0.70
- Recall: 0.87
- F1-score: 0.78

The hybrid system reduced false positives while maintaining strong fraud detection capability.

---

# Explainable AI

SHAP explainability was integrated to interpret model decisions and identify the most influential transaction features.

Top important features:
- V4
- V14
- V12
- V10

---

# Visualizations

## SHAP Summary Plot

Shows global feature impact on fraud predictions.

## SHAP Feature Importance

Displays the most influential transaction features.

## SHAP Force Plot

Provides local explanation for individual suspicious transactions.

## SHAP Waterfall Plot

Shows how each feature contributed to the final fraud score.

---

# Dataset

Dataset used:
Credit Card Fraud Detection Dataset

The dataset contains anonymized credit card transactions labeled as:
- Normal transaction
- Fraudulent transaction

---

# Future Improvements

- FastAPI fraud prediction API
- Streamlit dashboard
- Real-time fraud monitoring
- Docker deployment
- PostgreSQL integration
- Transaction history analysis
- LSTM behavioral modeling

---

# Project Goal

The purpose of this project is to demonstrate:
- machine learning engineering
- anomaly detection systems
- hybrid AI architecture
- explainable AI in banking
- fraud detection pipelines

---

# Author

Ramazan Meirambekuly
AI Student | Machine Learning Enthusiast | Future ML Engineer
