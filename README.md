# Binance Trade Data Analysis

## 📌 Project Overview
This project involves analyzing historical trade data from multiple Binance accounts over a 90-day period. The objective is to calculate key financial metrics for each account, rank them, and identify the best-performing portfolios.

## 📊 Key Metrics Calculated
The following metrics were computed for each account:
- **ROI (Return on Investment)**
- **PnL (Profit and Loss)**
- **Sharpe Ratio**
- **MDD (Maximum Drawdown)**
- **Win Rate**
- **Win Positions**
- **Total Positions**

## 📂 Dataset Information
The dataset contains:
- **Port_IDs**: Unique identifiers for accounts
- **Trade_History**: Details of trades, including timestamp, asset, side (BUY/SELL), price, and more

## 🔄 Steps in Analysis
### 1️⃣ Data Exploration & Cleaning
- Loaded and inspected dataset
- Handled missing values and inconsistencies

### 2️⃣ Feature Engineering
- Extracted key financial indicators
- Mapped trade actions using `side` and `positionSide`
- Classified trades into categories (e.g., `long_open`, `long_close`)

### 3️⃣ Ranking Algorithm
- Developed a scoring system with weighted metrics
- Ranked accounts based on profitability, consistency, and risk-adjusted returns

### 4️⃣ Visualization
- Generated plots to analyze trade distribution, PnL trends, and risk exposure

### 5️⃣ Reporting & Summary
- Identified:
  - **Best Performing Portfolios** 📈
  - **Risky Portfolios** 📉
  - **Consistent Performers** 📊
- Created CSV of results and documented findings

## 📑 Final Results
**Best Performing Portfolios:**
| Port_IDs      | Total_PnL | Win_Positions | Total_Positions | Win_Rate |
|--------------|-----------|--------------|-----------------|---------|
| 4.020000e+18 | 23.2      | 1            | 1               | 100%    |
| 4.020000e+18 | 6.9       | 1            | 1               | 100%    |
| 4.020000e+18 | 4.7       | 1            | 1               | 100%    |
| 4.021243e+18 | 0.8       | 1            | 1               | 100%    |

**Risky Portfolios:**
| Port_IDs      | Total_PnL | Win_Positions | Total_Positions | Win_Rate |
|--------------|-----------|--------------|-----------------|---------|
| 4.022642e+18 | 0.0       | 0            | 1               | 0%      |


