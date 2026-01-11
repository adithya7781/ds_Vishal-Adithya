# Trader Behavior vs Market Sentiment Analysis

This project analyzes how Bitcoin trader behavior changes under different market sentiment regimes (Fear, Neutral, Greed, Extreme Greed) using real trading data from Hyperliquid.

## Project Structure

ds_Vishal Adithya/
├── notebook_1.ipynb
├── csv_files/
│   └── sample_dataset.csv
├── outputs/
│   ├── pnl.png
│   ├── risk.png
│   └── winrate.png
├── ds_report.pdf
└── README.md

## Data Sources

- Bitcoin Fear & Greed Index  
- Hyperliquid Historical Trading Data

The original processed dataset contains over 180,000 trades and exceeds GitHub’s file size limits.  
A 5,000-row representative sample is provided in this repository for reference.

The full dataset is available via Google Drive 
Link - https://drive.google.com/file/d/1BFIeI_y5qmMl1fVHWkXSyr3SqEwd58m9/view?usp=drive_link

## Methodology

1. Converted Unix timestamps to calendar dates.
2. Merged trading data with market sentiment by date.
3. Computed key metrics:
   - Profitability (Closed PnL)
   - Risk (Trade size in USD)
   - Win rate (PnL > 0)
4. Compared trader behavior across Fear, Neutral, Greed, and Extreme Greed.

## Key Insights

- Extreme Greed shows the highest win rate but also the highest risk exposure.
- Fear markets show emotional trading with high exposure and lower accuracy.
- Neutral markets are the worst for active trading due to lack of clear direction.
- Greed periods generate the highest average profitability.

## Files

- `notebook_1.ipynb` – Google Colab analysis
- `ds_report.pdf` – Final summarized report
- `outputs/` – Charts used in the report
- `csv_files/sample_dataset.csv` – Sample processed data

Open `notebook_1.ipynb` in Google Colab and ensure Drive is mounted.  
All paths point to `/content/drive/MyDrive/ds_Vishal Adithya/`.
