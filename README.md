# 📈 Stock Sentiment Analysis

## 📝 Introduction

This project focuses on **stock sentiment analysis** using news headlines and technical indicators to predict stock price movements. Multiple machine learning models were trained — including **Logistic Regression**, **Random Forest**, **Support Vector Classifier (SVC)**, and a **Convolutional Neural Network (CNN)** — to identify **buy** and **sell** signals. The best-performing model is then used to generate trading signals and evaluate a trading strategy.

---

## 📂 Project Structure

The project is organized into two Jupyter Notebooks:

1. **DataScrapp** → Collects news headlines and stock data.
2. **SentimentAnalysis** → Performs complete analysis, model training, and evaluation.

---

## 🔄 Steps Involved

### 1️⃣ Data Collection

* **News Data** → Scraped using the *New York Times API*, covering **2016–2019**.
* **Stock Data** → Retrieved from the **yfinance** library for the same period.

### 2️⃣ Code Explanation

* **Data Preparation**

  * Import essential libraries (data manipulation, ML, visualization).
  * Load stock price data + news headlines into Pandas DataFrames.
  * Convert date columns → datetime format and merge stock & news data by date.

* **Sentiment Analysis**

  * Apply **VADER** and **TextBlob** to compute sentiment scores.
  * Add sentiment features to the dataset.

* **Technical Indicators**

  * Calculate **Simple Moving Average (SMA)** and **Relative Strength Index (RSI)** using the *ta* library.

* **Feature Engineering & Model Training**

  * Create new features: stock returns, binary labels (upward = 1, downward = 0).
  * Prepare **feature matrix (X)** and **target vector (y)**.
  * Train models: Logistic Regression, Random Forest, SVC, CNN.
  * Evaluate using **cross-validation**.

### 3️⃣ Trading Signals & Backtesting

* Generate trading signals from the **best-performing model**.
* Backtest strategy → simulate portfolio performance.

**Performance Metrics:**

* 📊 Sharpe Ratio
* 📉 Maximum Drawdown
* ✅ Win Ratio

**Visualizations:**

* ROC Curve
* Buy & Sell signals (graphical plots)

---

## 🛠️ Tools & Libraries Used

* **APIs** → New York Times API
* **Libraries** → Pandas, NumPy, VADER, TextBlob, ta, Scikit-learn, TensorFlow
* **Data Source** → yfinance

---

## 👤 Author

**Amey Somvanshi** IIT Roorkee
