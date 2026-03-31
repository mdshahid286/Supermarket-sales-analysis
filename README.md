# Supermarket Sales Analysis 📊

A comprehensive data analysis project examining supermarket sales patterns across multiple branches, product categories, and customer demographics. This project leverages Python and Jupyter notebooks to uncover actionable insights from retail transaction data.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Key Findings](#key-findings)
- [Technologies & Libraries](#technologies--libraries)
- [Analysis Methodology](#analysis-methodology)
- [Results & Visualizations](#results--visualizations)


## Overview

This project performs an in-depth exploratory data analysis (EDA) on supermarket sales data from multiple branches. The analysis reveals trends in customer behavior, product performance, and revenue patterns across different locations and customer segments.

**Key Objectives:**
- Analyze sales trends across branches and product categories
- Identify customer purchasing patterns and preferences
- Evaluate the impact of customer type and payment methods on sales
- Generate data-driven insights for business strategy optimization

## Dataset

**Source:** Supermarket Sales Transaction Data

**Time Period:** January 2019 - March 2019

**Size:** 1,000+ transaction records

### Data Fields

| Field | Description |
|-------|-------------|
| Invoice ID | Unique transaction identifier |
| Branch | Supermarket branch location (Alex, Cairo, Giza) |
| City | City name (Yangon, Mandalay, Naypyitaw) |
| Customer Type | Member or Normal customer classification |
| Gender | Customer gender (Male/Female) |
| Product Line | Product category (Electronics, Food & Beverages, Health & Beauty, etc.) |
| Unit Price | Price per unit (USD) |
| Quantity | Number of units purchased |
| Date | Transaction date |
| Time | Transaction time |
| Payment | Payment method (Cash, Credit Card, E-wallet) |
| Sales | Total sale amount |
| Rating | Customer satisfaction rating (1-10) |
| Tax | Tax amount (5% of sales) |
| Gross Income | Gross margin income |

## Features

✨ **Comprehensive Analysis Includes:**
- Sales trend analysis by branch and location
- Customer segmentation analysis (Members vs. Normal customers)
- Product category performance evaluation
- Payment method preferences
- Customer satisfaction correlation analysis
- Gender-based purchasing behavior
- Time-based (hourly, daily) sales patterns
- Revenue distribution and statistical summaries

## Installation

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or JupyterLab
- pip package manager

### Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/supermarket-sales-analysis.git
   cd supermarket-sales-analysis
   ```

2. **Create a virtual environment (recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install required packages:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

5. **Open the analysis notebook:**
   Navigate to `Supermarket_Sales__1_.ipynb` and run the cells sequentially.

## Project Structure

```
supermarket-sales-analysis/
├── README.md                          # Project documentation
├── requirements.txt                   # Python dependencies
├── SuperMarket_Analysis.csv          # Raw dataset
├── Supermarket_Sales__1_.ipynb       # Main analysis notebook
└── outputs/                          # Generated visualizations
    ├── sales_by_branch.png
    ├── product_performance.png
    └── customer_analysis.png
```

## Usage

### Running the Analysis

1. **Basic Execution:**
   ```bash
   jupyter notebook Supermarket_Sales__1_.ipynb
   ```
   Run all cells from top to bottom to execute the complete analysis.

2. **Step-by-Step Exploration:**
   - Run individual cells to explore specific analyses
   - Modify parameters in the code to customize analysis
   - Generate custom visualizations as needed

### Customization

To analyze specific subsets or time periods:

```python
# Filter by branch
branch_data = df[df['Branch'] == 'Alex']

# Filter by product line
electronics = df[df['Product line'] == 'Electronic accessories']

# Filter by date range
q1_data = df[df['Date'].str.contains('2019-01|2019-02|2019-03')]
```

## Key Findings

**Note:** Run the notebook to generate specific insights from your dataset. Key analysis areas include:

- **Branch Performance:** Comparative analysis of sales across all branches
- **Customer Insights:** Member vs. non-member purchasing patterns
- **Product Excellence:** Top-performing product categories
- **Payment Trends:** Customer payment method preferences
- **Satisfaction Metrics:** Correlation between sales values and customer ratings

## Technologies & Libraries

### Core Technologies
- **Python 3.x** - Programming language
- **Jupyter Notebook** - Interactive computing environment

### Data Analysis & Visualization Libraries
- **pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Scikit-learn** - Machine learning and statistical analysis (if applicable)

### Installation via requirements.txt
```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
scikit-learn>=1.0.0
```

## Analysis Methodology

### 1. **Data Preprocessing**
   - Load and inspect raw data
   - Handle missing values and data types
   - Clean and standardize data formats

### 2. **Exploratory Data Analysis (EDA)**
   - Statistical summary of key metrics
   - Distribution analysis
   - Correlation analysis
   - Outlier detection

### 3. **Visualization**
   - Distribution plots
   - Bar charts for categorical analysis
   - Heatmaps for correlation analysis
   - Time-series plots (if applicable)

### 4. **Insights Generation**
   - Pattern identification
   - Trend analysis
   - Performance benchmarking
   - Actionable recommendations

## Results & Visualizations

The notebook generates comprehensive visualizations including:

- **Sales Distribution:** Histograms and box plots of sales amounts
- **Branch Comparison:** Side-by-side analysis of branch performance
- **Product Analysis:** Revenue and quantity sold by product line
- **Customer Behavior:** Purchasing patterns by customer type and gender
- **Temporal Trends:** Sales patterns by date and time
- **Payment Methods:** Distribution of payment preferences
- **Satisfaction Correlation:** Rating vs. sales relationship analysis

All visualizations are saved automatically during notebook execution.

