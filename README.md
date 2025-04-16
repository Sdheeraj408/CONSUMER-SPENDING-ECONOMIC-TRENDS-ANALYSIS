Consumer Spending & Economic Trends Analysis
Project Title:
Consumer Spending and Economic Trends: A Data-Driven Analysis Using Affinity Insights

Overview:
In this project, I performed an end-to-end data analysis to explore, model, and forecast U.S. consumer spending behavior using high-frequency transaction data sourced from the Opportunity Insights Economic Tracker. The goal was to understand how consumer spending varies by income levels, geographic locations, and economic events—such as the COVID-19 crash and recovery—and to build robust forecasting models for economic trend prediction.

Key Objectives
Analyze consumer spending behavior across four income quartiles.

Compare essential vs. non-essential spending patterns.

Identify long-term and seasonal trends.

Predict future consumer spending using time series models.

Tools & Technologies
Languages & IDEs: Python, Jupyter Notebook, Excel

Libraries & Frameworks: Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Scikit-learn, TensorFlow, Prophet

Models Used: ARIMA, Prophet, LSTM, Transformer

Statistical Techniques: Paired t-test, Wilcoxon signed-rank test, Cohen’s d, STL decomposition

Project Workflow
Data Collection: Pulled 50,000+ records of consumer transaction data aggregated by ZIP code and income group (2018–2024).

Data Preprocessing: Created time features, addressed missing values using linear interpolation and fill methods, and filtered the dataset to focus on post-pandemic trends.

Exploratory Data Analysis: Visualized trends, spending distributions, and phase-based transitions (COVID crash, inflation, recovery).

Segmentation: Divided spending into essential vs. non-essential categories and income quartiles (Q1–Q4).

Modeling:

ARIMA: Effective for short-term linear trend forecasting

Prophet: Captured holiday and seasonality effects

LSTM: Achieved the lowest RMSE (0.0047) on full data

Transformer: Explored advanced sequence modeling with moderate results

Performance Metrics: RMSE, MAE, MSE were used to evaluate and compare model performance.

Results & Insights
LSTM outperformed other models in predicting complex non-linear trends in full data.

ARIMA excelled in forecasting within stabilized recovery-phase data.

Low-income groups (Q1) consistently spent more than high-income groups (Q4) during economic recovery phases—challenging conventional assumptions.

Spending trends across five defined economic phases revealed rapid recovery and stabilization post-pandemic.

Statistically significant differences were observed between income quartiles across essential and non-essential categories.

Key Takeaways
Robust data preparation and time series forecasting can yield valuable economic insights from transaction-level data.

Low-income household behavior plays a crucial role in driving consumer recovery post-economic disruptions.

Combining traditional statistical techniques with deep learning offers a comprehensive approach to modeling financial behavior.

