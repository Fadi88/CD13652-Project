# AI Trading Algorithms Project

## Project Title
Optimizing AI Trading Algorithms

## Project Description
This project focuses on optimizing machine learning models to predict stock price movements. Specifically, we analyze the Health Care Select Sector SPDR Fund (XLV) using data from the CBOE Volatility Index (VIX) and Google Trends search interest for "recession". The goal is to predict the direction of 5-day future returns using a Random Forest Classifier.

## Getting Started

To get a local copy up and running, follow these steps.

### Dependencies

*   Python 3.x
*   Jupyter Notebook
*   Pandas, NumPy, Matplotlib, Seaborn, Plotly
*   Scikit-learn
*   TA-Lib (Technical Analysis Library in Python)
*   yfinance

### Installation

1.  Clone the repository.
2.  Install `uv` if you haven't already:
    ```bash
    pip install uv
    ```
3.  Create a virtual environment and sync dependencies:
    ```bash
    uv venv
    uv pip install pandas numpy matplotlib seaborn plotly scikit-learn ta yfinance
    ```

### Usage

1.  Navigate to the `Project` directory.
2.  Open `project_submission.ipynb` (or `project_starter.ipynb`) in Jupyter Notebook.
3.  Run all cells to execute the analysis and model training.

## Files

*   `project_submission.ipynb`: The completed notebook with full analysis and implementation.
*   `solution.py`: Python script containing the core logic and verification of the implementation.
*   `xlv_data.csv`: Daily price data for XLV.
*   `vix_data.csv`: Daily price data for VIX.
*   `GoogleTrendsData.csv`: Monthly Google Trends data for the term "recession".
*   `readme.md`: This file.

## Methodologies

*   **Feature Engineering**: Cyclical date features, technical indicators (RSI, Bollinger Bands, IBS), rolling returns.
*   **Data Cleaning**: Handling NaNs, merging datasets with different frequencies.
*   **Model Training**: Random Forest Classifier with GridSearchCV for hyperparameter tuning.
*   **Evaluation**: Accuracy, Precision, Recall, F1-score, and Feature Importance analysis.
