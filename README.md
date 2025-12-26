# 📈 Quantitative Trading Strategy & ML Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Libraries](https://img.shields.io/badge/Library-Pandas%20%7C%20NumPy%20%7C%20Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

### 📌 Project Overview
This project implements a full-stack quantitative analysis pipeline for financial time-series data (AAPL). It combines traditional algorithmic trading strategies (Momentum & Mean Reversion) with modern Machine Learning techniques to predict future price movements.

The goal was to engineer robust features from raw market data, backtest trading logic against a "Buy & Hold" benchmark, and validatethe statistical significance of the results.

---

### 📊 Performance Visualizations
*Below is the output of the analysis, showing the strategy performance, volatility bands, risk drawdown, and ML model ROC curve.*

![App Screenshot](Screenshot%201.png)

---

### 🛠️ Key Features

#### 1. Data Pipeline & Processing
* **Automated Extraction:** Fetched multi-year OHLCV data using `yfinance`.
* **Feature Engineering:** Calculated technical indicators including Simple Moving Averages (50/200 SMA), Bollinger Bands, and Rolling Volatility.
* **Statistical Validation:** Applied **Augmented Dickey-Fuller (ADF)** tests to ensure stationarity of time-series data before modeling.

#### 2. Algorithmic Trading Strategy
* **Momentum Logic:** Implemented a Golden Cross strategy (Long when SMA_50 > SMA_200).
* **Backtesting Engine:** Simulated 4 years of trading to calculate key risk metrics:
    * **Sharpe Ratio:** Measured risk-adjusted returns.
    * **Max Drawdown:** Quantified downside risk and recovery periods.

#### 3. Machine Learning Forecast
* **Model:** Random Forest Classifier (Ensemble Learning).
* **Target:** Predict if the next day's closing price will be **Higher (1)** or **Lower (0)**.
* **Performance:** Evaluated using Confusion Matrix and ROC-AUC curves to minimize false positives.

---

### 📉 Results Snapshot

| Metric | Result | Description |
| :--- | :--- | :--- |
| **Sharpe Ratio** | *[Insert Your Value]* | >1.0 indicates good risk-adjusted returns |
| **Max Drawdown** | *[Insert Your Value]* | Maximum observed loss from peak |
| **ML Accuracy** | *[Insert Your Value]* | Prediction accuracy on unseen test data |

---

### 💻 Technologies Used
* **Analysis:** Python, Pandas, NumPy
* **Machine Learning:** Scikit-Learn (Random Forest)
* **Visualization:** Matplotlib, Seaborn
* **Financial Data:** Yahoo Finance API (`yfinance`)

### 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/yourusername/Quantitative-Trading-Strategy.git](https://github.com/yourusername/Quantitative-Trading-Strategy.git)
    ```
2.  Install dependencies:
    ```bash
    pip install yfinance pandas numpy matplotlib scikit-learn seaborn statsmodels
    ```
3.  Run the notebook or script:
    ```bash
    python quant_strategy.py
    ```

---

### 📬 Contact
**[Your Name]** *Aspiring Software Engineer & Data Analyst* [Your LinkedIn Profile Link] | [Your Email Address]
