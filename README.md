# 🔋 Energy Asset Risk Modelling & Financial Exposure Dashboard (ML + Power BI)

---

## 🔍 Overview

This project delivers an **end-to-end analytical solution** for assessing and prioritising risk across global energy assets.

It combines:

- Machine Learning (Python / Google Colab)  
- Financial exposure modelling  
- Interactive Power BI dashboard  

to provide clear, data-driven insights into:

- Asset risk levels  
- Financial exposure  
- Key drivers of risk  

The solution is designed to support **real-world decision-making**, enabling stakeholders to identify high-risk assets and allocate resources effectively.

---

## 🧠 Project Architecture

Data → Feature Engineering → ML Models → Predictions Export → Power BI Dashboard


- Python (Colab) → model development  
- CSV outputs → integration layer  
- Power BI → business-facing analytics  

---

## 📊 Executive Dashboard

<img width="1300" height="728" alt="Screenshot 2026-03-30 121108" src="https://github.com/user-attachments/assets/e3b5dc95-1773-4082-8ca7-12060830a8ff" />


### Key Capabilities

- Portfolio-level risk visibility  
- Financial exposure by fuel type and geography  
- Asset-level risk distribution  
- Interactive filtering (e.g. country-level analysis)  

---

## 📈 Key KPIs

| KPI | Description |
|-----|------------|
| **Total Assets (29K)** | Total number of energy assets analysed |
| **Total Expected Loss (£1bn)** | Estimated financial exposure across the portfolio |
| **Avg Risk Score (15.68)** | Average predicted risk level (0–100 scale) |
| **Avg Claim Probability (47.56%)** | Likelihood of a risk-related event |

---

## ⚙️ Machine Learning Models

Two complementary models were developed:

### 🔹 Regression Model (Risk Scoring)
- Predicts continuous **Risk Score (0–100)**  
- Used for **ranking and prioritisation**

### 🔹 Classification Model (Risk Detection)
- Predicts probability of a **risk event**  
- Used for **screening high-risk assets**

---

## 📉 Model Performance

<img width="1303" height="734" alt="Screenshot 2026-03-30 121457" src="https://github.com/user-attachments/assets/60318b81-3448-47a7-9012-5eba89062639" />


### Key Results

| Metric | Value | Interpretation |
|--------|------|---------------|
| **R²** | 0.86 | Strong predictive accuracy |
| **RMSE** | 4.34 | Low prediction error |
| **ROC AUC** | 0.65 | Moderate classification performance |
| **Recall** | 0.56 | Detects over half of high-risk cases |

---

## 🧠 Model Selection Strategy

Rather than forcing a single “best” model:

- **Gradient Boosting** → strongest for **risk scoring (regression)**  
- **Random Forest** → slightly stronger for **classification**

### Final Approach

> Gradient Boosting is used as the **primary model for risk scoring**,  
> while Random Forest supports **classification-based screening**

---

## 🔎 Risk Drivers Analysis

<img width="1297" height="729" alt="Screenshot 2026-03-30 121514" src="https://github.com/user-attachments/assets/c4f67f67-4be3-4fad-8987-9621b1e517e2" />


### Key Drivers of Risk

- Asset Age  
- Capacity × Age interaction  
- Capacity (MW)  
- Fuel volatility  
- Legacy asset indicators  

### Insight

> Older, high-capacity assets represent the highest risk concentration within the portfolio.

---

## 📊 Key Business Insights

### 1. Financial Exposure

- Highest losses concentrated in:
  - Coal  
  - Gas  
  - Oil  

---

### 2. Geographic Risk Concentration

Countries with highest exposure:

- United States  
- China  
- India  

---

### 3. Asset Risk Distribution

- Majority of assets = **Low Risk**  
- Small subset = **High Risk (high impact)**  

---

### 4. Capacity vs Risk

- Larger assets → higher financial exposure  
- Moderate correlation with risk score  

---

## 🧾 Model Outputs (CSV Files)

Generated from the notebook:

- `energy_asset_risk_predictions.csv`  
- `energy_asset_risk_summary_by_country.csv`  
- `energy_asset_risk_summary_by_fuel.csv`  
- `combined_feature_importance.csv`  
- `regression_model_results.csv`  
- `classification_model_results.csv`  

---

## 🧪 Notebook & Pipeline

<img width="1910" height="913" alt="Screenshot 2026-03-30 124155" src="https://github.com/user-attachments/assets/9df42007-f24a-48f0-8adb-7c626c3cd969" />


### Features

- Full ML pipeline (EDA → training → evaluation)  
- Model comparison (Random Forest vs Gradient Boosting)  
- Export-ready outputs for Power BI integration  

---

## ⚠️ Disclaimer

This project uses **synthetic target variables** to simulate risk outcomes.

It is intended to demonstrate:

- modelling approach  
- analytical thinking  
- business integration  

> Not real-world predictive deployment.

---

## 🚀 Tools & Technologies

- Python (Pandas, Scikit-learn)  
- Google Colab  
- Power BI  
- DAX  
- Machine Learning (Regression + Classification)  

---

## 📁 Project Structure

/notebooks → ML model (Colab)
/data → Processed datasets & outputs
/dashboard → Power BI (.pbix)
/images → Screenshots for README
/report → Whitepaper & analysis


---

## 💼 Business Value

This solution enables:

- Risk-based asset prioritisation  
- Financial exposure visibility  
- Data-driven maintenance planning  
- Transparent, explainable modelling  

---

## 🏁 Conclusion

This project demonstrates a complete, scalable approach to **energy asset risk assessment**, combining machine learning with business intelligence to support **practical, data-driven decision-making**.

---
