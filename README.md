# Forex Agentic AI – Currency Forecasting System

## Overview
This project is an agentic AI system for forex analysis that automatically collects historical currency exchange data, trains forecasting models, predicts future exchange rates, and identifies whether currencies are likely to increase or decrease in 2026.

The system uses Yahoo Finance for data retrieval and Facebook Prophet for time-series forecasting.

## What This Agent Does
- Automatically fetches historical forex data  
- Trains one forecasting model per currency pair  
- Predicts average exchange rates for the year 2026  
- Classifies each pair as Increase or Decrease  
- Visualizes forecasts for individual pairs or all pairs together  

## Technologies Used
- Python  
- yfinance – financial data from Yahoo Finance  
- pandas – data processing  
- Prophet – time-series forecasting  
- matplotlib – data visualization  

## Currency Pairs Used
The project analyzes 20 major forex pairs, including:

EURUSD, GBPUSD, USDJPY, AUDUSD, USDCAD,  
USDCHF, NZDUSD, EURGBP, EURJPY, GBPJPY,  
AUDJPY, CHFJPY, EURCHF, GBPCHF, AUDCAD,  
AUDCHF, AUDNZD, CADJPY, EURAUD, GBPAUD  

Example:  
EURUSD=X means 1 Euro priced in US Dollars.

## Project Workflow
### Data Collection
Historical forex data is downloaded from Yahoo Finance.

### Model Training
Each currency pair is trained using a Prophet forecasting model.

### Prediction
The model predicts the average exchange rate for 2026.

### Decision Signal
- Increase → predicted rate > current rate  
- Decrease → predicted rate < current rate  

### Visualization
Forecasts can be plotted individually or all together.

## Output Example

| Pair      | Current Rate | Predicted Rate 2026 | Signal   |
|----------|--------------|---------------------|----------|
| EURUSD=X | 1.09         | 1.14                | Increase |
| USDJPY=X | 145.3        | 138.7               | Decrease |
