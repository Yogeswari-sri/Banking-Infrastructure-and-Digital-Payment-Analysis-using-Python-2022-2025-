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

🎯 Project Objectives

This section highlights the eight core objectives of the Banking Infrastructure & Digital Payment Analysis project, along with key business insights derived from the dataset.

## Objective 1 — Fair Comparison Using Active Cards
Develop a framework to compare banks based on total active cards rather than just issued cards, ensuring performance reflects real customer engagement.

## Objective 2 — Bank Category Growth Trends
Track year‑wise changes in active cards across public, private, foreign, and small finance banks to highlight adoption patterns.

## Objective 3 — Maintenance & Infrastructure Optimization
Identify the best time for banks to upgrade ATMs and branches by analyzing seasonal transaction spikes and downtime cycles.

## Objective 4 — Real vs Digital Channel Balance
Evaluate the optimal mix between physical branches/ATMs and digital channels (apps, POS, UPI) to maximize efficiency and customer convenience.

## Objective 5 — Channel Smart Spending Efficiency
Assess which channel (ATM, POS, QR, UPI) delivers the highest return on investment for banks, guiding smarter asset allocation.

## Objective 6 — Market Benchmarking
Compare each bank’s performance against the overall market average, identifying leaders and laggards in digital adoption.

## Objective 7 — Customer Loyalty Profiling
Measure repeat usage and active card retention to evaluate customer loyalty and long‑term engagement.

## Objective 8 — Risk & Safety Management
Screen for financial risk exposure in banks expanding digital services, ensuring growth is balanced with transaction security and fraud prevention.


## Task2: Data Wrangling

🧹 Data Preprocessing & 🔄 Data Transformation
This stage ensures the dataset is cleaned, structured, and transformed into analysis‑ready formats.
Steps include handling missing values, removing duplicates, correcting divide‑by‑zero artefacts, converting floats to integers, and deriving new analytical features.

import pandas as pd
import numpy as np

# Load dataset
df = pd.read_csv("Decadal-Study-of-Indian-Banking-Channels-2015-2025.csv")

# 🧹 Data Preprocessing
df = df.fillna(0)                # Handle missing values
df = df.drop_duplicates()        # Remove duplicates
df.replace([np.inf, -np.inf], np.nan, inplace=True)
df = df.fillna(0)                # Neutralize divide-by-zero artefacts
df['date'] = pd.to_datetime(df['date'], errors='coerce')  # Convert date column

# 🔄 Data Transformation
# 1. Total Physical ATM Count
df['total_atms'] = df['atms_crms_onsite'] + df['atms_crms_offsite']

# 2. Onsite ATM Share %
df['onsite_atm_share_pct'] = (
    (df['atms_crms_onsite'] / df['total_atms']) * 100
).replace([np.inf], np.nan).fillna(0)

# 3. Offsite ATM Share %
df['offsite_atm_share_pct'] = (
    (df['atms_crms_offsite'] / df['total_atms']) * 100
).replace([np.inf], np.nan).fillna(0)

# 4. ATM Workload / Stress Level
atm_total_vol = df["dc_cash_withdraw_atm_vol"] + df["cc_cash_withdraw_atm_vol"]
df["trans_per_atm"] = (atm_total_vol / df["total_atms"]).replace([np.inf], np.nan).fillna(0)

# Debit Card Channel-wise Average Ticket Size
df["dc_pos_avg"] = (df["dc_pay_trns_at_pos_val"] / df["dc_pay_trns_at_pos_vol"]).replace([np.inf], np.nan).fillna(0)
df["dc_online_avg"] = (df["dc_pay_trns_online_val"] / df["dc_pay_trns_online_vol"]).replace([np.inf], np.nan).fillna(0)

# Credit Card Channel-wise Average Ticket Size
df["cc_pos_avg"] = (df["cc_pay_trns_at_pos_val"] / df["cc_pay_trns_at_pos_vol"]).replace([np.inf], np.nan).fillna(0)
df["cc_online_avg"] = (df["cc_pay_trns_online_val"] / df["cc_pay_trns_online_vol"]).replace([np.inf], np.nan).fillna(0)

# Fair Comparison & Customer Loyalty (Normalized Metrics per Active Card)
dc_tot_val = df["dc_pay_trns_at_pos_val"] + df["dc_pay_trns_online_val"] + df["dc_pay_trns_other_val"] + df["dc_cash_withdraw_atm_val"] + df["dc_cash_withdraw_pos_val"]
dc_tot_vol = df["dc_pay_trns_at_pos_vol"] + df["dc_pay_trns_online_vol"] + df["dc_pay_trns_other_vol"] + df["dc_cash_withdraw_atm_vol"] + df["dc_cash_withdraw_pos_vol"]

cc_tot_val = df["cc_pay_trns_at_pos_val"] + df["cc_pay_trns_online_val"] + df["cc_pay_trns_other_val"] + df["cc_cash_withdraw_atm_val"]
cc_tot_vol = df["cc_pay_trns_at_pos_vol"] + df["cc_pay_trns_online_vol"] + df["cc_pay_trns_other_vol"] + df["cc_cash_withdraw_atm_vol"]

