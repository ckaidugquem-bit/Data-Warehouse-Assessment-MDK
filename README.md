# S&P 500 Stock Segmentation and Portfolio Analysis
## Data Warehousing and Business Intelligence - Group Coursework (7BUIS010W)
### University of Westminster

## Authors
- Dilara Yigit (21634297)
- Mihai-Catalin Vasile (21171570)
- Kai Dugquem (2170430)

## Project Overview
This project analyses the S&P 500 index to cluster stocks based on 
risk-return metrics and support portfolio diversification decisions. 
The analysis uses daily market data from 2022-2025 to calculate 
Daily Return, Beta and Annual Volatility, and applies agglomerative 
and K-Means clustering to segment stocks into low, medium and high 
risk categories.

## Repository Structure
├── DataWarehouse_CW2.ipynb   # Main Google Colab notebook
├── README.md                 # Project documentation

## Requirements
yfinance
yahoofinancials
pandas
numpy
matplotlib
seaborn
scikit-learn
scipy
plotly
requests

## How to Run
1. Open `DataWarehouse_CW2.ipynb` in Google Colab
2. Run all cells in order (Runtime → Run all)
3. All data is fetched automatically — no file uploads required

## Tasks Covered
- **Task A** — Data extraction, cleaning and metric calculation
  (Daily Return, Beta, Annual Volatility)
- **Task B** — Stock segmentation using Agglomerative and K-Means clustering
- **Task C** — Data mart design, results review and CRM sustainability discussion

## Data Sources
- S&P 500 constituents: Wikipedia
- Daily stock prices: Yahoo Finance via yfinance (2022-01-01 to 2025-01-01)
- Benchmark index: S&P 500 (^GSPC)

## Key Results
- 493 clean stocks after data preprocessing
- 3 clusters identified by both methods:
  - Cluster 0: Low risk (Beta ~0.70, Volatility ~25%)
  - Cluster 1: Medium risk (Beta ~1.17, Volatility ~36%)
  - Cluster 2: High risk (Beta ~1.72, Volatility ~53%)
