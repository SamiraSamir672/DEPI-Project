🪙 Bitcoin Market Behavior Analysis & Feature Engineering

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-purple.svg)](https://pandas.pydata.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Interactive-orange.svg)](https://plotly.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

🚀 Project Overview
This project focuses on analyzing historical Bitcoin market data to build a clean, feature-rich dataset that captures complex market behaviors. By engineering advanced financial features and processing multiple timeframes, this project bridges the gap between raw trading data and actionable insights for **Data Analysis, Machine Learning, and Interactive Dashboards**.

---

📂 Dataset Architecture
* **Source:** Kaggle Bitcoin Historical Dataset
* **Time Period:** 2018 – 2025
* **Analyzed Timeframes:** `15m` | `1h` | `4h` | `1d`

---

🧹 Data Preprocessing Pipeline
Key preprocessing and validation steps implemented:
* **Data Merging:** Combined multiple timeframe datasets into a unified analytical structure.
* **Temporal Sorting:** Chronologically ordered data and converted timestamps to UTC datetime format.
* **Data Sanitization:** Removed missing values, invalid records, and eliminated duplicates based on `(Open time, timeframe)`.
* **Time Feature Extraction:** Extracted explicit fields for `Year`, `Month`, `Day`, and `Quarter` for macroeconomic analysis.

---

⚙️ Advanced Feature Engineering 

📈 Price & Trend Dynamics
* `price_change`: Measures raw interval movement ($Close - Open$).
* `return_pct`: Percentage return per interval.
* `volatility`: Intraday price range ($High - Low$).
* `trend_direction`: Categorical classification of Bullish/Bearish phases.
* `trend_length`: Counts consecutive intervals moving in the same direction.
* `trend_strength`: Quantifies price movement velocity weighted by volume.

💰 Volume & Liquidity Microstructure
* `Buy/Sell Volume`: Separates taker buy volume from overall volume.
* `buy_ratio` & `sell_ratio`: Proportional dominance of buyers vs. sellers.
* `order_flow`: Net imbalance ($Taker\ Buy - Sell\ Volume$) to anticipate short-term moves.
* `capital_flow`: Total fiat-equivalent volume filtered through the market (Quote Asset Volume in USDT).
* `trade_activity`: Total trade count per interval to gauge active retail/institutional participation.

🚨 Market Behavior & Strategic Signals
* **High Volatility Clusters:** Flags sustained periods of elevated risk.
* **Market Compression:** Detects price tightening and volume drops (low-volatility squeezing before breakouts).
* **Volume Spikes:** Highlights institutional entry or panic events.
* **Market Overheating:** Signals extreme FOMO or overbought conditions.
* **Whale Activity:** Pinpoints high-volume execution via unusually low trade counts.
* **Support & Resistance Levels:** Tracks price rejection boundaries using trailing rolling windows (`Close - Low` and `High - Close`).
* **Breakout Detection:** Real-time flagging of prices exceeding recent historical bounds (`breakout_up` / `breakout_down`).

---

📊 Analytical Dashboards 
The data is visualized across **4 modular interactive dashboards** built to tell a comprehensive market story:

1. **Markert Behavier Analysis:** Explores overall direction, trend duration distribution, and whether price moves are backed by volume.
2. market participation:** Monitors raw liquidity, trade counts, and the aggressive buying/selling order flow imbalance.
3. **Market Risk:** Offers an annual breakdown of market overheating rates, high-volatility frequency, and whale participation.
4. **Support & Market Structure:** Visualizes dynamic price rejection zones and identifies market compression phases preceding major explosive moves.

---

🛠️ Technologies Used
* **Languages & Core:** Python 
* **Data Manipulation:** Pandas, NumPy
* **Data Ingestion:** KaggleHub
* **Visualization:** Matplotlib, Seaborn

---

👥 Authors & Contributors
Meet the team behind this project (DEPI Project Team):

Samira Samir
Yasmin Abdelhamid
Sama Mohamed
Rewaa Sabry
