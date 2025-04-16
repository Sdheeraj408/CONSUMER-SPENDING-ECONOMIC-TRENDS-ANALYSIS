# CONSUMER SPENDING & ECONOMIC TRENDS ANALYSIS
Absolutely! Here's a **GitHub project overview** written in the same structure and style as your Amazon Reviews project, but for your **Consumer Spending and Economic Trends** capstone:

---

## Consumer-Spending-Analysis

### Consumer Spending and Economic Trends: A Data-Driven Analysis Using Affinity Insights

**Overview**  
• **Dataset**: Affinity Solutions consumer transaction data via Opportunity Insights Economic Tracker  
• **Problem**: Analyzing consumer spending behavior across income groups and forecasting future spending  
• This project aims to uncover trends and behavioral shifts in U.S. consumer spending across income levels and economic phases, such as the COVID-19 crash and recovery.  
• We used statistical techniques and advanced time series forecasting models (ARIMA, Prophet, LSTM, Transformer) to address four key research questions.  
• Achieved the highest forecasting accuracy using LSTM with RMSE of **0.0047** on full data and ARIMA with RMSE of **0.0088** on the recovery phase.

---

### Data Preprocessing  
• **Data Loading**: Loaded Affinity consumer transaction dataset with 50K+ records from Dec 2018 to June 2024.  
• **Cleaning**: Handled missing values with linear interpolation and forward/backward fill. Filtered data from Jan 2020 to June 2024 and created a recovery-phase subset (2021–2024).  
• **Feature Engineering**: Created combined date field, classified data by income quartiles (Q1 to Q4), and grouped by economic phases (COVID crash, inflation, recovery, etc.).

---

### Exploratory Data Analysis (EDA)  
• Generated histograms, boxplots, and bar charts to compare spending patterns.  
• Analyzed volatility and trends across five economic phases.  
• Time series decomposition revealed seasonal peaks (e.g., December holiday spikes) and post-pandemic recovery.

---

### Modeling  
• **Forecasting Models**: ARIMA, Prophet, LSTM, Transformer  
• **Statistical Tests**: Paired t-test, Wilcoxon signed-rank test, Cohen’s d for effect size  
• **Segmentation**: Analyzed essential vs. non-essential spending across income quartiles

---

### Code  
`Consumer_Spending_Analysis.ipynb`  
• Data cleaning, time-based aggregation, visualizations  
• Applied STL decomposition, ACF/PACF for ARIMA  
• Implemented ML/DL forecasting models: ARIMA, Prophet, LSTM, Transformer  
• Statistical testing for income-based and category-based differences  

---

### Results  
• **Four time series models** were compared using MAE, MSE, RMSE.  
• **LSTM** was best for full dataset (RMSE: **0.0047**), **ARIMA** for recovery-phase data (RMSE: **0.0088**)  
• **Income-based insights**: Q1 (low income) spent more than Q4 (high income) during recovery.  
• **Spending trends**: Recovery showed strong rebounds, with seasonal trends stabilizing by 2022.  
• **Essential vs. Non-Essential**: Low-income groups had higher spending in both, with stronger differences in non-essential categories.

| Model         | Dataset        | RMSE   |
|---------------|----------------|--------|
| ARIMA         | Full           | 0.0079 |
| ARIMA         | Recovery Phase | 0.0088 |
| Prophet       | Full           | 0.0162 |
| LSTM          | Full           | 0.0047 |
| Transformer   | Full           | 0.0246 |

---

This format will look great in your GitHub README. Let me know if you'd like it converted into Markdown or need help uploading the notebook and visualizations!

