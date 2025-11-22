# Financial Sentiment Analysis - Week 1

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A comprehensive analysis project that combines **financial sentiment analysis** with **quantitative metrics** for major technology stocks. This project explores the relationship between market sentiment, news headlines, and stock performance through exploratory data analysis and advanced quantitative modeling.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Analysis Components](#analysis-components)
- [Results & Reports](#results--reports)
- [Data Sources](#data-sources)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project performs a dual-faceted analysis of major technology stocks:

1. **Sentiment Analysis**: Analyzes financial news headlines and analyst ratings to extract market sentiment
2. **Quantitative Analysis**: Evaluates stock performance using traditional financial metrics including returns, volatility, Sharpe ratios, and technical indicators

The analysis focuses on six major tech stocks: **AAPL** (Apple), **AMZN** (Amazon), **GOOG** (Google), **META** (Meta), **MSFT** (Microsoft), and **NVDA** (NVIDIA).

## ✨ Features

- **Multi-Stock Analysis**: Comprehensive analysis across 6 major technology stocks
- **Sentiment Extraction**: Utilizes TextBlob and VADER Sentiment for headline analysis
- **Risk-Return Profiling**: Calculates and compares key financial metrics
- **Technical Indicators**: Implements moving averages, RSI, and other technical analysis tools
- **Automated Visualization**: Generates professional charts and reports
- **Comparative Analysis**: Side-by-side performance comparisons across stocks
- **Time Series Analysis**: Examines trends and patterns over time

## 📁 Project Structure

```
financial-sentiment-week1/
├── notebooks/
│   ├── 01_eda_analysis.ipynb          # Exploratory Data Analysis
│   ├── 02_quantitative_analysis.ipynb  # Quantitative Financial Analysis
│   ├── README.md                       # Notebooks documentation
│   └── reports/                        # Generated analysis reports
│       ├── comparative_returns.png
│       ├── eda_visualizations.png
│       ├── headline_length_dist.png
│       ├── monthly_trends.png
│       ├── sharpe_comparison.png
│       ├── technical_analysis_AAPL.png
│       ├── time_series_patterns.png
│       ├── top_publishers.png
│       ├── top_stocks.png
│       ├── top_words.png
│       └── volatility_comparison.png
├── data/
│   ├── raw/                            # Raw data files
│   │   ├── stocks/                     # Stock price data (CSV)
│   │   │   ├── AAPL.csv
│   │   │   ├── AMZN.csv
│   │   │   ├── GOOG.csv
│   │   │   ├── META.csv
│   │   │   ├── MSFT.csv
│   │   │   └── NVDA.csv
│   │   └── row/                        # Raw analyst ratings
│   │       ├── raw_analyst_ratings.csv
│   │       └── stock/                  # Stock-specific ratings
│   └── processed/                      # Processed/cleaned data
├── scripts/                            # Utility scripts
├── src/                                # Source code modules
├── tests/                              # Unit tests
├── reports/                            # Additional reports
├── requirements.txt                    # Python dependencies
└── README.md                           # This file
```

## 🛠️ Technologies Used

### Core Libraries
- **Python 3.8+**: Programming language
- **Jupyter Notebooks**: Interactive analysis environment

### Data Processing
- **Pandas** (≥2.0.0): Data manipulation and analysis
- **NumPy** (≥2.0.0): Numerical computing

### Visualization
- **Matplotlib** (≥3.7.0): Static plotting
- **Seaborn** (≥0.12.0): Statistical visualizations
- **Plotly** (≥5.15.0): Interactive visualizations

### Financial Data
- **yFinance** (≥0.2.0): Stock market data retrieval

### Sentiment Analysis
- **TextBlob** (≥0.17.0): Text processing and sentiment analysis
- **VADER Sentiment** (≥3.3.0): Financial text sentiment analyzer

### Technical Analysis
- **TA** (≥0.10.0): Technical indicators library

### Scientific Computing
- **SciPy** (≥1.10.0): Statistical functions and optimization

## 🚀 Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Git (optional, for cloning the repository)

### Setup Instructions

1. **Clone the repository** (or navigate to the project directory):
   ```bash
   git clone <repository-url>
   cd financial-sentiment-week1
   ```

2. **Create a virtual environment** (recommended):
   ```bash
   # On Windows
   python -m venv .venv
   .venv\Scripts\activate

   # On macOS/Linux
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

5. **Open the analysis notebooks**:
   - Start with `notebooks/01_eda_analysis.ipynb` for exploratory analysis
   - Proceed to `notebooks/02_quantitative_analysis.ipynb` for quantitative metrics

## 📊 Usage

### Running the Analysis

1. **Exploratory Data Analysis**:
   - Open `notebooks/01_eda_analysis.ipynb`
   - Execute cells sequentially to:
     - Load and clean financial data
     - Perform initial data exploration
     - Generate visualizations
     - Analyze sentiment from headlines

2. **Quantitative Analysis**:
   - Open `notebooks/02_quantitative_analysis.ipynb`
   - Execute cells to:
     - Calculate returns and volatility
     - Compute Sharpe ratios
     - Generate technical indicators
     - Create comparative visualizations

### Data Preparation

The project expects stock data in CSV format in `data/raw/stocks/`. If data is not available locally, the notebooks include functionality to download data using `yfinance`.

## 📈 Analysis Components

### 1. Exploratory Data Analysis (EDA)

- **Data Quality Assessment**: Missing values, data types, and completeness
- **Stock Price Visualization**: Time series plots for all stocks
- **Headline Analysis**: 
  - Text length distribution
  - Most common words
  - Publisher analysis
  - Monthly trend analysis
- **Basic Statistical Analysis**: Summary statistics for all stocks

### 2. Quantitative Analysis

- **Stock Performance Metrics**:
  - Daily and cumulative returns
  - Volatility (standard deviation of returns)
  - Risk-adjusted returns (Sharpe ratio)
  
- **Technical Indicators**:
  - Moving averages (SMA, EMA)
  - Relative Strength Index (RSI)
  - Bollinger Bands
  - Volume analysis

- **Comparative Analysis**:
  - Side-by-side return comparisons
  - Volatility rankings
  - Sharpe ratio comparisons
  - Risk-return scatter plots

## 📊 Results & Reports

The analysis generates several visualization reports saved in `notebooks/reports/`:

- **Comparative Returns**: Multi-stock return comparison
- **Volatility Comparison**: Risk analysis across stocks
- **Sharpe Ratio Comparison**: Risk-adjusted performance metrics
- **Technical Analysis**: Detailed technical indicators for individual stocks
- **EDA Visualizations**: Comprehensive exploratory data analysis charts
- **Time Series Patterns**: Temporal trend analysis
- **Top Words/Publishers/Stocks**: Key insights from sentiment analysis

## 📥 Data Sources

- **Stock Price Data**: 
  - Local CSV files in `data/raw/stocks/`
  - Alternative: yFinance API for real-time data
  
- **Sentiment Data**:
  - Analyst ratings from `data/row/raw_analyst_ratings.csv`
  - Financial news headlines (processed in notebooks)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- yFinance for providing stock market data
- The open-source community for excellent Python libraries
- Financial data providers and news sources

## 📧 Contact

For questions, suggestions, or collaborations, please open an issue in the repository.

---

**Note**: This project is for educational and research purposes. Always consult with a financial advisor before making investment decisions. Past performance does not guarantee future results.
