# Market-Interaction-Based-Company-Performance-Predictor
# Stock Market Behaviour Analysis using K-Means Clustering

## Project Overview
This project applies **unsupervised machine learning (K-Means clustering)** to analyze and group NIFTY-50 companies based on their **price movement, trading activity, and return characteristics**.  
The objective is to identify **behavioural similarities between companies** and understand how related stocks move together.

---

## Objectives
- Identify relationships between companies using behavioural similarity
- Understand how related companies influence each other’s performance
- Group stocks based on trading activity and return patterns

---

## Dataset Description
The dataset contains daily market-related features:
- Open, High, Low, Last Traded Price (LTP)
- Absolute Change and Percentage Change
- Trading Volume and Turnover
- 30-day and 365-day percentage change
- 52-week High and Low

Each row represents a **company**, not time-series data.

---

## Data Preprocessing
- Checked for missing values across numerical features
- Applied **mean imputation** to handle missing data
- Selected relevant numerical columns for clustering
- Standardized features to ensure fair distance computation

---

## Clustering Methodology
- Used **K-Means clustering** to group companies
- Determined optimal clusters using the **Elbow Method**
- Selected **K = 3** for interpretability
- Assigned each company to a cluster

---

## Cluster Interpretation

### Cluster 0 – Stable Stocks
- Low price volatility
- Lower trading volume and turnover
- Moderate long-term growth  

These stocks exhibit stable behaviour.

---

### Cluster 1 – High Growth & High Activity Stocks
- High trading volume and turnover
- Strong long-term returns
- Short-term fluctuations present  

These stocks attract active trading and investor attention.

---

### Cluster 2 – Volatile / Cyclical Stocks
- Higher daily price changes
- Moderate long-term performance
- Sensitive to market conditions  

These stocks are more reactive to macroeconomic factors.

---

## Key Insights
- Stocks within the same cluster show similar behaviour
- Clustering captures hidden relationships beyond sector labels
- Useful for relative performance and risk analysis

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## Future Scope
- Add time-series based clustering
- Use PCA for visualization
- Build cluster-based trading signals

