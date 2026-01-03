# Web3 Trading Behavior vs Market Sentiment Analysis

This repository contains my data science internship assignment analyzing how trader behavior varies under different Bitcoin market sentiment conditions, specifically **Fear** and **Greed**.

The objective of this project is to understand how market psychology influences trading behavior in terms of capital allocation, risk intensity, and profitability using real world trading data.

---

## 📌 Problem Statement

Cryptocurrency markets are highly influenced by collective sentiment. This project explores the relationship between **market sentiment (Fear vs Greed)** and **trader behavior**, answering questions such as:

- Do traders allocate more capital during Greed periods?
- Are losses more severe during Fear dominated markets?
- Does increased trading activity translate into higher profitability?
- How does sentiment influence risk taking behavior?

---

## 📂 Repository Structure

```

ds_insha/
│
├── notebook_1.ipynb          # Complete analysis notebook (Google Colab compatible)
│
├── csv_files/
│   └── merged_clean_data.csv # Cleaned and merged dataset used for analysis
│
├── outputs/
│   ├── trade_value_by_sentiment.png
│   ├── abs_pnl_by_sentiment.png
│
├── ds_report.pdf             # Final summarized report with insights and conclusions
│
└── README.md                 # Project overview and instructions

```

---

## 📊 Datasets Used

### 1. Bitcoin Fear & Greed Index
- Provides **daily market sentiment classification**
- Values: `Fear`, `Greed`
- Used as a contextual indicator of overall market psychology

### 2. Historical Trader Data (Hyperliquid)
- Contains **individual trading events**
- Includes trade size, execution price, profit/loss, timestamps, and fees
- Each row represents a **trading event**, not necessarily a completed trade

> Note: The dataset does not include explicit leverage information. Risk behavior is therefore evaluated using capital exposure and profit/loss magnitude as proxy measures.

---

## 🧠 Methodology Overview

The analysis is structured into five phases:

1. **Phase 1 – Data Understanding**  
   Understanding dataset structure, semantics, and limitations.

2. **Phase 2 – Data Cleaning & Feature Engineering**  
   - Timestamp normalization  
   - Feature creation (trade value, profitability flag, absolute PnL)  
   - Dataset merging based on date  

3. **Phase 3 – Exploratory Data Analysis (EDA)**  
   - Comparison of trader behavior across Fear vs Greed  
   - Distribution based analysis using visualizations  

4. **Phase 4 – Insight Extraction & Interpretation**  
   - Translating observed patterns into behavioral insights  
   - Discussing trading and risk implications  

5. **Phase 5 – Reporting**  
   - Summarizing findings in a professional PDF report  

---

## 🔑 Key Insights

- Traders tend to allocate **higher capital per trade during Greed periods**
- **Loss severity is higher during Fear-dominated markets**
- Increased trading activity during Greed does **not guarantee higher profitability**
- Market sentiment influences **risk behavior more than trade outcomes**

---

## ⚠️ Limitations

- Leverage data is not available in the trading dataset
- Sentiment data is available only at **daily granularity**
- Analysis is **observational**, not causal

These limitations are explicitly acknowledged and incorporated into the analysis design.

---

## 🛠 Tools & Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Google Colab  

---

## 📄 How to View the Analysis

- Open `notebook_1.ipynb` in **Google Colab**  
- View saved plots inside the `outputs/` directory  
- Read summarized insights in `ds_report.pdf`

---

## 👤 Author

**Insha**  
Data Science Internship Applicant  
Web3 Trading Analytics

---

## 📬 Notes

This project is submitted as part of the internship evaluation process.  
All analysis follows the standardized submission format and emphasizes clarity, correctness, and real-world applicability.
```