# 📈 Stock Price Analysis with Numerical Methods

## 🧮 Numerical Analysis - 2025 Coursework

This repository contains the implementation and report for the 2025 Numerical Analysis programming assignment at the Department of Electrical and Computer Engineering, Aristotle University of Thessaloniki.

**Authors**  
- Παναγιώτης Παπαδόπουλος (AEM: 10697)  
- Βασίλειος Κουδούνης (AEM: 10739)  
**Submission Date:** 31/05/2025

---

## 📂 Contents

- `Εργασία 2025 - Αριθμητική Ανάλυση.ipynb`: Python notebook with full implementation using `yfinance`, NumPy, and Matplotlib.
- `Αριθμητική_Ανάλυση - αναφορά.pdf`: Detailed PDF report with explanations, results, graphs, and theoretical justifications.
- `project_NA_2025.pdf`: The original assignment specification (in Greek).

---

## 📊 Project Overview

The goal of this project is to analyze and predict stock prices using historical data from Yahoo Finance through various **numerical methods**, including:

### 1. **Data Collection**
- Stock: **AAPL (Apple Inc.)**
- Sampling: Every 30 minutes for 5 consecutive trading days
- Source: Yahoo Finance API (`yfinance`)

### 2. **Polynomial Least Squares Fitting**
- Fitting 1st, 2nd, and 3rd-degree polynomials
- Train/Test split: 80% / 20%
- Evaluation: MAE and MSE for each model
- Discussion on **overfitting**, error comparison, and model selection

### 3. **Next-Day Forecasting**
- Forecasting the next 24 hours (48 intervals) using the best-fit model
- Visualization of extrapolated trends and stability evaluation

### 4. **Numerical Integration**
- Estimating the **average stock price** using:
  - Trapezoidal Rule
  - Simpson's Rule
- Comparison of step sizes (h = 1 to 6) and polynomial degrees

### 5. **Anomaly Detection**
- Segmenting time series into windows of 5 points
- Applying:
  - Aitken-Neville interpolation
  - Newton’s divided differences
- Dynamic anomaly threshold:  
  `δ = 0.05 × Range + 0.5 × σ`
- Visualization of predicted vs. actual values and flagged anomalies

---

## 🧠 Key Learning Points

- Application of **interpolation and integration** techniques in real-world financial data
- Trade-offs in **model complexity** and **prediction stability**
- Use of **adaptive thresholds** for anomaly detection based on data volatility
- Importance of **visualization** and **error analysis** in model validation

---

## 🛠 Technologies Used

- Python 3.x
- yfinance
- NumPy
- Matplotlib
- pandas
- Jupyter Notebook

---

## 📌 How to Run

1. Install the required packages:
   ```bash
   pip install yfinance numpy matplotlib pandas
   ```
2.	Open the Jupyter Notebook:
    ```bash
    jupyter notebook "Εργασία 2025 - Αριθμητική Ανάλυση.ipynb"
    ```
3.	Run each cell sequentially to reproduce the analysis and plots.

## 📎 License

This project is intended for academic purposes only and follows the guidelines of the Numerical Analysis course at AUTH.