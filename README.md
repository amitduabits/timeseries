# Time Series Analytics

## A Comprehensive Course for Financial Data Analysis

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Colab](https://img.shields.io/badge/Google-Colab-orange.svg)](https://colab.research.google.com/)
[![License](https://img.shields.io/badge/License-Educational-green.svg)](#)

---

## Table of Contents

1. [Course Overview](#course-overview)
2. [Prerequisites](#prerequisites)
3. [Installation & Setup](#installation--setup)
4. [Course Structure](#course-structure)
5. [Complete Topic Reference](#complete-topic-reference)
6. [How to Use These Materials](#how-to-use-these-materials)
7. [Quick Start Guide](#quick-start-guide)
8. [Learning Path Recommendations](#learning-path-recommendations)
9. [Troubleshooting](#troubleshooting)
10. [Additional Resources](#additional-resources)

---

## Course Overview

This course provides a hands-on, practical approach to **Time Series Analytics** with a focus on financial data analysis. Through real-world examples using Bitcoin, Gold, and stock price data, students will learn to:

- Understand and visualize time series patterns
- Build forecasting models (ARIMA, SARIMA, Exponential Smoothing)
- Model volatility using GARCH
- Analyze multiple time series with VAR models
- Validate and compare model performance
- Create interactive visualizations for data exploration

### Course Philosophy

```
Theory → Implementation → Interpretation → Application
```

Each topic follows this pattern:
1. **Concept explanation** with mathematical formulas
2. **Working Python code** with real financial data
3. **Output interpretation** with practical insights
4. **Visualization** for better understanding

---

## Prerequisites

### Required Knowledge

| Area | Topics | Level |
|------|--------|-------|
| **Statistics** | Mean, variance, correlation, hypothesis testing | Intermediate |
| **Mathematics** | Basic calculus, linear algebra fundamentals | Basic |
| **Python** | Variables, loops, functions, pandas basics | Intermediate |
| **Finance** | Understanding of prices, returns, volatility | Basic |

### Recommended (Not Required)

- Prior exposure to regression analysis
- Familiarity with Jupyter notebooks
- Basic understanding of financial markets

---

## Installation & Setup

### Option 1: Google Colab (Recommended)

No installation required! Simply:

1. Go to [Google Colab](https://colab.research.google.com/)
2. Upload the `.ipynb` notebook files
3. Run the first cell to install dependencies

```python
# Run this in the first cell of any notebook
!pip install yfinance pmdarima arch plotly --quiet
```

### Option 2: Local Installation

```bash
# Create a new directory for your project
mkdir timeseries_analytics
cd timeseries_analytics

# Create a virtual environment
python -m venv venv

# Activate it
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

# Install required packages
pip install yfinance pandas numpy matplotlib seaborn statsmodels scipy pmdarima arch plotly jupyter
```

### Package Dependencies

| Package | Version | Purpose |
|---------|---------|---------|
| `yfinance` | ≥0.2.0 | Download financial data |
| `pandas` | ≥1.5.0 | Data manipulation |
| `numpy` | ≥1.21.0 | Numerical computing |
| `matplotlib` | ≥3.5.0 | Static visualizations |
| `seaborn` | ≥0.12.0 | Statistical visualizations |
| `statsmodels` | ≥0.14.0 | Time series models (ARIMA, VAR) |
| `scipy` | ≥1.9.0 | Statistical functions |
| `pmdarima` | ≥2.0.0 | Auto ARIMA |
| `arch` | ≥5.0.0 | GARCH models |
| `plotly` | ≥5.0.0 | Interactive visualizations |

---

## Course Structure

```
Time Series Analytics/
│
├── 📓 Jupyter Notebooks (Complete Modules)
│   ├── module3_forecasting_model_selection.ipynb
│   ├── module4_advanced_models.ipynb
│   └── module5_integration_practice.ipynb
│
├── 📜 Python Scripts (Original Modules)
│   ├── module3_forecasting_model_selection.py
│   ├── module4_advanced_models.py
│   └── module5_integration_practice.py
│
├── 📁 individual_topics/ (20 Self-Contained Scripts)
│   ├── topic_3_1_train_test_split.py
│   ├── topic_3_2_ar_model.py
│   ├── ... (17 more files)
│   └── topic_5_3_interactive_plotly.py
│
└── 📖 README.md (This file)
```

---

## Complete Topic Reference

### Module 3: Forecasting and Model Selection

| # | Topic | Key Concepts | Notebook | Script | Time |
|---|-------|--------------|----------|--------|------|
| 3.1 | Train-Test Split | Chronological split, data leakage prevention | `module3_*.ipynb` | `topic_3_1_train_test_split.py` | 15 min |
| 3.2 | AR Model | Autoregressive, momentum, φ coefficients | `module3_*.ipynb` | `topic_3_2_ar_model.py` | 20 min |
| 3.3 | MA Model | Moving average, shock effects, θ coefficients | `module3_*.ipynb` | `topic_3_3_ma_model.py` | 20 min |
| 3.4 | ARMA Selection | AIC, BIC, model comparison | `module3_*.ipynb` | `topic_3_4_arma_selection.py` | 25 min |
| 3.5 | ARIMA | Non-stationarity, differencing, ADF test | `module3_*.ipynb` | `topic_3_5_arima_nonstationary.py` | 25 min |
| 3.6 | Auto ARIMA | Automatic parameter selection, pmdarima | `module3_*.ipynb` | `topic_3_6_auto_arima.py` | 15 min |
| 3.7 | Residual Diagnostics | White noise, Ljung-Box test, Q-Q plot | `module3_*.ipynb` | `topic_3_7_residual_diagnostics.py` | 25 min |
| 3.8 | Rolling Validation | Walk-forward, RMSE, MAE | `module3_*.ipynb` | `topic_3_8_rolling_validation.py` | 20 min |
| 3.9 | Prediction Intervals | Confidence bands, uncertainty quantification | `module3_*.ipynb` | `topic_3_9_prediction_intervals.py` | 20 min |

**Module 3 Total Time: ~3 hours**

---

### Module 4: Advanced Time Series Models

| # | Topic | Key Concepts | Notebook | Script | Time |
|---|-------|--------------|----------|--------|------|
| 4.1 | SARIMA | Seasonal patterns, (P,D,Q,s) order | `module4_*.ipynb` | `topic_4_1_sarima.py` | 25 min |
| 4.2 | Simple Exp. Smoothing | Alpha parameter, weighted averages | `module4_*.ipynb` | `topic_4_2_simple_exp_smoothing.py` | 20 min |
| 4.3 | Holt's Linear | Trend component, level + slope | `module4_*.ipynb` | `topic_4_3_holt_linear.py` | 20 min |
| 4.4 | Holt-Winters | Seasonality, additive vs multiplicative | `module4_*.ipynb` | `topic_4_4_holt_winters.py` | 25 min |
| 4.5 | VAR Model | Multivariate, Granger causality | `module4_*.ipynb` | `topic_4_5_var_model.py` | 30 min |
| 4.6 | ARCH Detection | Volatility clustering, LM test | `module4_*.ipynb` | `topic_4_6_arch_detection.py` | 20 min |
| 4.7 | GARCH | Conditional volatility, α + β | `module4_*.ipynb` | `topic_4_7_garch.py` | 30 min |
| 4.8 | Model Comparison | Multi-criteria evaluation, dashboards | `module4_*.ipynb` | `topic_4_8_model_comparison.py` | 25 min |

**Module 4 Total Time: ~3.5 hours**

---

### Module 5: Integration and Practice

| # | Topic | Key Concepts | Notebook | Script | Time |
|---|-------|--------------|----------|--------|------|
| 5.1 | Complete Pipeline | 8-step workflow, end-to-end analysis | `module5_*.ipynb` | `topic_5_1_complete_pipeline.py` | 45 min |
| 5.2 | Reusable Functions | Modular code, compare_models() | `module5_*.ipynb` | `topic_5_2_reusable_function.py` | 30 min |
| 5.3 | Interactive Viz | Plotly, hover, zoom, exploration | `module5_*.ipynb` | `topic_5_3_interactive_plotly.py` | 25 min |

**Module 5 Total Time: ~1.5 hours**

---

### Course Summary

| Module | Topics | Total Time | Focus |
|--------|--------|------------|-------|
| Module 3 | 9 | ~3 hours | Fundamentals & Forecasting |
| Module 4 | 8 | ~3.5 hours | Advanced Models |
| Module 5 | 3 | ~1.5 hours | Integration & Practice |
| **Total** | **20** | **~8 hours** | **Complete Course** |

---

## How to Use These Materials

### Option A: Complete Notebooks (Recommended for Structured Learning)

Best for: **Classroom instruction, sequential learning, comprehensive understanding**

1. Open Google Colab
2. Upload the module notebook (`.ipynb` file)
3. Run cells sequentially from top to bottom
4. Read explanations, run code, observe outputs
5. Complete all topics in a module before moving on

```
📓 module3_forecasting_model_selection.ipynb
   ├── Setup cell (run first)
   ├── Topic 3.1: Train-Test Split
   ├── Topic 3.2: AR Model
   ├── ... (all topics in sequence)
   └── Module Summary
```

**Advantages:**
- Logical flow from basic to advanced
- All dependencies handled in setup
- Rich markdown explanations
- Summary tables for review

---

### Option B: Individual Topic Scripts (Recommended for Quick Reference)

Best for: **Quick review, specific topic lookup, copy-paste examples**

1. Navigate to `individual_topics/` folder
2. Find the specific topic you need
3. Copy the entire script
4. Paste into Google Colab or Python IDE
5. Run and modify as needed

```python
# Example: Just want to learn GARCH?
# Copy contents of topic_4_7_garch.py into Colab
```

**Advantages:**
- Self-contained (no dependencies on other files)
- Under 40 lines of code each
- Heavy comments for quick understanding
- Perfect for exam review

---

### Usage Comparison

| Feature | Complete Notebooks | Individual Scripts |
|---------|-------------------|-------------------|
| Best for | Full learning | Quick reference |
| Setup | Once per module | Each script standalone |
| Learning style | Sequential | Topic-specific |
| Code length | Comprehensive | Minimal (~35 lines) |
| Comments | Markdown cells | Inline comments |
| Time investment | Hours | Minutes |

---

## Quick Start Guide

### 5-Minute Quick Start

```python
# Step 1: Open Google Colab (colab.research.google.com)

# Step 2: Run this setup cell
!pip install yfinance statsmodels --quiet
import yfinance as yf
import matplotlib.pyplot as plt
from statsmodels.tsa.arima.model import ARIMA

# Step 3: Download data
btc = yf.download('BTC-USD', start='2020-01-01', progress=False)['Close'].dropna()

# Step 4: Split data (80% train, 20% test)
train = btc[:int(len(btc)*0.8)]
test = btc[int(len(btc)*0.8):]

# Step 5: Fit ARIMA model
model = ARIMA(train, order=(1, 1, 1))
fitted = model.fit()

# Step 6: Forecast and plot
forecast = fitted.forecast(steps=len(test))
plt.figure(figsize=(12, 5))
plt.plot(train[-100:], label='Training')
plt.plot(test, label='Actual Test')
plt.plot(test.index, forecast, label='Forecast', linestyle='--')
plt.legend()
plt.title('Your First Time Series Forecast!')
plt.show()

print(f"Model AIC: {fitted.aic:.2f}")
print("Congratulations! You've built your first forecasting model!")
```

---

## Learning Path Recommendations

### Path 1: Complete Beginner (No Prior Experience)

```
Week 1: Module 3 (Topics 3.1 - 3.5)
        Focus: Fundamentals, stationarity, basic ARIMA

Week 2: Module 3 (Topics 3.6 - 3.9)
        Focus: Model selection, diagnostics, validation

Week 3: Module 4 (Topics 4.1 - 4.4)
        Focus: Exponential smoothing family

Week 4: Module 4 (Topics 4.5 - 4.8)
        Focus: VAR, GARCH, model comparison

Week 5: Module 5 (All Topics)
        Focus: Integration, practice, projects
```

### Path 2: Intermediate (Some Statistics Background)

```
Day 1: Module 3 (Complete)
       Skim 3.1-3.3, focus on 3.4-3.9

Day 2: Module 4 (Complete)
       Focus on GARCH (4.6-4.7) and VAR (4.5)

Day 3: Module 5 + Practice
       Build your own analysis pipeline
```

### Path 3: Quick Review (Exam Preparation)

```
Session 1 (2 hours): Individual scripts 3.1-3.9
Session 2 (2 hours): Individual scripts 4.1-4.8
Session 3 (1 hour):  Individual scripts 5.1-5.3
```

### Path 4: Project-Focused

```
Start: Topic 5.1 (Complete Pipeline)
Then:  Pick specific topics as needed
       - Need GARCH? → Topic 4.7
       - Need seasonality? → Topics 4.1, 4.4
       - Need multivariate? → Topic 4.5
```

---

## Troubleshooting

### Common Issues and Solutions

#### 1. Package Installation Errors

```python
# Problem: "ModuleNotFoundError: No module named 'yfinance'"
# Solution: Install the package
!pip install yfinance --quiet

# Problem: "arch" package installation fails
# Solution: Try with specific version
!pip install arch==5.3.1 --quiet
```

#### 2. Data Download Issues

```python
# Problem: yfinance returns empty data
# Solution 1: Check internet connection
# Solution 2: Try different date range
btc = yf.download('BTC-USD', start='2022-01-01', progress=False)

# Solution 3: Add error handling
try:
    data = yf.download('BTC-USD', start='2020-01-01', progress=False)['Close']
    if data.empty:
        print("No data returned. Check ticker symbol and date range.")
except Exception as e:
    print(f"Error: {e}")
```

#### 3. Model Convergence Issues

```python
# Problem: "Model did not converge"
# Solution 1: Try simpler model
model = ARIMA(data, order=(1, 1, 0))  # Simpler than (2, 1, 2)

# Solution 2: Use different optimizer
model = ARIMA(data, order=(1, 1, 1))
fitted = model.fit(method='powell')

# Solution 3: Scale your data
data_scaled = (data - data.mean()) / data.std()
```

#### 4. Memory Issues in Colab

```python
# Problem: "ResourceExhaustedError" or Colab crashes
# Solution 1: Use smaller dataset
data = data[-500:]  # Last 500 observations only

# Solution 2: Clear memory
import gc
gc.collect()

# Solution 3: Restart runtime (Runtime → Restart runtime)
```

#### 5. Plotting Issues

```python
# Problem: Plots not showing
# Solution 1: Use plt.show()
plt.plot(data)
plt.show()

# Solution 2: For Colab, use inline magic
%matplotlib inline

# Problem: Plotly not displaying
# Solution: Use Colab-specific renderer
import plotly.io as pio
pio.renderers.default = 'colab'
```

#### 6. Date/Time Issues

```python
# Problem: "DatetimeIndex has no attribute 'date'"
# Solution: Access index correctly
print(data.index[0])  # Not data.index[0].date() for some versions

# Problem: Forecast index doesn't align
# Solution: Create proper date range
forecast_index = pd.date_range(
    start=train.index[-1] + pd.Timedelta(days=1),
    periods=30,
    freq='D'  # or 'B' for business days
)
```

### Getting Help

1. **Check the error message carefully** - Python errors are usually descriptive
2. **Search the error** on Stack Overflow
3. **Check package documentation**:
   - [statsmodels](https://www.statsmodels.org/)
   - [pmdarima](https://alkaline-ml.com/pmdarima/)
   - [arch](https://arch.readthedocs.io/)
4. **Simplify your code** - isolate the problem

---

## Additional Resources

### Books
- *Forecasting: Principles and Practice* by Hyndman & Athanasopoulos (free online)
- *Time Series Analysis* by Hamilton
- *Analysis of Financial Time Series* by Tsay

### Online Resources
- [Statsmodels Documentation](https://www.statsmodels.org/stable/tsa.html)
- [pmdarima Documentation](https://alkaline-ml.com/pmdarima/)
- [ARCH Package Documentation](https://arch.readthedocs.io/)

### Video Tutorials
- Search "ARIMA Python tutorial" on YouTube
- Coursera: "Practical Time Series Analysis"
- DataCamp: "Time Series with Python"

---

## File Checklist

### Jupyter Notebooks
- [ ] `module3_forecasting_model_selection.ipynb`
- [ ] `module4_advanced_models.ipynb`
- [ ] `module5_integration_practice.ipynb`

### Individual Topic Scripts (in `individual_topics/`)
- [ ] `topic_3_1_train_test_split.py`
- [ ] `topic_3_2_ar_model.py`
- [ ] `topic_3_3_ma_model.py`
- [ ] `topic_3_4_arma_selection.py`
- [ ] `topic_3_5_arima_nonstationary.py`
- [ ] `topic_3_6_auto_arima.py`
- [ ] `topic_3_7_residual_diagnostics.py`
- [ ] `topic_3_8_rolling_validation.py`
- [ ] `topic_3_9_prediction_intervals.py`
- [ ] `topic_4_1_sarima.py`
- [ ] `topic_4_2_simple_exp_smoothing.py`
- [ ] `topic_4_3_holt_linear.py`
- [ ] `topic_4_4_holt_winters.py`
- [ ] `topic_4_5_var_model.py`
- [ ] `topic_4_6_arch_detection.py`
- [ ] `topic_4_7_garch.py`
- [ ] `topic_4_8_model_comparison.py`
- [ ] `topic_5_1_complete_pipeline.py`
- [ ] `topic_5_2_reusable_function.py`
- [ ] `topic_5_3_interactive_plotly.py`

---

## License

This material is for educational purposes. Feel free to use, modify, and share for learning.

---

## Contact

For questions or feedback about the course materials, please contact the course instructor.

---

*Last Updated: December 2024*

*Created for Time Series Analytics Course @ BITS*
