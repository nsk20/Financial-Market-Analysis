```markdown
# Financial-Market-Analysis-Nifty-SP500-Gold-USDINR

This repository contains a Google Colab notebook that performs a comprehensive analysis of various financial market instruments: Nifty 50, S&P 500, Gold Futures, and USD/INR exchange rates.

## Project Description

The goal of this project is to load, clean, transform, and analyze historical data for key financial assets. The analysis includes:

- **Data Loading and Combination**: Loading historical data from multiple CSV files for each asset and combining them into single DataFrames.
- **Date and Data Type Conversion**: Ensuring 'Date' columns are correctly parsed and 'Price' related columns are converted to numeric types, handling commas and other formatting issues.
- **Nifty 50 Currency Conversion**: Converting Nifty 50 prices from INR to USD by merging with interpolated USD/INR exchange rate data.
- **Gold Price Unit Conversion**: Converting Gold Futures prices from Troy Ounce to Grams (USD per gram).
- **Historical Returns Calculation**: Calculating 1-year, 3-year, 5-year, 10-year, and 15-year historical returns for Nifty 50 (in USD), S&P 500, and Gold.
- **Correlation Analysis**: Investigating the correlation between daily percentage changes in Gold prices and USD/INR exchange rates.

## Key Findings

- **Historical Returns**: The notebook provides a summary of historical returns for Gold, Nifty-50 (in USD), and S&P500 over different periods (1-year, 3-year, 5-year, 10-year, 15-year, 20-year).
- **Gold vs. USD/INR Correlation**: A weak negative correlation (-0.1992) was observed between the daily percentage change of gold prices and the daily percentage change of USD/INR exchange rates. This suggests that while there's a slight inverse relationship, it's not a strong indicator for day-to-day movements.

## How to Run the Notebook

1.  **Clone the Repository**: Clone this GitHub repository to your local machine.
2.  **Open in Google Colab**: Upload or open the `.ipynb` file in Google Colab.
3.  **Upload Data Files**: Ensure all required CSV data files (e.g., 'Nifty 50 Historical Data.csv', 'S&P 500 Historical Data.csv', 'Gold Futures Historical Data.csv', 'USD_INR Historical Data.csv' and their corresponding 'Historical Data2.csv' files) are present in the Colab environment (e.g., uploaded to `/content/` or mounted from Google Drive).
4.  **Run All Cells**: Execute all cells in the notebook sequentially.

## Data Sources

The historical data for Nifty 50, S&P 500, Gold Futures, and USD/INR exchange rates are assumed to be provided via CSV files named:
- `Nifty 50 Historical Data.csv`
- `Nifty 50 Historical Data2.csv`
- `S&P 500 Historical Data.csv`
- `S&P 500 Historical Data2.csv`
- `Gold Futures Historical Data.csv`
- `Gold Futures Historical Data2.csv`
- `USD_INR Historical Data.csv`
- `USD_INR Historical Data2.csv`

These files should contain columns such as 'Date', 'Price', 'Open', 'High', 'Low', 'Vol.', and 'Change %'.
```
