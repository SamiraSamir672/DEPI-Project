# 📈 Bitcoin Market Analysis & Buy Signal Prediction

![Uploading image.png…]()


## 📌 Project Overview

This project is an end-to-end Business Intelligence and Machine Learning solution for analyzing Bitcoin market behavior and predicting Buy Signals across multiple timeframes.

The solution combines data engineering, machine learning, Microsoft Fabric, and Power BI to build a complete analytics pipeline using the Medallion Architecture.

The project analyzes historical Bitcoin market data from **2018 to 2025** across four different timeframes:

- 15 Minutes
- 1 Hour
- 4 Hours
- 1 Day

---

# 🎯 Objectives

- Analyze Bitcoin market trends.
- Detect market volatility and trading behavior.
- Identify whale activities.
- Predict future Buy Signals using Machine Learning.
- Build interactive dashboards for decision making.
- Automate the data pipeline using Microsoft Fabric.

---

# 🏗 Project Architecture

The project follows the **Medallion Architecture**.

```
Raw Data
    │
    ▼
Bronze Layer
    │
    ▼
Silver Layer
    │
    ▼
Gold Layer
    │
    ▼
Machine Learning
    │
    ▼
Power BI Dashboard
```

---

# 📂 Dataset

Historical Bitcoin OHLCV market data

Timeframes:

- 15m
- 1h
- 4h
- 1d

Main columns include:

- Open
- High
- Low
- Close
- Volume
- Number of Trades
- Taker Buy Volume

---

# ⚙ Data Engineering

The data engineering process includes:

- Cleaning missing values
- Removing duplicates
- Creating calculated columns
- Feature Engineering
- Data transformation
- Data validation

---

# 🥇 Bronze Layer

The Bronze layer stores the raw Bitcoin datasets exactly as received.

Tasks:

- Download dataset
- Load CSV files
- Save raw files into OneLake Bronze

---

# 🥈 Silver Layer

The Silver layer performs data cleaning and feature engineering.

Features created include:

- Price Change
- Return %
- Volatility
- Buy Volume
- Sell Volume
- Buy Ratio
- Sell Ratio
- Order Flow
- Capital Flow
- Liquidity
- Trend Direction
- Trend Length
- Trend Strength
- Volume Spike
- High Volatility
- Compression
- Breakout Detection
- Support
- Resistance
- Whale Activity

---

# 🥇 Gold Layer

The Gold layer creates the final analytical model.

Tables include:

### Fact Table

- fact_bitcoin_market

### Dimension Tables

- dim_date
- dim_timeframe

### Machine Learning Tables

- ml_predictions
- ml_metrics
- confusion_matrix
- feature_importance

---

# 🤖 Machine Learning

The ML model predicts whether the Bitcoin price is likely to generate a Buy Signal.

Target:

```
1 → Buy Signal

0 → No Buy Signal
```

Model Used:

- Random Forest Classifier

Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

Prediction confidence is also calculated for every timeframe.

---

# 📊 Power BI Dashboard

The dashboard provides interactive analysis including:

## Market Overview

- Price Trend
- Market Performance
- Trading Volume
- Returns

---

## Liquidity Dashboard

- Liquidity Score
- Order Flow
- Buy vs Sell Ratio
- Capital Flow

---

## Support & Resistance

- Support Levels
- Resistance Levels
- Breakout Detection

---

## Trend Analysis

- Trend Direction
- Trend Length
- Trend Strength

---

## Trader Activity & Whale Watch

- Total Trades
- Whale Flags
- Trade Intensity
- Volatility Clusters

---

## Machine Learning Dashboard

- Model Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Feature Importance
- Live Buy Signal
- Prediction Confidence

---

# ☁ Microsoft Fabric

This project is implemented using Microsoft Fabric.

Components:

- OneLake
- Lakehouse
- Notebook
- Data Pipeline
- Semantic Model
- Power BI Report

The pipeline automatically executes:

Bronze Notebook

↓

Silver Notebook

↓

Gold Notebook

↓

Machine Learning Notebook

↓

Semantic Model Refresh

↓

Power BI Dashboard Refresh

---

# 🛠 Technologies Used

Programming

- Python

Libraries

- Pandas
- NumPy
- Scikit-Learn
- Matplotlib

Cloud

- Microsoft Fabric
- OneLake
- Lakehouse

Business Intelligence

- Power BI

Machine Learning

- Random Forest

---

# 📁 Repository Structure

```
Bitcoin_Project

│
├── Bronze_Notebook
├── Silver_Notebook
├── Gold_Notebook
├── ML_Notebook
│
├── PowerBI
│     └── Dashboard.pbix
│
├── Fabric_Links
│
├── README.md
```

---

# 📷 Dashboard Preview

(Add dashboard screenshots here)

Example:

```
/images/dashboard1.png
/images/dashboard2.png
```

---

# 🔗 Fabric Links

See:

```
Fabric_Links/Fabric Links.md
```

---

# 👩‍💻 Developed By

- Yasmin Abdelhamid
- Sama Mohamed
- Rewaa Mostafa
- Samira Samir

DEPI Graduation Project

Data Analysis & Machine Learning

2026