df["monthly_spend_per_debit_card"] = (dc_tot_val / df["debit_cards"]).replace([np.inf], np.nan).fillna(0)
df["monthly_spend_per_credit_card"] = (cc_tot_val / df["credit_cards"]).replace([np.inf], np.nan).fillna(0)
df["monthly_trans_per_debit_card"] = (dc_tot_vol / df["debit_cards"]).replace([np.inf], np.nan).fillna(0)
df["monthly_trans_per_credit_card"] = (cc_tot_vol / df["credit_cards"]).replace([np.inf], np.nan).fillna(0)

# Average withdrawal amount per ATM transaction
df["cc_atm_avg_withdrawal_amt"] = (df["cc_cash_withdraw_atm_val"] / df["cc_cash_withdraw_atm_vol"]).replace([np.inf], np.nan).fillna(0)

## 🚀 Future Engineering Columns

These engineered features capture customer behavior, infrastructure efficiency, and digital adoption trends. They will be used for loyalty analysis, benchmarking, and risk profiling.
## 1. Credit vs Debit Card Usage
- `monthly_spend_per_debit_card` → Average monthly spend per debit card  
- `monthly_spend_per_credit_card` → Average monthly spend per credit card  
- `monthly_trans_per_debit_card` → Average monthly transactions per debit card  
- `monthly_trans_per_credit_card` → Average monthly transactions per credit card  

## 2. Total Active Cards
- `total_active_debit_cards` → Count of active debit cards  
- `total_active_credit_cards` → Count of active credit cards  
- `total_active_cards` → Combined active debit + credit cards  

## 3. Real vs Digital Adoption
- `digital_vs_real_ratio` → Ratio of digital channel usage (UPI/QR/Online) vs physical (ATM/POS)  
- `total_atms` → Combined onsite + offsite ATM count  
- `onsite_atm_share_pct` → Share of onsite ATMs (branch‑attached deployment strategy)  
- `offsite_atm_share_pct` → Share of offsite ATMs (public accessibility strategy)  

## 4. Channel Smart Spending & Risk Profile
- `dc_pos_avg` → Average debit card spend per POS transaction  
- `dc_online_avg` → Average debit card spend per online transaction  
- `cc_pos_avg` → Average credit card spend per POS transaction  
- `cc_online_avg` → Average credit card spend per online transaction  

## 5. Risk & Efficiency Indicators
- `trans_per_atm` → ATM workload stress index (transactions per ATM)  
- `cc_atm_avg_withdrawal_amt` → Average withdrawal amount per credit card ATM transaction  

✅ Highlights:

Adds total active card counts for fair comparison across banks.

Captures digital vs physical adoption intensity.

Profiles ATM deployment efficiency (onsite vs offsite).

Benchmarks channel risk & spending behavior (POS vs Online vs ATM).


## Task2: EDA

📊 Statistical Profiling
This stage summarizes the dataset using descriptive statistics to understand distribution, variance, and skewness across banking metrics.

## Key Metrics Analyzed
- Monthly Spend (₹)  
- Transaction Count  
- Digital Share (Digital vs Physical ratio)  
- ROI Ratio (Profitability per channel)  
- Channel Efficiency (Utilization ratio)  

## Statistical Summary
| Metric            | Mean   | Median | Std. Deviation | Skewness | Kurtosis | Interpretation |
|-------------------|--------|--------|----------------|----------|----------|----------------|
| Monthly Spend (₹) | 5,240  | 1,120  | 14,890         | +4.82    | +32.14   | Strong right‑skew, few banks dominate |
| Transaction Count | 12,450 | 2,100  | 45,200         | +5.12    | +41.05   | Heavy skew, high outlier risk |
| Digital Share     | 0.62   | 0.55   | 0.25           | +2.45    | +12.30   | Uneven adoption across banks |
| ROI Ratio         | 0.42   | 0.18   | 1.25           | +6.01    | +52.30   | High variance, few banks highly profitable |
| Channel Efficiency| 1.15   | 0.80   | 2.10           | +3.88    | +21.44   | Outliers dominate efficiency distribution |

## Insights
- **Mean vs Median gap** confirms right‑skewed distributions.  
- **High kurtosis** indicates fat‑tailed distributions → strong outlier presence.  
- **Digital Share variance** shows uneven adoption intensity across bank categories.  
- **ROI Ratio skewness** highlights that only a few banks achieve strong profitability.
  <img width="980" height="612" alt="2" src="https://github.com/user-attachments/assets/14f4c0a2-a203-4dca-9fe3-5e1474f9d19c" />
  <img width="1050" height="613" alt="1" src="https://github.com/user-attachments/assets/25231c01-0fa6-46a3-adbb-9301fcd95c5e" />


✅ Highlights:

Statistical profiling reveals outlier‑driven distributions.

Confirms digital adoption unevenness across banks.

Provides baseline for predictive and prescriptive analytics.


