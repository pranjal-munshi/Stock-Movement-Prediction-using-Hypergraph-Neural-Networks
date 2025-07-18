# 📈 Sector-Aware Stock Prediction Evaluation Framework

This repository provides a flexible and extensible framework for evaluating stock price predictions using blind test cases and sector-based grouping. The system supports weekly predictions on multiple stock tickers, segmented by sectors, and allows evaluation using metrics like MAPE.

## 🗂️ Project Structure

- `blind_test_cases.json` — JSON file containing blind test cases for various stock tickers and dates. These are used to validate predictions without revealing the ground truth during inference.
- `hyperedges.json` — Defines sector-level groupings of tickers for sector-aware analysis.
- `validation_stock_data.csv` — CSV file with the ground truth validation data (e.g., Open, High, Low, Close, Volume) for comparison and scoring.

## 🧠 Key Features

- **Sector-based Evaluation**: Group tickers into sectors to allow per-sector performance analysis.
- **Blind Testing Setup**: Make predictions for predefined dates and tickers without peeking at the true data.
- **Evaluation Metrics**: Currently supports MAPE (Mean Absolute Percentage Error); can be extended with additional metrics.
- **Extensible Format**: Easy to plug into other forecasting models or evaluation pipelines.
