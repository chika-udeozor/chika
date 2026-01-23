# Fraud Detection and Transaction Risk Analysis (Python)

Exploratory and predictive analytics project using Python to analyze financial transaction data, identify fraud patterns, and evaluate key risk indicators that support data-driven fraud detection decisions.

---

## Project Overview
Financial transaction fraud presents significant operational and financial risk for organizations.  
This project applies exploratory data analysis and predictive modeling techniques to understand fraud trends, identify high-risk transaction characteristics, and evaluate the relationship between transaction behavior and risk indicators.

The analysis supports fraud monitoring and risk-based decision-making beyond traditional rule-based approaches.

---

## Business Understanding (5W & 1H)

**Who:**  
Customers affected by fraud, fraud operations teams, and risk & compliance teams  

**What:**  
Identify patterns and indicators associated with fraudulent financial transactions  

**When:**  
During transaction processing and ongoing fraud monitoring  

**Where:**  
Across transaction types, merchant categories, and countries  

**Why:**  
To reduce financial losses, operational costs, and protect customer trust  

**How:**  
Using exploratory data analysis and regression-based predictive modeling  

---

## Data Understanding

- **Source:** Synthetic Financial Fraud Dataset (Kaggle)
- **Records:** 10,000 transactions
- **Variables:** 10

### Key Features
- **Transaction Details:** amount, hour
- **Risk Indicators:** device_risk_score, ip_risk_score
- **Transaction Attributes:** transaction_type, merchant_category, country
- **Target Variable:** is_fraud (0 = non-fraud, 1 = fraud)

All analysis was conducted using Python.

---

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Data Cleaning Summary
- Checked for missing values and duplicate records
- Validated transaction amount, hour, and risk score ranges
- Verified binary fraud labels
- Ensured correct data types for all variables

---

## Exploratory Analysis & Visual Insights

Key visual analyses included:
- Distribution of transaction amounts
- Transaction amount comparison by fraud status
- Average fraud rate by transaction type
- Average fraud rate by country
- Relationship between transaction amount and device risk score

### Key Observations
- Fraudulent transactions tend to have higher transaction amounts
- Fraud occurs across all transaction types, indicating the need for consistent controls
- Fraud rates vary by country, highlighting geographic risk differences
- High transaction amounts combined with high device risk scores indicate elevated fraud risk

---

## Predictive & Analytical Questions
- Which transaction characteristics explain device risk score?
- Do risk indicators explain transaction amount?
- How strongly does IP risk score explain device risk score?
- How strongly does transaction amount explain device risk score?

Regression analysis shows that transaction amount and IP risk score significantly explain device risk score, confirming the value of risk signals in fraud detection.

---

## Key Insights & Recommendations
- High transaction amounts and elevated risk scores are strongly associated with fraud
- Fraud controls should be applied consistently across transaction types
- Geographic location should be incorporated carefully into fraud monitoring
- IP and device risk signals should be prioritized for high-value transactions in real time

---

## Deliverables
- Cleaned transaction dataset
- Python exploratory analysis notebook
- Fraud risk visualizations
- Regression-based analytical insights

---

## Project Summary
This project demonstrates the use of Python-based exploratory and predictive analytics to support fraud detection and transaction risk assessment. The findings highlight the importance of combining transaction value with device and IP risk indicators to improve real-time fraud monitoring decisions.

---

## How to Reproduce
1. Load the dataset from the `data/` folder.
2. Open the notebook in `notebooks/`.
3. Run all cells to reproduce cleaning, visualizations, and analysis.

---

## Data Source
- Umitka. (2024). Synthetic Financial Fraud Dataset. Kaggle.  
  https://www.kaggle.com/datasets/umitka/synthetic-financial-fraud-dataset

---

## Project Status
Completed – academic analytics project demonstrating Python-based exploratory and predictive analysis.

