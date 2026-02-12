
# 📈 NIFTY 50 -Stock Price prediction

## 📌 Project Overview
This project focuses on predicting the **High price of the NIFTY 50 index** using historical market data.  
Multiple Machine Learning and Deep Learning models are implemented and compared to evaluate their effectiveness in time-series forecasting.

The study investigates how different **lookback windows (30, 60, 90 days)** influence model performance and identifies the most suitable architecture for financial prediction.

---

## 🎯 Assignment Objective
Build and evaluate the following models for predicting the **'High' column**:

### Models Used:
- KNN (K-Nearest Neighbors Regressor)
- Simple RNN (Recurrent Neural Network)
- GRU (Gated Recurrent Unit)
- LSTM (Long Short-Term Memory)
- Bidirectional LSTM

### Time Windows (Input Sequence Length):
- 30 Days
- 60 Days
- 90 Days

### Training Requirement:
All Deep Learning models were trained for **50 epochs**.

### Evaluation Metrics:
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)

---

## 📊 Dataset
The dataset contains historical NIFTY 50 stock data with features like:
- Date
- Open
- High
- Low
- Close
- Volume

For this project, we focus specifically on predicting the **High price** using past historical values.

---

## ⚙️ Methodology

1️⃣ Data Preprocessing  
- Sorted data by date  
- Selected **High price** for forecasting  
- Normalized values using MinMaxScaler  

2️⃣ Sequence Creation  
- Converted data into time-series format using sliding windows:
  - 30-day window
  - 60-day window
  - 90-day window

3️⃣ Model Training  
- KNN trained as baseline model  
- Deep Learning models trained for **50 epochs** each  

4️⃣ Evaluation  
Predictions evaluated using:
- MAE → Measures average error  
- RMSE → Penalizes large errors more strongly  

---

## 🤖 Models Explanation

### 🔹 KNN Regressor
Used as a baseline.
Does not understand time dependencies → performed poorly.

### 🔹 RNN
Captures sequential relationships but struggles with long-term memory.

### 🔹 GRU ⭐
Best performing model.
Efficient gating mechanism learns market patterns effectively.

### 🔹 LSTM
Strong time-series model but slightly heavier than GRU.

### 🔹 Bidirectional LSTM
Less suitable for stock prediction since financial data is **forward-looking only**.

---

## 📈 Results Summary

| Model | Window | Performance |
|------|--------|-------------|
KNN | All | Weak baseline |
RNN | Good | Captures sequences |
GRU | ⭐ Best | Lowest MAE & RMSE |
LSTM | Very Good | Slightly heavier |
BiLSTM | Moderate | Not ideal for causal data |

---

## 🔍 Key Insights

✔ Deep Learning models significantly outperform traditional ML models.  
✔ GRU provides the best balance between complexity and performance.  
✔ Financial time-series rely more on **recent history**, making 30–60 day windows highly effective.  
✔ KNN fails to model sequential dependencies.

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-Learn
- TensorFlow / Keras
- Matplotlib / Seaborn

---

## ▶️ How to Run This Project

### Download  Notebook and open in google colab or jupyter Notebook
