<div align="center">

# 🏦 Banking Infrastructure & Digital Payment Analysis (2022–2025)

📊 **Python + Power BI Capstone Project**

👩‍💻 Prepared by: **Yogeswari K**  
🎓 Course: Programme in AI Driven Data Analytics, Entri  

</div>

---

## 📌 Project Overview
This project presents a **Python‑based exploratory, statistical, and business intelligence analysis** of Indian banking transactions and digital adoption trends between 2022–2025.  

Workflow includes:
- Data Cleaning & Preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature Engineering  
- Statistical Profiling  
- Data Visualization (Python + Power BI)  
- Business Insights & Recommendations  

---
## Task1: Problem Statement & Business Understanding
<div align="center">

## 📝 Problem Statement

Banks and policymakers often have access to large volumes of raw transaction data but lack a structured framework to convert it into actionable insights.  
This project applies a complete Python data‑analytics pipeline to RBI transaction records, identifying growth trends, digital adoption ratios, seasonal anomalies, and translating findings into **prescriptive business recommendations**.

</div>

---

## 📂 Dataset
| Details   | Value |
|-----------|-------|
| Dataset   | Decadal Study of Indian Banking Channels (2015–2025) |
| Source    | RBI Bankwise ATM & POS Transactions |
| Records   | ~350 MB CSV |
| Features  | 30+ Columns (ATM, POS, QR, UPI, Debit/Credit transactions) |
| Storage   | GitHub + Git LFS |
| Environment | Google Colab / Jupyter Notebook |

---

<div align="left">

## 🛠 Tools & Technologies

**Python** (Pandas, NumPy, Matplotlib, Seaborn)  
**Power BI** (Interactive dashboards)  
**Google Colab** (Analysis environment)  
**GitHub + Git LFS** (Version control & dataset hosting)

</div>

---

📂 Column Dictionary

This section provides a clear description of each column in the Banking Infrastructure & Digital Payment Analysis (2022–2025) dataset. It helps recruiters and reviewers quickly understand the dataset structure and the meaning of each field.
| Column | Description |
|--------|-------------|
| id | Unique identifier for each bank record |
| date | Reporting date (month/year) of transaction data |
| bank_category | Classification of bank (Public, Private, Foreign, etc.) |
| bank_name | Official name of the bank |
| atms_crms_onsite | Number of onsite ATMs/CRMs within branch premises |
| atms_crms_offsite | Number of offsite ATMs/CRMs outside branch premises |
| pos | Total POS terminals deployed by the bank |
| micro_atms | Count of micro‑ATMs used for rural transactions |
| bharat_qr | Number of Bharat QR codes issued or active |
| upi_qr | Number of UPI QR codes issued or active |
| credit_cards | Total credit cards issued by the bank |
| debit_cards | Total debit cards issued by the bank |
| cc_pay_trns_at_pos_vol | Volume of credit card transactions at POS terminals |
| cc_pay_trns_at_pos_val | Value of credit card transactions at POS terminals |
| cc_pay_trns_online_vol | Volume of credit card online transactions |
| cc_pay_trns_online_val | Value of credit card online transactions |
| cc_pay_trns_other_vol | Volume of credit card transactions through other channels |
| cc_pay_trns_other_val | Value of credit card transactions through other channels |
| cc_cash_withdraw_atm_val | Value of credit card cash withdrawals at ATMs |
| cc_cash_withdraw_atm_vol | Volume of credit card cash withdrawals at ATMs |
| dc_pay_trns_at_pos_vol | Volume of debit card transactions at POS terminals |
| dc_pay_trns_at_pos_val | Value of debit card transactions at POS terminals |
| dc_pay_trns_online_vol | Volume of debit card online transactions |
| dc_pay_trns_online_val | Value of debit card online transactions |
| dc_pay_trns_other_vol | Volume of debit card transactions through other channels |
| dc_pay_trns_other_val | Value of debit card transactions through other channels |
| dc_cash_withdraw_atm_val | Value of debit card cash withdrawals at ATMs |
| dc_cash_withdraw_atm_vol | Volume of debit card cash withdrawals at ATMs |
| dc_cash_withdraw_pos_val | Value of debit card cash withdrawals at POS terminals |
| dc_cash_withdraw_pos_vol | Volume of debit card cash withdrawals at POS terminals |

-----

🎯 Analytical Objectives & Insights
This section highlights the eight core objectives of the Banking Infrastructure & Digital Payment Analysis project, along with key business insights derived from the dataset.
## Objective 1 — Fair Comparison Using Active Cards
- Compare banks based on active card usage, not just issued cards  
- Public banks lead adoption with highest active card counts  
- Private banks competitive in urban segments  
- Payment banks weakest in retention  

---

## Objective 2 — Bank Category Growth Trends
- Year‑wise active card growth analysis (2022–2025)  
- SBI consistently ranked best, peaking in 2023  
- Decline in 2024–25 highlights retention challenges  

---

## Objective 3 — Real vs Digital Channel Balance
- Digital vs branch ratio across categories  
- Private banks show healthy hybrid mix  
- Public banks slower digital shift  
- Small Finance banks extremely digital, Payment banks almost fully physical  

---

## Objective 4 — Channel Smart Spending Efficiency
- Correlation analysis between ATMs, POS, Bharat QR, UPI QR  
- POS + Bharat QR synergy → strongest ROI driver  
- UPI QR evolving independently as future digital engine  

---

## Objective 5 — Maintenance & ATM Stress
- Onsite ATMs carry higher maintenance load → quarterly checks  
- Offsite ATMs under‑utilized → half‑yearly checks sufficient  
- Overall ATM stress line ~2.4% → infra under‑utilized  

---

## Objective 6 — Bank Market Benchmarking
- Private banks dominate debit spend  
- Foreign banks balanced debit + credit spend  
- Public banks lag in credit adoption  
- Payment banks negligible spend  

---

## Objective 7 — Customer Loyalty Profiling
- Private sector banks show strongest loyalty (HDFC, ICICI, Axis)  
- Foreign banks premium but concentrated risk  
- Public banks weaker engagement  
- Payment banks lowest retention  

---

## Objective 8 — Risk & Safety Management
- Cash‑heavy banks face concentrated risk  
- Airtel Payments Bank safest with digital focus  
- American Express → high‑value withdrawals, concentrated risk  
- Balanced adoption in Au Small Finance & Axis Bank  


## Task2: Data Wrangling
## 🧹 Data Preprocessing
```python
import pandas as pd
import numpy as np

# Load dataset
df = pd.read_csv("Decadal-Study-of-Indian-Banking-Channels-2015-2025.csv")

# Handle missing values
df = df.fillna(0)

# Remove duplicates
df = df.drop_duplicates()

# Neutralize divide-by-zero artefacts
df.replace([np.inf, -np.inf], np.nan, inplace=True)
df = df.fillna(0)

# Convert date column
df['date'] = pd.to_datetime(df['date'], errors='coerce')

