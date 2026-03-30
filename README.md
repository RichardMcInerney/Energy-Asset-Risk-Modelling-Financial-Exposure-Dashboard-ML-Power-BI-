🔍 Overview

This project delivers an end-to-end analytical solution for assessing and prioritising risk across global energy assets. It combines machine learning modelling (Python) with an interactive Power BI dashboard to provide clear, data-driven insights into:

Asset risk levels

Financial exposure

Key drivers of risk

The solution is designed to move beyond raw data and support real-world decision-making, enabling stakeholders to identify high-risk assets and allocate resources effectively.

<img width="1300" height="728" alt="Screenshot 2026-03-30 121108" src="https://github.com/user-attachments/assets/812a8f26-ea2b-49fa-8866-99fa6d212b48" />


🧠 Project Architecture
Data → Feature Engineering → ML Models → Predictions Export → Power BI Dashboard
Python (Colab) → model development
CSV outputs → integration layer
Power BI → business-facing analytics

📊 Executive Dashboard (Power BI)

<img width="1303" height="734" alt="Screenshot 2026-03-30 121457" src="https://github.com/user-attachments/assets/36b407d7-9b66-40ae-b97f-41842c7493cb" />


Key Capabilities:
Portfolio-level risk visibility
Financial exposure by fuel type and geography
Asset-level risk distribution
Interactive filtering (e.g. by country)

📈 Key KPIs

KPI	Description
Total Assets (29K)	Total number of energy assets analysed
Total Expected Loss (£1bn)	Estimated financial exposure across the portfolio
Avg Risk Score (15.68)	Average predicted risk level (0–100 scale)
Avg Claim Probability (47.56%)	Likelihood of a risk-related event

⚙️ Machine Learning Models

Two complementary models were developed:

🔹 Regression Model (Risk Scoring)
Predicts continuous Risk Score (0–100)
Used for ranking and prioritisation
🔹 Classification Model (Risk Detection)
Predicts probability of a risk event
Used for screening high-risk assets

📉 Model Performance Dashboard

<img width="1297" height="729" alt="Screenshot 2026-03-30 121514" src="https://github.com/user-attachments/assets/6efa8d33-9f42-43c9-8425-3cf44368c950" />


Key Results:
Metric	Value	Meaning
R² = 0.86	Strong predictive accuracy	
RMSE = 4.34	Low prediction error	
ROC AUC = 0.65	Moderate classification capability	
Recall = 0.56	Detects over half of high-risk cases	

🧠 Model Selection Strategy

Rather than forcing a single “best” model:

Gradient Boosting → best for risk scoring (regression)
Random Forest → slightly better for classification

👉 Final approach:

Gradient Boosting is used as the primary model for risk scoring, with Random Forest supporting classification-based screening

🔎 Risk Drivers Analysis

Top Drivers of Risk:
Asset Age
Capacity × Age interaction
Capacity (MW)
Fuel volatility
Legacy asset indicators

👉 Insight:

Older, high-capacity assets present the greatest risk concentration.

📊 Key Business Insights

1. Financial Exposure
Highest losses concentrated in:
Coal
Gas
Oil
2. Geographic Risk Concentration
Countries like:
United States
China
India

show the highest exposure levels.

3. Asset Risk Distribution
Majority = Low Risk
Small subset = High Impact / High Priority
4. Capacity vs Risk Relationship
Larger assets = higher financial exposure
Moderate correlation with risk score

🧾 Model Outputs (CSV Files)

<img width="1910" height="913" alt="Screenshot 2026-03-30 124155" src="https://github.com/user-attachments/assets/34b1ce6a-13c9-4a59-8082-0ee940388a7a" />


Generated from the notebook:

energy_asset_risk_predictions.csv
energy_asset_risk_summary_by_country.csv
energy_asset_risk_summary_by_fuel.csv
combined_feature_importance.csv
regression_model_results.csv
classification_model_results.csv
🧪 Notebook & Pipeline

Features:
Full ML pipeline (EDA → training → evaluation)
Model comparison (RF vs GB)
Export-ready outputs for BI integration
⚠️ Disclaimer

This project uses synthetic target variables to simulate risk outcomes.

It is intended to demonstrate:

modelling approach
analytical thinking
business integration

👉 Not real-world predictive deployment.

🚀 Tools & Technologies
Python (Pandas, Scikit-learn)
Google Colab
Power BI
DAX
Machine Learning (Regression + Classification)

📁 Project Structure
/notebooks        → ML model (Colab)
/data             → Processed datasets & outputs
/dashboard        → Power BI (.pbix)
/images           → Screenshots for README
/report           → Whitepaper & analysis

💼 Business Value

This solution enables:

Risk-based asset prioritisation
Financial exposure awareness
Data-driven maintenance planning
Transparent, explainable modelling
