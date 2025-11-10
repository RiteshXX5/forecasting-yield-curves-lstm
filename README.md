
# Forecasting Yield Curves Using LSTM: An AI Approach with ARIMA Benchmark

## 📘 Overview
This project explores the use of **Long Short-Term Memory (LSTM)** networks to forecast U.S. Treasury yield curves and compares its performance with a traditional **ARIMA** model.  
The project demonstrates how AI can capture nonlinear dependencies and temporal patterns in financial time-series data better than conventional econometric methods.

---

## 🧩 Objectives
- Collect and preprocess U.S. Treasury yield data (3M, 2Y, 5Y, 10Y)
- Train an LSTM model to forecast 10-Year yield using short- and medium-term maturities
- Benchmark the performance against an ARIMA model
- Evaluate models using RMSE and MAPE metrics

---

## 🧠 Methodology
1. **Data Source:** Federal Reserve Economic Data (FRED)
2. **Preprocessing:** Handle missing values, apply MinMax scaling, 30-day lookback window
3. **Models:**
   - **LSTM:** Two hidden layers with dropout and Adam optimizer
   - **ARIMA:** (5,1,0) univariate model as baseline
4. **Evaluation:** RMSE and MAPE on test data

---

## ⚙️ Tech Stack
- Python, TensorFlow, Scikit-learn, Pandas, NumPy, Matplotlib
- Google Colab for training
- FRED dataset for U.S. Treasury yields

---

## 📊 Results
| Model | RMSE | MAPE |
|--------|------|------|
| **LSTM** | 0.0463 | 0.0498 |
| **ARIMA** | 0.4241 | 0.0841 |

LSTM outperformed ARIMA, capturing nonlinear dynamics and multi-maturity dependencies effectively.

---

## 📈 Visualizations
Include in `results/`:
- Actual vs Predicted Yields (LSTM)
- Actual vs Predicted Yields (ARIMA)

---

## 🚀 Future Work
- Try advanced models like **Transformers** or **Temporal Convolutional Networks (TCNs)**
- Add macroeconomic variables (GDP, inflation)
- Incorporate financial sentiment data for better market context

---

## 📜 Credits
Developed by **Ritesh Kashyap**  
Under the supervision of **ZeTheta Algorithms Pvt. Ltd.**  
Department of Information Technology, J. K. College of Science and Commerce

---

## 📚 References
- Diebold & Li (2006). *Forecasting the Term Structure of Government Bond Yields.*
- Hochreiter & Schmidhuber (1997). *Long Short-Term Memory.*
- Siami-Namini et al. (2018). *A Comparison of ARIMA and LSTM in Forecasting Time Series.*

---
