# Consumer Spending & Economic Trends Analysis

**Project Title:**  
**Consumer Spending and Economic Trends: A Data-Driven Analysis Using Affinity Insights**

## Overview
This project analyzes U.S. consumer spending behavior using high-frequency transaction data from the [Opportunity Insights Economic Tracker](https://opportunityinsights.org). The analysis focuses on spending across income levels, essential vs. non-essential categories, and different economic phases (e.g., COVID crash, recovery, inflation). The project integrates traditional statistical testing with machine learning and deep learning models to forecast future trends and derive actionable insights.

---

## Key Objectives
- Forecast future consumer spending using time series models.
- Explore behavioral differences across income groups.
- Identify long-term, seasonal, and volatility trends in spending.
- Analyze essential vs. non-essential spending patterns.

---

## Tools & Technologies
- **Languages & IDEs:** Python, Jupyter Notebook, Excel  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Scikit-learn, TensorFlow/Keras, Prophet  
- **Models Used:** ARIMA, Prophet, LSTM, Transformer  
- **Statistical Tests:** Paired t-test, Wilcoxon signed-rank, Cohen’s d  
- **Techniques:** STL decomposition, ACF/PACF analysis

---

## Workflow Summary

### Data Collection
- Dataset: Affinity consumer transaction data (2018–2024)  
- ~50,000 records with ZIP-level aggregation and income quartile segmentation

### Data Preprocessing
- Created date features from raw columns
- Cleaned and imputed missing values using interpolation + fill methods
- Filtered to focus on post-2020 recovery phase

###  Exploratory Data Analysis
- Histograms, boxplots, time-series plots
- Segmentation by income (Q1–Q4) and category (essential vs. non-essential)
- Economic phase analysis: COVID crash, recovery, inflation, stabilization

### Modeling
| Model       | Dataset Type     | RMSE     |
|-------------|------------------|----------|
| ARIMA       | Full             | 0.0079   |
| ARIMA       | Recovery Phase   | 0.0088   |
| Prophet     | Full             | 0.0162   |
| LSTM        | Full             | **0.0047** |
| Transformer | Full             | 0.0246   |

- **ARIMA**: Best for stable, structured recovery data  
- **LSTM**: Most accurate for complex patterns across the full dataset  
- **Prophet**: Captured holiday and seasonal effects  
- **Transformer**: Handled long-term dependencies, moderate performance  
---
## Results & Insights
- LSTM provided the most accurate forecasts for dynamic spending trends.
- ARIMA excelled in modeling recovery-phase patterns.
- Low-income households (Q1) consistently outspent high-income (Q4) during recovery.
- Non-essential spending differences were more significant than essentials between income groups.
- Seasonal trends (e.g., holiday spending) normalized by 2022 after COVID disruption.
---
##Key Takeaways
- Time series forecasting combined with robust data preprocessing delivers valuable insights for both policy and business decisions.
- Behavioral segmentation reveals critical drivers in economic recovery, especially from low-income consumer groups.
- Merging traditional statistical methods with deep learning models offers a more holistic economic analysis framework.
---
## 🔗 Dataset Source
[Opportunity Insights Economic Tracker](https://opportunityinsights.org)


