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
- [Interim Status](#interim-status)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project performs a comprehensive three-faceted analysis of major technology stocks:

1. **Exploratory Data Analysis (EDA)**: Initial data exploration, cleaning, and visualization of financial news and stock data
2. **Quantitative Analysis**: Evaluates stock performance using traditional financial metrics including returns, volatility, Sharpe ratios, and technical indicators
3. **Sentiment Correlation Analysis**: Analyzes the relationship between financial news sentiment and stock price movements using advanced statistical methods

The analysis focuses on six major tech stocks: **AAPL** (Apple), **AMZN** (Amazon), **GOOG** (Google), **META** (Meta), **MSFT** (Microsoft), and **NVDA** (NVIDIA).

### Key Research Question
**Does news sentiment predict or correlate with stock price movements?** This project answers this question through rigorous statistical analysis, correlation testing, and lagged correlation studies.

## ✨ Features

- **Multi-Stock Analysis**: Comprehensive analysis across 6 major technology stocks
- **Advanced Sentiment Analysis**: 
  - VADER Sentiment Analyzer (optimized for financial text)
  - TextBlob integration for additional sentiment metrics
  - Daily sentiment aggregation and normalization
- **Correlation Analysis**:
  - Pearson correlation (linear relationships)
  - Spearman correlation (monotonic relationships)
  - Lagged correlation analysis (temporal patterns)
  - Statistical significance testing
- **Risk-Return Profiling**: Calculates and compares key financial metrics
- **Technical Indicators**: Implements moving averages, RSI, and other technical analysis tools
- **Automated Visualization**: Generates professional charts and reports
- **Comparative Analysis**: Side-by-side performance comparisons across stocks
- **Time Series Analysis**: Examines trends and patterns over time
- **Date Alignment**: Sophisticated date normalization between news and trading days
- **Export Capabilities**: CSV exports for further analysis and modeling

## 📁 Project Structure

```
financial-sentiment-week1/
├── notebooks/
│   ├── 01_eda_analysis.ipynb          # Exploratory Data Analysis
│   ├── 02_quantitative_analysis.ipynb  # Quantitative Financial Analysis
│   ├── 03_news_sentiment_analysis.ipynb # News Sentiment & Stock Correlation
│   ├── README.md                       # Notebooks documentation
│   └── reports/                        # Generated analysis reports
│       ├── comparative_returns.png
│       ├── eda_visualizations.png
│       ├── headline_length_dist.png
│       ├── monthly_trends.png
│       ├── sentiment_correlation_analysis.png  # Task 3: Correlation visualizations
│       ├── sharpe_comparison.png
│       ├── technical_analysis_AAPL.png
│       ├── time_series_patterns.png
│       ├── top_publishers.png
│       ├── top_stocks.png
│       ├── top_words.png
│       ├── volatility_comparison.png
│       └── sentiment_returns_merged.csv  # Task 3: Merged dataset
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
   - Complete with `notebooks/03_news_sentiment_analysis.ipynb` for sentiment correlation analysis

## 🔄 Project Workflow

The project follows a structured three-task workflow:

```
Task 1: EDA → Task 2: Quantitative Analysis → Task 3: Sentiment Correlation
   ↓                        ↓                              ↓
Data Exploration    Financial Metrics          Sentiment-Return Analysis
```

### Task Progression

1. **Task 1 - EDA**: Understand the data structure, quality, and basic patterns
2. **Task 2 - Quantitative Analysis**: Calculate financial metrics and technical indicators
3. **Task 3 - Sentiment Correlation**: Link news sentiment to stock performance

Each task builds upon the previous one, creating a comprehensive analysis pipeline.

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

3. **News Sentiment Correlation Analysis**:
   - Open `notebooks/03_news_sentiment_analysis.ipynb`
   - Execute cells to:
     - Load and filter news data for specific stocks
     - Perform sentiment analysis using VADER
     - Align news dates with trading days
     - Calculate correlations between sentiment and stock returns
     - Analyze lagged correlations
     - Generate comprehensive visualizations

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

### 3. News Sentiment Correlation Analysis (Task 3)

- **Date Alignment**:
  - Normalize timestamps between news articles and stock trading days
  - Handle timezone-aware timestamps
  - Match news to corresponding trading days

- **Sentiment Analysis**:
  - **VADER Sentiment Analyzer**: Specifically designed for financial text and social media
  - Sentiment scores range from -1 (most negative) to +1 (most positive)
  - Daily sentiment aggregation (mean, median, standard deviation)
  - Article volume analysis

- **Correlation Analysis**:
  - **Pearson Correlation**: Linear relationship between sentiment and returns
  - **Spearman Correlation**: Monotonic relationship (non-parametric)
  - Statistical significance testing (p-values)
  - Analysis for all trading days vs. days with news only

- **Lagged Correlation**:
  - Time-shifted correlation analysis (-5 to +5 days)
  - Identify if sentiment leads or follows stock returns
  - Detect predictive patterns in sentiment-return relationships

- **Visualizations**:
  - Scatter plots with regression lines
  - Lagged correlation plots
  - Time series comparisons
  - Sentiment distribution histograms
  - Article volume impact analysis

## 📊 Results & Reports

The analysis generates several visualization reports saved in `notebooks/reports/`:

- **Comparative Returns**: Multi-stock return comparison
- **Volatility Comparison**: Risk analysis across stocks
- **Sharpe Ratio Comparison**: Risk-adjusted performance metrics
- **Technical Analysis**: Detailed technical indicators for individual stocks
- **EDA Visualizations**: Comprehensive exploratory data analysis charts
- **Time Series Patterns**: Temporal trend analysis
- **Top Words/Publishers/Stocks**: Key insights from sentiment analysis
- **Sentiment Correlation Analysis** (Task 3): 
  - Correlation scatter plots with regression lines
  - Lagged correlation visualizations
  - Time series sentiment vs. returns comparison
  - Sentiment distribution analysis
  - Merged dataset CSV export for further analysis

## 📥 Data Sources

- **Stock Price Data**: 
  - Local CSV files in `data/raw/stocks/`
  - Alternative: yFinance API for real-time data
  
- **Sentiment Data**:
  - Analyst ratings from `data/row/raw_analyst_ratings.csv`
  - Financial news headlines (processed in notebooks)

## 🎯 Task 3: News Sentiment Correlation Analysis

### Overview
Task 3 focuses on establishing the statistical relationship between financial news sentiment and stock price movements. This analysis answers the critical question: **Can news sentiment predict or explain stock returns?**

### Key Achievements

✅ **Complete Implementation**
- Full sentiment analysis pipeline using VADER Sentiment Analyzer
- Robust date alignment between news articles and trading days
- Comprehensive correlation analysis with statistical validation

✅ **Advanced Statistical Analysis**
- Pearson correlation (linear relationships)
- Spearman correlation (non-parametric, monotonic relationships)
- Lagged correlation analysis (-5 to +5 days)
- Statistical significance testing with p-values

✅ **Comprehensive Visualizations**
- 4-panel dashboard showing:
  - Sentiment vs. Returns scatter plot with regression line
  - Lagged correlation patterns
  - Time series comparison
  - Sentiment distribution analysis

✅ **Research Quality**
- Academic references included
- Methodology documentation
- Reproducible analysis framework
- Results exported for further research

### Key Findings

The analysis reveals:
- **Correlation Strength**: Quantified relationship between sentiment and returns
- **Temporal Patterns**: Whether sentiment leads or follows price movements
- **Statistical Significance**: Validated findings through rigorous testing
- **Practical Insights**: Actionable information for financial analysis

### Files Generated

- `notebooks/03_news_sentiment_analysis.ipynb`: Complete analysis notebook
- `notebooks/reports/sentiment_correlation_analysis.png`: Visualization dashboard
- `notebooks/reports/sentiment_returns_merged.csv`: Merged dataset for further analysis

## 📊 Interim Status

### ✅ Completed Milestones

1. **Project Setup & Infrastructure**
   - Repository structure established with conventional directory layout
   - Virtual environment configuration
   - Dependencies documented in `requirements.txt`
   - Git workflow initialized

2. **Exploratory Data Analysis (EDA)**
   - Data loading and path resolution utilities implemented
   - Dataset loaded: 1,407,328 analyst rating records
   - Basic descriptive statistics completed
   - Headline length and word count analysis
   - Publisher and stock coverage analysis
   - Time series analysis with hourly/daily patterns
   - Visualization suite generated (11+ charts)

3. **Quantitative Analysis Foundation**
   - yFinance integration with robust error handling
   - Stock data download functionality
   - Multi-stock analysis framework established
   - Technical indicator calculations prepared

4. **News Sentiment Correlation Analysis (Task 3)** ✅
   - Complete sentiment analysis pipeline using VADER
   - Date alignment between news articles and trading days
   - Daily sentiment aggregation and statistics
   - Pearson and Spearman correlation calculations
   - Lagged correlation analysis (-5 to +5 days)
   - Comprehensive visualizations (4-panel dashboard)
   - Statistical significance testing
   - Results export to CSV
   - Academic references and methodology documentation

5. **Documentation**
   - Comprehensive README with project overview
   - Notebook headers and structure
   - Directory READMEs in place

### 🔄 In Progress

1. **Quantitative Analysis Completion**
   - Sharpe ratio calculations
   - Volatility comparisons
   - Technical indicator visualizations
   - Risk-return profiling

2. **Code Quality Improvements**
   - Standardized docstrings for all functions
   - Consistent inline comments
   - Error handling enhancements

### 📋 Next Steps

1. **Advanced Sentiment Analysis**
   - Multi-stock sentiment correlation comparison
   - Sector-wide sentiment analysis
   - Sentiment-based trading strategy backtesting
   - Real-time sentiment monitoring pipeline

2. **Predictive Modeling**
   - Machine learning models for return prediction
   - Sentiment-based feature engineering
   - Model evaluation and validation
   - Portfolio optimization with sentiment signals

3. **Extended Analysis**
   - Cross-stock sentiment spillover effects
   - News source credibility weighting
   - Sentiment momentum indicators
   - Integration with technical indicators

3. **Documentation Enhancement**
   - Complete function docstrings
   - Add code examples to README
   - Create analysis methodology documentation
   - Generate API documentation for utility functions

4. **Testing & Validation**
   - Unit tests for data loading functions
   - Validation tests for calculations
   - Data quality checks
   - Edge case handling

5. **Performance Optimization**
   - Optimize large dataset processing
   - Implement caching for repeated calculations
   - Parallel processing where applicable

### 🎯 Project Goals

- ✅ Complete sentiment analysis pipeline
- ✅ Establish statistical relationships between sentiment and stock performance
- ✅ Generate actionable insights for financial analysis
- ✅ Create reproducible analysis framework
- 🔄 Develop predictive models using sentiment signals
- 🔄 Build real-time sentiment monitoring system

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

- **yFinance** for providing stock market data
- **VADER Sentiment**: Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14).
- **Financial Sentiment Research**: Bollen, J., Mao, H., & Zeng, X. (2011). Twitter mood predicts the stock market. Journal of Computational Science, 2(1), 1-8.
- The open-source community for excellent Python libraries
- Financial data providers and news sources

## 📚 Research & Methodology

### Sentiment Analysis Approach

This project uses **VADER (Valence Aware Dictionary and sEntiment Reasoner)**, a rule-based sentiment analysis tool specifically designed for social media text and financial news. VADER provides:

- **Compound Score**: Normalized score between -1 (most negative) and +1 (most positive)
- **Context Awareness**: Handles financial terminology, capitalization, and punctuation
- **Speed**: Fast processing suitable for large datasets (1M+ articles)

### Statistical Methods

- **Pearson Correlation**: Measures linear relationships between sentiment and returns
- **Spearman Correlation**: Non-parametric measure of monotonic relationships
- **Lagged Correlation**: Identifies temporal patterns and predictive signals
- **Statistical Significance**: p-value testing to validate findings

### Date Alignment Strategy

News articles are matched to trading days using:
- Date normalization (removing time components)
- Trading day alignment (excluding weekends and holidays)
- Multiple aggregation strategies (mean, median, weighted by volume)

### Interpreting Results

**Correlation Strength Guidelines:**
- |r| < 0.1: Very weak relationship
- 0.1 ≤ |r| < 0.3: Weak relationship
- 0.3 ≤ |r| < 0.5: Moderate relationship
- 0.5 ≤ |r| < 0.7: Strong relationship
- |r| ≥ 0.7: Very strong relationship

**Statistical Significance:**
- p < 0.05: Statistically significant (reliable finding)
- p ≥ 0.05: Not statistically significant (may be due to chance)

**Lagged Correlation Interpretation:**
- Positive lag: Sentiment leads returns (predictive signal)
- Negative lag: Returns lead sentiment (reactive sentiment)
- Lag = 0: Same-day correlation (contemporaneous relationship)

## 🔬 Example: Running Task 3 Analysis

Here's a quick example of what Task 3 accomplishes:

```python
# Load and prepare data
news_df = load_news_data()  # Load 1.4M+ articles
stock_df = load_stock_data()  # Load AAPL price data

# Perform sentiment analysis
sentiment_scores = analyze_sentiment(news_df['headline'])

# Aggregate daily sentiment
daily_sentiment = aggregate_by_date(sentiment_scores)

# Calculate correlations
correlation = calculate_correlation(daily_sentiment, stock_returns)

# Result: Statistical relationship between news sentiment and stock returns
print(f"Correlation: {correlation:.4f}")
```

### Expected Output

- **Correlation coefficients**: Quantified relationship strength
- **Statistical significance**: p-values indicating reliability
- **Lagged patterns**: Temporal relationships between sentiment and returns
- **Visualizations**: Comprehensive charts showing all relationships

## 📧 Contact

For questions, suggestions, or collaborations, please open an issue in the repository.

---

**Note**: This project is for educational and research purposes. Always consult with a financial advisor before making investment decisions. Past performance does not guarantee future results.
