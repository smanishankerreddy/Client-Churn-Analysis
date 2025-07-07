# Client-Churn-Analysis
Project: Energy Client Churn & Consumption Modeling
Author: Manishankerreddy Sanampudi
Tools Used: Python · Pandas · Seaborn · Matplotlib · Scikit-learn · Jupyter Notebook

📬 Scenario
A utility provider shared two datasets:

client_data.csv – containing electricity/gas consumption history, margin metrics, product engagement, and churn labels

price_data.csv – containing dynamic pricing for off-peak, peak, and mid-peak periods over time

The client requested a comprehensive Exploratory Data Analysis (EDA) to understand:

What features are most predictive of churn?

Do consumption habits affect customer retention?

How does pricing variability influence contract cancellations?

Can we identify segments based on margin and product engagement?

🔧 Workflow Overview
1. Data Import & Initial Exploration
Loaded both client_data.csv and price_data.csv

Merged datasets using id for alignment of client and pricing data

Checked for null values, inconsistent formats, and outliers

2. Feature Understanding
Based on the Data Description.pdf, columns include:

Consumption patterns: cons_12m, forecast_cons_12m, imp_cons

Margin indicators: net_margin, margin_net_pow_ele

Temporal features: contract start, end, and renewal dates

Flags: has_gas, nb_prod_act, churn

3. EDA & Visualization
Correlation matrix to identify strongest predictors of churn

Histogram and boxplot visualizations of margin vs churn

Trend analysis on num_years_antig, pow_max, and nb_prod_act

Clustered plots by channel_sales and origin_up to detect segment behavior

4. Insights & Initial Observations
Clients with low net margins and short contract antiquity tend to churn more

Gas users exhibit different churn patterns than electricity-only clients

Forecast accuracy vs actual consumption has a churn impact

Seasonal pricing variability (peak/off-peak) aligns with churn spikes

📈 Outcome
The EDA helped build a foundation for future churn prediction models. Key features were shortlisted for modeling based on:

High correlation with churn

Business interpretability

Low data sparsity

The client is now positioned to proceed with supervised learning to predict churn probability and strategize retention efforts.
