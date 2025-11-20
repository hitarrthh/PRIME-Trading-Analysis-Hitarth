# 📊 Market Sentiment & Trader Behavior Analysis  
### PRIME Trading Data Science Task  
**Candidate:** Hitarth Bhatt  
**Date:** November 2025  

---

## 🔗 Important Links

- **Google Colab Notebook**  
  👉 [Open in Colab](<YOUR_COLAB_LINK_HERE>)

- **Final PDF Report**  
  Included in `/report/ds_report.pdf`

---

# 📁 Project Structure

```
ds_Hitarth_Bhatt/
│
├── notebook/
│   └── PRIME_TRADE_TASK_HITARTH_BHATT.ipynb
│
├── csv_files/
│   ├── historical_data.csv
│   ├── fear_greed_index.csv
│   ├── summary_by_sentiment.csv
│   ├── correlation_matrix.csv
│   ├── t_test_results.csv
│   └── lag_correlation.csv
│
├── outputs/
│   ├── ts_pnl.png
│   ├── ts_volume.png
│   ├── ts_bias.png
│   ├── ts_tradecount.png
│   ├── rel_pnl_scatter.png
│   ├── bar_pnl.png
│   ├── bar_volume.png
│   ├── bar_bias.png
│   ├── box_pnl.png
│   └── corr_heatmap.png
│
├── report/
│   └── ds_report.pdf
│
├── README.md
└── requirements.txt
```

---

## 🧠 Project Overview

This project analyzes how trader behavior—profitability, risk, volume, directional bias and activity—aligns or diverges from market sentiment. Using aggregated trading data and the Fear-&-Greed Index, the aim is to uncover actionable behavioral trends for smarter trading strategies.

---

## 🧮 Key Insights (Summary)

- **Fear’s Premium** — Higher average PnL during fear states; however, risk (PnL volatility) is also highest.  
- **Liquidity Behavior** — Volume spikes during extreme sentiment states (both fear & greed).  
- **Directional Bias** — Traders lean *short* in fear and *long* in greed, reflecting alignment with sentiment.  
- **Pro-Cyclic Activity** — High trade count and volume during emotionally extreme days rather than neutral ones.  
- **Statistical Significance** — Fear vs. Greed states show significant differences in PnL, volume, win-rate, and bias.

---

## 🛠 Methodology

**Data Integration**  
- Merged trading history with sentiment index on daily basis.  
- Computed daily features: total PnL, PnL std, volume, trade count, long/short bias.

**Statistical Analysis**  
- Summary statistics by sentiment class.  
- Correlation matrix and heatmap between key metrics and sentiment.  
- Welch t-tests comparing “Fear” vs “Greed” states.  
- Scatter and regression for PnL vs sentiment.

**Visualization**  
- Time-series plots of key metrics.  
- Barplots showing means per sentiment.  
- Boxplots showing distributions.  
- Heatmap showing correlation structure.

---

## 📊 Results & Outputs

### CSV Files  
Located in `csv_files/`: summary_by_sentiment.csv, correlation_matrix.csv, t_test_results.csv, merged_full_dataset.csv

### Plot Files  
Located in `outputs/`: time-series, barplots, boxplots, scatter, heatmap.

### Report  
Final analysis and conclusions in `report/ds_report.pdf`.

---

## 🎯 How to Run

1. Open the [Colab Notebook]([<YOUR_COLAB_LINK_HERE>](https://colab.research.google.com/drive/1d68x_YV3KpVNMExpLS-aOnzyuHpsDs8j?usp=sharing))  
2. Upload `historical_data.csv` and `fear_greed_index.csv` 
3. Run all cells — this will regenerate all CSVs and plots  
4. Inspect results in `csv_files/` and `outputs/`


---

*Thank you for your time and consideration.*  
