# Financial Sentiment Analysis - Week 1

## 📊 Project Description
A comprehensive analysis of financial sentiment and quantitative metrics for major tech stocks, combining exploratory data analysis with quantitative financial modeling.

## 🏗️ Project Structure
financial-sentiment-week1/
├── notebooks/
│ ├── 01_eda_analysis.ipynb # Exploratory Data Analysis
│ ├── 02_quantitative_analysis.ipynb # Quantitative Financial Analysis
│ ├── README.md # Notebooks documentation
│ └── reports/ # Generated analysis reports
│ ├── comparative_returns.png
│ ├── sharpe_comparison.png
│ ├── technical_analysis_AAPL.png
│ └── volatility_comparison.png
├── data/
│ ├── raw/ # Raw data files
│ │ └── stocks/
│ │ ├── AAPL.csv
│ │ ├── AMZN.csv
│ │ ├── GOOG.csv
│ │ ├── META.csv
│ │ ├── MSFT.csv
│ │ └── NVDA.csv
│ └── processed/ # Processed data (git-tracked)
├── .gitignore # Excludes large data files
└── requirements.txt # Python dependencies

## 📈 Analysis Completed

### 1. Exploratory Data Analysis (EDA)
- Initial data exploration and cleaning
- Stock price visualization
- Data quality assessment
- Basic statistical analysis

### 2. Quantitative Analysis
- **Stock Performance Analysis**: Returns calculation and comparison
- **Risk Metrics**: Volatility analysis across multiple stocks
- **Sharpe Ratio**: Risk-adjusted return comparisons
- **Technical Analysis**: Technical indicators for AAPL
- **Comparative Analysis**: Side-by-side performance metrics

## 🎯 Key Features
- Multi-stock analysis (AAPL, AMZN, GOOG, META, MSFT, NVDA)
- Comprehensive risk-return profiling
- Technical indicator implementation
- Automated report generation
- Professional data visualization

## 🛠️ Technologies Used
- **Python 3.x**
- **Jupyter Notebooks**
- **Data Analysis**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Financial Data**: yFinance
- **Version Control**: Git & GitHub

## 🚀 Quick Start

### Prerequisites
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
Installation
pip install -r requirements.txt
