# DEPI-Project

##📊 Bitcoin Data Analysis & Feature Engineering
This project focuses on analyzing historical data of Bitcoin from 2018 to 2025. The goal is to build a clean, feature-rich dataset that captures market behavior and can be used for data analysis, machine learning, and dashboard visualization.

##🚀 Project Overview
In this project, I developed a complete data preprocessing pipeline that:

Combines multiple timeframes (15m, 1h, 4h, 1d)
Cleans and validates the dataset
Engineers advanced financial features
Prepares a structured dataset for analysis and modeling
##📂 Dataset
Source: Kaggle Bitcoin Historical Dataset

Time Period: 2018 – 2025

Timeframes:

15 Minutes
1 Hour
4 Hours
1 Day
##🧹 Data Preprocessing
Key preprocessing steps:

Merged multiple datasets into one unified DataFrame

Converted time columns to datetime format (UTC)

Sorted data chronologically

Removed missing values and invalid records

Eliminated duplicates based on (Open time, timeframe)

Extracted time-based features:

Year
Month
Day
Quarter
##⚙️ Feature Engineering
📈 Price Features
price_change → Close - Open
return_pct → Price return percentage
volatility → High - Low
📊 Trend Features
trend_direction → Uptrend / Downtrend
trend_length → Consecutive trend duration
trend_strength → Price movement weighted by volume
💰 Volume & Market Activity
Buy/Sell volume
Buy/Sell ratios
Order flow
Capital flow
Trade activity
🚨 Market Behavior Signals
High volatility
Compression (low activity periods)
Volume spikes
Overheating (strong bullish pressure)
Whale activity
📉 Technical Indicators
Support & Resistance levels
Breakout detection (up/down) using rolling windows
🧠 Output
Final dataset:

bitcoin_kpis.csv
This dataset is ready for:

Data analysis
Machine learning models
Time-series forecasting
Trading strategy development
📊 Dashboard (Coming Soon)
An interactive dashboard will be added to visualize:

Price trends
Volume behavior
Market signals
Breakout events
Tools that may be used:

Power BI / Tableau
Python (Plotly / Dash / Streamlit)
##🛠️ Technologies Used
Python
Pandas
NumPy
KaggleHub
##📌 Future Work
Build predictive models (price movement / trend prediction)
Add technical indicators (RSI, MACD, Moving Averages)
Develop an interactive dashboard
Deploy the project
##🙌 Authors
Yasmin Abdelhamid
Samira Samir
Sama Mohamed
Rewaa Sabry
