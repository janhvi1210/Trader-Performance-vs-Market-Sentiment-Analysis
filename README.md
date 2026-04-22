
# Trader Performance vs Market Sentiment

## 📌 Overview
This project analyzes how market sentiment (Fear vs Greed) influences trader behavior and performance on Hyperliquid.

The goal is to uncover patterns that can help design smarter trading strategies based on sentiment-driven market conditions.

---

## 🎯 Objectives
- Compare trader performance across Fear vs Greed regimes  
- Analyze behavioral changes (trading frequency, leverage, position size)  
- Segment traders based on behavior and performance  
- Propose actionable trading strategies  

---

## 📂 Dataset
The analysis uses two datasets:

1. **Bitcoin Market Sentiment**
   - Columns: Date, Classification (Fear / Greed)

2. **Trader Data (Hyperliquid)**
   - Includes: account, trade size, side, timestamp, closedPnL, leverage, etc.

---

## ⚙️ Methodology

### 1. Data Preparation
- Removed duplicates and checked missing values  
- Converted timestamps to datetime format  
- Aggregated trade-level data into **daily trader-level metrics**  
- Merged datasets on date  

### 2. Feature Engineering
Created key metrics:
- Daily PnL per trader  
- Win rate  
- Average trade size  
- Trades per day  
- Leverage (proxy)  
- Long/Short ratio  

---

## 📊 Analysis

### 🔹 Performance vs Sentiment
- Fear regimes show higher PnL volatility and extreme outcomes  
- Greed regimes show more stable and consistent performance  

### 🔹 Behavioral Changes
- Trade frequency increases significantly during Fear periods  
- Indicates reactive or emotion-driven trading  
- Leverage and position sizes vary across sentiment regimes  

---

## 👥 Trader Segmentation

### 1. High vs Low Leverage Traders
- High-leverage traders experience larger gains and losses  
- More sensitive to market volatility  

### 2. Frequent vs Infrequent Traders
- Frequent traders tend to overtrade during Fear  
- Lower consistency in performance  

### 3. Consistent vs Inconsistent Traders
- Consistent traders maintain stable performance  
- Less impacted by sentiment changes  

---

## 🔑 Key Insights
- Market sentiment impacts **behavior more than raw profitability**  
- Fear leads to **higher volatility and aggressive trading**  
- Stable trading strategies outperform reactive behavior  

---

## 🚀 Strategy Recommendations

### 1. Risk Control During Fear
- Reduce leverage  
- Avoid excessive trading  
- Focus on capital preservation  

### 2. Controlled Trading During Greed
- Maintain moderate leverage  
- Avoid overtrading due to overconfidence  

---

## ⚠️ Limitations
- Daily aggregation may hide intra-day patterns  
- External market factors not included  
- No transaction cost modeling  

---

## 🛠️ How to Run

1. Clone the repository  
2. Place datasets inside the `data/` folder  
3. Open and run:
