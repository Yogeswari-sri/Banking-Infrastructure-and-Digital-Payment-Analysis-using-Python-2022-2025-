# 🏦 Banking Infrastructure & Digital Payment Analysis (2022–2025)  
### 📊 Python + Power BI Capstone Project  

👩‍💻 Prepared by: **Yogeswari K**  
🎓 Course: Programme in AI Driven Data Analytics, Entri  

---

### 🚀 RBI Dataset • 2022–2025 • End‑to‑End Analytics  

🔎 **Descriptive → Diagnostic → Predictive → Prescriptive**  
💡 Turning raw banking data into actionable insights  

---

📌 **Highlights**
- 8 Visualization Objectives (ATM, POS, QR, UPI, Loyalty, Risk)  
- 10+ Engineered Features (Active Cards, Stress Index, ROI Ratios)  
- Four‑Layer Analytics Framework for strategic recommendations  
- Recruiter‑friendly README with insights, findings, and business roadmap  

----

## 🔗 Navigation  

- [Executive Summary](#executive-summary)  
- [Industry Context](#industry-context)  
- [Problem Statement](#problem-statement)  
- [Project Objectives](#project-objectives)  
- [Dataset Description](#dataset-description)  
- [Tools & Technologies](#tools--technologies)
- [Python Data Analytics Workflow](#project-workflow) 
- [Data Preprocessing](#data-preprocessing)  
- [Feature Engineering](#feature-engineering)  
- [Visualization Objectives](#visualization-objectives)  
- [Four-Layer Analytics Framework](#four-layer-analytics-framework)  
- [Key Findings — Consolidated](#key-findings--consolidated)  
- [Business Recommendations](#business-recommendations)  
- [Limitations of the Study](#limitations-of-the-study)  
- [Conclusion](#conclusion)  
- [Project Files & Access](#project-files--access)
- [Power BI Dashboard – Banking Infrastructure & Digital Payment (2022–2025)](#PowerBI-Dashboard)

  

## Executive Summary

This project analyzes Indian banking infrastructure and digital payment adoption between 2022–2025 using RBI datasets.  
It benchmarks banks on **ATM stress, POS + QR ROI, UPI QR adoption, customer loyalty, and risk exposure**, delivering recruiter‑friendly insights and recommendations.  

The study demonstrates how **Python (Pandas, NumPy, Matplotlib, Seaborn)** can be applied to transform raw datasets into **strategic insights** for banks, policymakers, and regulators.  

---

## Industry Context
 
The Indian banking sector (2022–2025) is undergoing rapid transformation:  
- **Digital Payments Boom** → UPI, QR, and online channels driving transaction growth.  
- **ATM & POS Infrastructure** → Still critical for cash‑based segments, but facing stress.  
- **Customer Behavior Shift** → Credit card adoption rising, debit card usage stabilizing.  
- **Regulatory Push** → RBI promoting financial inclusion, digital adoption, and fraud risk management.  
- **Competitive Landscape** → Banks competing on digital efficiency, loyalty programs, and infrastructure modernization.  

---

##  Problem Statement  

## Task1: Problem Statement & Business Understanding
<div align="left">

Despite rapid growth in digital payments (UPI, QR, online channels),  
Indian banks face **three major challenges**:

1. **ATM Infrastructure Stress**  
   - High workload per ATM, limited expansion, and rising maintenance costs.  

2. **Unbalanced Digital vs Physical Adoption**  
   - Urban centers show strong digital penetration, but rural branches remain cash‑dependent.  

3. **Customer Loyalty & Risk Exposure**  
   - Credit card adoption rising, but customer risk persists.  
   - Fraud vulnerability linked to outdated infrastructure and low digital adoption.  

</div>

-----
## Project Objectives

This project presents a Python‑based exploratory, statistical, and business intelligence analysis of Indian banking transactions and digital adoption trends between 2022–2025.  

This section highlights the eight core objectives of the Banking Infrastructure & Digital Payment Analysis project, along with key business insights derived from the dataset.

## Objective 1 — Fair Comparison Using Active Cards
Develop a framework to compare banks based on total active cards rather than just issued cards, ensuring performance reflects real customer engagement.

## Objective 2 — Year-wise ROI
Track Track year‑wise highest ROI which returns to Physical Vs Digitally Investment.

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

---
## Dataset Description

| **Attribute**   | **Details** |
|-----------------|-------------|
| **Source**      | Reserve Bank of India (RBI) published datasets (2022–2025) |
| **Scope**       | Banking infrastructure, card usage, ATM/POS terminals, QR/UPI transactions, debit & credit spending patterns |
| **Granularity** | Yearly + quarterly transaction volumes, balances, and infrastructure counts |
| **Period**      | 2022–2025 |
| **File Format** | Excel / CSV |
| **Environment** | Python (Jupyter Notebook) + Power BI |
| **Link:**       | [https://drive.google.com/drive/folders/1Dcf209_M68RG_CIUWIYA9ZuGPV3Hfd81?usp=drive_link] |
---

## 🔑 Key Features Extracted

| **Feature**                  | **Description** |
|-------------------------------|-----------------|
| **Active Cards**              | Debit & Credit card counts and usage |
| **ATM & POS Terminals**       | Deployment, usage, and growth trends |
| **QR & UPI Transactions**     | Digital payment adoption metrics |
| **Digital vs Physical Ratios**| Balance between cash vs digital transactions |
| **ROI Drivers**               | POS + QR efficiency indicators |
| **ATM Stress Index**          | Maintenance vs usage pressure |
| **Customer Loyalty Metrics**  | Profiling based on active card engagement |
| **Risk & Safety Indicators**  | Fraud exposure, infrastructure gaps |

  ---

<div align="left">

## Tools & Technologies

This project leverages a **Python data analysis stack** with industry‑standard libraries:

- **Python 3.x** → Core programming language  
- **Pandas** → Data wrangling, preprocessing, feature engineering  
- **NumPy** → Numerical operations & handling divide‑by‑zero artefacts  
- **Matplotlib** → Visualizations (line charts, barplots, scatter plots)  
- **Seaborn** → Advanced statistical plots (pair plots, heatmaps)  
- **Jupyter Notebook** → Interactive analysis & documentation  

</div>

---

## Python Data Analytics Workflow

📥 Data Ingestion  
   ↓  
🔍 Data Inspection  
   ↓  
🧹 Data Cleaning  
   ↓  
🔄 Data Transformation  
   ↓  
⚙️ Feature Engineering  
   ↓  
📊 Exploratory Data Analysis (EDA)  
   ↓  
📈 Statistical Analysis  
   ↓  
📉 Data Visualization  
   ↓  
💡 Insights Generation  
   ↓  
🗂️ Decision Making

----

## 📂 Attribute / Column Dictionary

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

## Task 2: Data Wrangling  
## Data Preprocessing  

Steps applied to clean and prepare the dataset before feature engineering:

1. **Handle Missing Values**  
   - `fillna(0)` → Replace nulls with zero for consistency.  

2. **Remove Duplicates**  
   - `drop_duplicates()` → Avoid repeated records.  

3. **Replace Infinite Values**  
   - `replace([np.inf, -np.inf], np.nan)` → Handle divide‑by‑zero artefacts.  

4. **Neutralize NaN Values**  
   - `fillna(0)` → Ensure dataset remains numeric and usable.  

5. **Convert Date Column**  
   - `pd.to_datetime(errors="coerce")` → Standardize date formats.  

👉 Purpose: Ensures dataset is **clean, consistent, and analysis‑ready** for transformation and visualization.

---

## Feature Engineering 

This stage focuses on transforming raw banking transaction data into derived analytical features that capture customer behavior, infrastructure efficiency, and digital adoption intensity. These engineered metrics enable loyalty analysis, benchmarking, and risk profiling across banks.

---

### 1. Credit vs Debit Card Usage
- `monthly_spend_per_debit_card`  
- `monthly_spend_per_credit_card`  
- `monthly_trans_per_debit_card`  
- `monthly_trans_per_credit_card`  

👉 Compare debit vs credit adoption.  

---

### 2. Total Active Cards
- `total_active_debit_cards`  
- `total_active_credit_cards`  
- `total_active_cards`  

👉 Benchmark active usage vs issued cards.  

---

### 3. Real vs Digital Adoption
- `digital_vs_real_ratio`  
- `total_atms`  
- `onsite_atm_share_pct`  
- `offsite_atm_share_pct`  

👉 Measure digital intensity & ATM efficiency.  

---

### 4. Channel Smart Spending
- `dc_pos_avg`  
- `dc_online_avg`  
- `cc_pos_avg`  
- `cc_online_avg`  

👉 Profile POS vs Online risk & spending.  

---

### 5. Risk & Efficiency Indicators
- `trans_per_atm`  
- `cc_atm_avg_withdrawal_amt`  

👉 Detect ATM stress & cash‑heavy risk.  

---

✅ **Highlights**
- Fair comparison across banks.  
- Digital vs physical adoption clarity.  
- ATM deployment efficiency.  
- Channel risk benchmarking.

-----

## Exploratory Data Analysis (EDA)
## Task3:

Visualizations help in understanding customer spending, digital adoption, and infrastructure efficiency. They also reveal skewness and kurtosis patterns in the dataset.

## 📊 Statistical Profiling
This stage summarizes the dataset using descriptive statistics to understand distribution, variance, and skewness across banking metrics.

## Key Metrics Analyzed
- Monthly Spend (₹)  
- Transaction Count  
- Digital Share (Digital vs Physical ratio)  
- ROI Ratio (Profitability per channel)  
- Channel Efficiency (Utilization ratio)  

## Statistical Summary
<img width="1100" height="503" alt="image" src="https://github.com/user-attachments/assets/a786ba76-b98d-43ec-9dea-541670da926f" />
<img width="975" height="816" alt="image" src="https://github.com/user-attachments/assets/43663533-76a1-4afa-8b32-d3b0a53f0caa" />

## Insights
- **Mean vs Median gap** confirms right‑skewed distributions.  
- **High kurtosis** indicates fat‑tailed distributions → strong outlier presence.  
- **Digital Share variance** shows uneven adoption intensity across bank categories.  
- **ROI Ratio skewness** highlights that only a few banks achieve strong profitability.
  
## 📐 Skewness & Kurtosis (Project Context)
These measures describe the shape and balance of banking channel distributions. They highlight whether customer spending and transactions are evenly spread or dominated by extreme outliers.
## 🔹 Skewness → Symmetry / Tilt
<img width="1102" height="461" alt="image" src="https://github.com/user-attachments/assets/7bfdc00e-deb4-4e28-ae54-0ed494662676" />

- **Definition:** Shows whether data is balanced or tilted.  
- **Positive skew:** Right‑heavy → many small spends, few extreme large spends.  
- **Negative skew:** Left‑heavy → many large spends, few very small spends.  
- **Zero skew:** Perfectly balanced (mean ≈ median).


## 👉 Project Insight:  
- **Debit card usage** → often **positive skew** → majority of customers transact small amounts, few heavy spenders dominate.  
- **Credit card usage** → closer to **zero skew** → balanced adoption across active users.  

---

## 🔹 Kurtosis → Outlier Impact / Tail Heaviness
<img width="1077" height="421" alt="image" src="https://github.com/user-attachments/assets/7dc9c5ba-b761-4bfa-81ab-673b07d80d6e" />

- **Definition:** Shows whether extreme outliers dominate the distribution.  
- **High kurtosis:** Heavy tails → few extreme outliers drive results.  
- **Low kurtosis:** Flat tails → balanced, no extreme spikes.  
- **Normal kurtosis (~3):** Near‑normal distribution.  

👉 Project Insight:  
- **Debit card spend** → **high kurtosis** → few heavy users drive overall spend.  
- **Credit card spend** → **near‑normal kurtosis** → balanced, less outlier domination.  
- **Digital vs Real ratio** → skewed towards branch‑heavy public banks, while private banks show balanced kurtosis with hybrid adoption. 

## Summary and Key Insights

Skewness tells tilt → whether spending is dominated by small vs large transactions.

Kurtosis tells outlier impact → whether extreme users dominate or usage is balanced.

Together, they explain customer loyalty, adoption imbalance, and risk concentration in Indian banking channels.

## Visualization Objectives

The goal of visualization is to convert engineered features into **clear, actionable insights**.  
Key objectives include:

## 1️⃣ Fair Comparison Using Active Cards

### 🎯 Goal: Compare banks fairly by measuring active card usage instead of just issued cards, ensuring performance reflects real customer engagement.

## 📈 Visualization

Barplot / Stacked Bar / Pie Chart

Compare total active debit vs credit cards across bank categories.

Highlights engagement vs capacity (issued cards).

## Visual:
<img width="702" height="517" alt="3" src="https://github.com/user-attachments/assets/dc02c4fd-4973-4d72-90e1-eb95da056180" />


### Chart Interpretation (Active Cards by Bank Category)

- **Interpretation →** Comparing banks by active cards shows **real customer engagement**, not just bank size.  
- **Key Insight →** Large banks may issue many cards, but only **active cards prove usage**.  
- **Pattern →** Public banks lead with the highest active cards, private banks are strong but slower, small finance & foreign banks remain niche, payment banks weakest.  
- **Trend →** Active card count highlights **adoption differences** across categories.  
- **Observation →** Fair comparison = focus on **engagement (active cards)** instead of **capacity (bank size)**.  

## 📌 Key Business Insights

Public banks dominate active card usage → strong penetration in mass markets.

Private banks competitive but slower in scale → urban/premium focus.

Small finance & foreign banks → niche adoption.

Payment banks weakest → structural retention challenges.

Univariate analysis confirms engagement differences across categories.

## 2️⃣ 2. Year-wise ROI Performance
### 🎯 Goal: Track year‑wise highest ROI which returns to Physical Vs Digitally Investment?.

## 📈 Visualization
Line Chart / Trend Plot

Compare ayear‑wise ROI (2022–2025).

Identify best performing ROI each year.

## Visual:
<img width="1039" height="668" alt="image" src="https://github.com/user-attachments/assets/7fd76717-ed78-423f-a8b8-c25d0cee3fc7" />

### Chart Interpretation (Year‑wise Active Cards)

- **Interpretation →** Line chart shows growth/decline in the year of across categories.  
- **Key Insight →** 2025 consistently ranked best by moves Digitally and their ROI is 16.35%.  
- **Pattern →** 2025 year (16.35% ROI), then declined in 2024–2025.  
- **Trend →** Initial growth momentum followed by decline → signals customer migration or reduced activity.  
- **Observation →** Growth trends highlight need for **digital adoption + retention strategies**.  

### ROI Analysis (2022-2025)
##📌 Key Business Insights
2025 gave the highest ROI = 16.25%, proving digital infra investments yielded maximum returns that year.
## Pattern
ROI shows a growth → peak → decline → recovery cycle, with 2025 marking the strongest recovery point.
## Trend 
From 2022-2024 ROI remained low/negative, but 2025 upward trend highlights customer shift toward cashless channels (POS, QR, Online).
## Observation
Overall ROI peaked in 2025 (16.25%), confirming banks benefited most from digital adoption, while ATM-based infra lagged behind.


## 3️⃣ Real vs Digital Channel Balance
### 🎯 Goal: Evaluate the optimal mix between physical branches/ATMs and digital channels (apps, POS, UPI) to maximize efficiency and customer convenience.

## 📈 Visualization
Scatter Plot / Barplot

Compare Digital vs Real Ratio across bank categories.

Spot extremes (too digital vs too branch‑heavy) and highlight hybrid models.

## Visual:
<img width="834" height="505" alt="image" src="https://github.com/user-attachments/assets/23d7e6a4-3791-47fa-aef2-dd79d1fc20ec" />

<img width="543" height="399" alt="image" src="https://github.com/user-attachments/assets/0dfdddef-dcd8-4985-9384-380adf32fded" />

### Chart Interpretation (Digital vs Real Ratio)

- **Interpretation →** Scatter plot shows balance between digital adoption (UPI/QR/Online) and physical infra (ATMs/Branches).  
- **Key Insight →** Small Finance Banks extremely digital (ratio > 400), Payment & Foreign Banks remain branch‑heavy.  
- **Pattern →** Private Banks (~100) show healthiest hybrid mix, Public Banks (~70) slower digital shift.  
- **Trend →** Market is uneven — digital adoption rising, but hybrid models prove most sustainable.  
- **Observation →** Strong digital apps = convenience, but branch presence = trust & inclusion.  

## 📌 Key Business Insights
Small Finance Banks → Digital‑dominant, minimal branch presence.

Private Banks → Balanced hybrid model (apps + branches).

Public Banks → Branch‑oriented, lagging in digital modernization.

Payment Banks → Weak digital adoption, almost fully physical.

Foreign Banks → Nearly all branch‑based, minimal digital.

## 4️⃣ Channel Smart Spending Efficiency
### 🎯 Goal: Assess which channel (ATM, POS, Bharat QR, UPI QR) delivers the highest ROI, and identify correlations between physical vs digital infrastructure to guide smarter asset allocation.

## 📈 Visualization
Correlation Heatmap

Compare Onsite vs Offsite ATMs, POS terminals, Bharat QR, and UPI QR.

Identify synergies, independent growth paths, and ROI drivers.

## Visual:
<img width="947" height="727" alt="image" src="https://github.com/user-attachments/assets/9c41c62c-5c84-4838-bd24-5b0f06243abc" />

### Chart Interpretation (Channel Correlation Heatmap)

- **Interpretation →** Heatmap shows how physical and digital channels grow together or independently.  
- **Key Insight →** Onsite & Offsite ATMs strongly correlated (0.905), POS + Bharat QR moderately correlated (0.683), UPI QR weak correlation (independent growth).  
- **Pattern →** POS + QR synergy acts as the immediate profit driver, while UPI QR evolves independently as the future digital engine.  
- **Trend →** Banks balancing physical infra for stability + POS/QR for ROI will outperform.  
- **Observation →** Smart spending = diversify → maintain ATMs for trust, expand POS/QR for profit, prepare UPI QR for long‑term growth.  

 ## 📌 Key Business Insights
ATM Expansion → Onsite & Offsite ATMs grow together, supporting debit base but limited ROI in digital growth.

POS + Bharat QR Synergy → Moderate correlation, strongest ROI driver, boosts credit card adoption.

UPI QR → Weak correlation, independent growth path, positioned as future digital driver.

## Return on Investment (ROI) Analysis of Channel Spending Efficiency  
**POS, ATM, and QR Code Channels | 2022 – 2025**

---

### 📊 ROI Summary Table  

| Year | ROI - POS (%) | ROI - ATM (%) | ROI - QR (%) |
|------|---------------|---------------|--------------|
| 2022 | -55.80        | -80.80        | 16.54        |
| 2023 | -53.22        | -78.08        | 5.43         |
| 2024 | -49.56        | -75.02        | 9.11         |
| 2025 | -47.11        | -72.90        | 168.75       |

---

### 🔑 Key Insights  
- **POS channel ROI** → Consistently negative but steadily improving, moving from ‑55.80% in 2022 to ‑47.11% in 2025 (recovery of ~8.7 percentage points).  
- **ATM channel ROI** → Remains the weakest performer, deeply negative throughout (‑80.80% → ‑72.90%), proving it is a cost/loss center despite slight improvement.  
- **QR Code channel ROI** → Only consistently positive performer, with an exceptional surge in 2025 (9.11% → 168.75%, >18x increase).  
- **Strategic Takeaway** → The dramatic 2025 spike in QR ROI signals rapidly growing adoption and cost‑efficiency of QR‑based payments, driven by low infrastructure costs and rising digital/contactless usage.  

---


## 5️⃣ Maintenance & ATM Stress (Onsite vs Offsite Combined)
### 🎯 Goal: Track ATM workload trends and identify which locations (onsite vs offsite) need more frequent maintenance, ensuring cost‑efficient infrastructure management.

## 📈 Visualization
Grouped Barplot

Compare onsite vs offsite ATM counts across years.

Measure stress line (2.4%) to check utilization levels.

Flag maintenance priorities based on workload distribution.

## Visual:
<img width="781" height="489" alt="image" src="https://github.com/user-attachments/assets/2089346e-9808-4bf7-b247-b6965057673e" />

### Chart Interpretation (ATM Stress Analysis)

- **Interpretation →** Grouped barplot shows workload distribution between onsite and offsite ATMs.  
- **Key Insight →** Onsite ATMs carry higher maintenance share, offsite ATMs show very low stress.  
- **Pattern →** Overall stress line at 2.4% → ATMs underutilized, no urgent upgrades required.  
- **Trend →** Onsite ATMs need quarterly checks, offsite ATMs can be maintained half‑yearly.  
- **Observation →** Maintenance strategy should prioritize onsite ATMs while minimizing offsite costs.  

## 📌 Key Business Insights
Onsite ATMs → Higher workload, require quarterly maintenance.

Offsite ATMs → Lower stress, can be maintained half‑yearly.

Overall Stress Line (2.4%) → ATM infra underutilized, no urgent upgrades needed.

## 6️⃣ Bank Market (Debit vs Credit Spend)
### 🎯 Goal: Compare average debit vs credit card spend across bank categories, spot leaders/laggards, and highlight uneven adoption patterns.

## 📈 Visualization
Pivot Table / Comparative Barplot

Compare average debit vs credit spend across Public, Private, Foreign, Small Finance, and Payment banks.

Rank categories by spend levels to identify leaders and weak performers.

## Visual:
<img width="757" height="405" alt="image" src="https://github.com/user-attachments/assets/e78f14e5-c510-4323-93a5-24a7a650341f" />

### Chart Interpretation (Debit vs Credit Spend)

- **Interpretation →** Pivot table shows debit‑driven vs credit‑driven adoption across categories.  
- **Key Insight →** Private banks lead debit spend, foreign banks balance debit + credit, public banks lag in credit adoption.  
- **Pattern →** Payment banks negligible spend, weakest adoption.  
- **Trend →** Debit spend dominates Indian banking, but credit adoption remains uneven.  
- **Observation →** Market leaders = Private banks (loyalty), Foreign banks (premium balance).  

## 📌 Key Business Insights
Private Sector Banks → Debit (12.9), Credit (1.4) → highest debit spends, strong customer loyalty.

Foreign Banks → Debit (7.7), Credit (3.7) → balanced debit + credit, premium customer base.

Public Sector Banks → Debit (6.2), Credit (0.9) → wide reach but weak credit engagement.

Small Finance Banks → Debit (2.6), Credit (0.5) → lowest among mainstream, inclusion‑focused.

Payment Banks → Debit (0.0), Credit (0.1) → negligible spend, weakest adoption.

## 7️⃣ Customer Loyalty Profiling
### 🎯 Goal: Identify which banks keep customers most active and engaged by analyzing debit and credit card usage patterns.

📈 Visualization
Stacked Bar Chart

Group banks by category (Public, Private, Foreign, Small Finance, Payment).

Plot average debit + credit card transactions per category.

Add a red benchmark line to compare loyalty across categories.
<img width="822" height="681" alt="image" src="https://github.com/user-attachments/assets/be8ff8f5-1569-4260-a46a-027052677f85" />

### Chart Interpretation (Customer Loyalty by Bank Category)

- **Interpretation →** Stacked bar chart shows combined debit + credit activity per bank category.  
- **Key Insight →** Private banks consistently above benchmark, proving stronger customer retention.  
- **Pattern →** Foreign banks show very high debit but negligible credit → risk concentrated in one channel.  
- **Trend →** Public banks lag behind, weaker engagement compared to private sector.  
- **Observation →** Benchmark line highlights only private banks consistently stay above market average.  

## 📌 Key Business Insights
Private Sector Banks (HDFC, ICICI, Axis, etc.) → Highest combined activity, strong loyalty, balanced debit + credit usage.

Foreign Banks → Outliers → very high debit, negligible credit, risk concentrated in one channel.

Regional Private Banks → Moderate loyalty, steady debit reliance, slower digital adoption.

Public Sector Banks (SBI, Union, IDBI) → Lower per‑card activity, weaker customer engagement.

Payment Banks → Minimal ATM reliance, overall transaction volume still low.


## 8️⃣ Risk & Safety Management
### 🎯 Goal: Screen for financial risk exposure in banks expanding digital services, ensuring growth is balanced with transaction security and fraud prevention.

## 📈 Visualization
Pair Plot

Compare ATM withdrawal amounts vs transactions per ATM across top banks.

Identify cash‑heavy risk concentration vs digital safety balance.

<img width="954" height="772" alt="image" src="https://github.com/user-attachments/assets/94219770-c7bd-40d6-b7a0-6d1b91e38734" />

### Chart Interpretation (Risk & Digital Safety)

- **Interpretation →** Pair plot shows how reliance on cash vs digital adoption impacts risk.  
- **Key Insight →** More cash = more risk, more digital = more safety.  
- **Pattern →** Airtel Payments Bank safest (low withdrawals, few transactions), American Express highest risk (large withdrawals, few transactions).  
- **Trend →** Balanced banks (Au Small Finance, Axis) show moderate risk, Bandhan Bank inclusion effort but uneven adoption.  
- **Observation →** Digital‑focused banks manage risk better, cash‑heavy banks face concentrated exposure.  

## 📌 Key Business Insights
Airtel Payments Bank → Lowest withdrawals (₹200–₹300), very few transactions (<50) → safest, digital‑focused.

Au Small Finance & Axis Bank → Moderate withdrawals (₹1,000–₹1,500), transactions (100–200) → balanced, safe but moderate risk.

American Express → Very high withdrawals (₹4,000–₹5,000), few transactions (<30) → concentrated high‑value risk.

Bandhan Bank → Low withdrawals (₹500–₹700), moderate transactions (80–120) → inclusion effort but uneven adoption.

-----
## Four-Layer Analytics Framework
The project follows a **four‑layer analytics maturity model** to ensure structured insights:

### 1️⃣ Descriptive Analysis — "What happened?"
- Public + Private banks together account for 85–90% of active cards → dominance of traditional categories.  
- Debit spend drives adoption in Private/Public banks, while Foreign banks lead in credit spends.  
- Digital adoption uneven → Small Finance banks lean heavily digital, Payment banks remain weak.  

---

### 2️⃣ Diagnostic Analysis — "Why did it happen?"
- Public banks benefit from large customer bases but lag in digital modernization.  
- Private banks push urban loyalty programs → higher debit activity.  
- Foreign banks attract premium customers → balanced debit + credit spend.  
- Payment banks face trust + infra gaps → limited adoption.  

---

### 3️⃣ Predictive Analysis — "What will happen?"
- Hybrid models (Private/Public) will dominate → branch trust + digital convenience.  
- POS + QR synergy → near‑term profit growth.  
- UPI QR → independent digital driver, reshaping future adoption.  
- Cash‑heavy banks → risk concentration may increase unless digital channels expand.  

---

### 4️⃣ Prescriptive Analysis — "What should we do?"
- Reward loyalty in Private/Foreign banks to sustain engagement.  
- Modernize Public banks with stronger digital adoption programs.  
- Invest in POS + QR for immediate ROI, prepare UPI QR as long‑term growth engine.  
- Balance infra strategy → onsite ATMs quarterly, offsite half‑yearly, shift focus to digital channels.  

## Key Business Takeaways
Descriptive: Clear dominance of Public + Private banks, debit‑driven adoption.

Diagnostic: Structural reasons → modernization gaps, loyalty programs, premium focus.

Predictive: Hybrid + UPI QR will shape future adoption.

Prescriptive: Actionable roadmap → loyalty rewards, modernization, ROI drivers, infra balance.

----

## Key Findings — Consolidated
This section summarizes the most important insights derived from the analysis of Indian banking infrastructure and digital payment adoption (2022–2025).

### Consolidated Insights

- **ATM Infrastructure**
  - Onsite & Offsite ATMs grow together, but overall stress is low (2.4%).  
  - ATMs are underutilized → no urgent upgrades required.  

- **POS + QR Synergy**
  - Strongest profit driver, pushing credit card adoption.  
  - POS + Bharat QR channels show moderate correlation, delivering immediate ROI.  

- **UPI QR Adoption**
  - Evolves independently, positioned as the **future digital driver**.  
  - Weak correlation with other channels → long‑term growth engine.  

- **Customer Loyalty**
  - Private banks → strongest loyalty (6.2 txns/card).  
  - Foreign banks → balanced debit + credit, premium customer base.  
  - Public/Small Finance banks → moderate loyalty.  
  - Payment banks → weakest adoption, minimal engagement.  

- **Risk Analysis**
  - Cash‑heavy banks face concentrated risk.  
  - Digital‑focused banks (e.g., Airtel Payments Bank) manage risk best.  
  - American Express shows high‑value risk due to large withdrawals with few transactions.  

## Business Takeaways
ATM infra → maintain but avoid overinvestment.

POS + QR → immediate ROI driver, expand merchant acceptance.

UPI QR → prepare as independent digital growth engine.

Customer loyalty → strongest in Private/Foreign banks, modernization needed in Public/Payment banks.

Risk management → cash‑heavy banks must diversify into digital channels.

-----

## Business Recommendations  

Based on the consolidated findings, the following strategic actions are recommended:

1. **ATM Infrastructure Optimization**  
   - Reduce stress by redistributing workload across onsite/offsite ATMs.  
   - Invest in smart ATMs with lower maintenance costs.  

2. **Digital Adoption Acceleration**  
   - Expand UPI/QR penetration in semi‑urban & rural branches.  
   - Incentivize customers with cashback/rewards for digital transactions.  

3. **Customer Loyalty Programs**  
   - Strengthen credit card loyalty with tiered benefits.  
   - Bridge debit card engagement gap with personalized offers.  

4. **Channel Efficiency Enhancement**  
   - Promote online channels for higher ticket size transactions.  
   - Optimize POS infrastructure in retail hubs.  

5. **Risk & Safety Management**  
   - Deploy fraud detection systems for cash‑heavy banks.  
   - Enhance cyber‑security for digital‑first banks.  

## 📌 Key Takeaways
Infra Strategy → Optimize ATM maintenance, avoid over‑spending on low‑stress infra.

ROI Drivers → POS + QR channels deliver immediate profitability.

Future Growth → UPI QR adoption will reshape digital payments.

Customer Engagement → Loyalty programs + modernization critical for retention.

Risk Management → Cash‑heavy banks must diversify into digital channels.

-----

## Limitations of the Study  

While the analysis provides valuable insights, certain limitations exist:

1. **Data Availability**  
   - RBI datasets provide aggregated values; micro‑level customer data is not accessible.  
   - Limited granularity for rural vs urban segmentation.  

2. **Time Coverage**  
   - Focused on 2015–2025; future adoption trends beyond this period not captured.  

3. **Feature Engineering Assumptions**  
   - Derived metrics (e.g., spend per card, ATM stress index) assume uniform distribution.  
   - Actual customer behavior may vary across regions and demographics.  

4. **Predictive Scope**  
   - Forecasts are indicative, not prescriptive.  
   - External shocks (policy changes, fintech disruptions) not modeled.  

5. **Risk Analysis Constraints**  
   - Fraud vulnerability assessed at infrastructure level, not transaction‑level.  
   - Cyber‑security measures vary widely across banks, not fully captured.  

---

## Conclusion

This project demonstrates how **Indian banking infrastructure and digital payment adoption (2022–2025)** can be analyzed using a structured, four‑layer analytics framework.  

- **Data Insights** → Highlighted ATM stress, digital vs physical balance, and loyalty gaps.  
- **Business Value** → Provided actionable recommendations for infrastructure optimization, digital acceleration, and risk management.  
- **Recruiter Relevance** → Showcases end‑to‑end workflow: data preprocessing → feature engineering → visualization → strategic recommendations.  

---

## Project Files & Access  

- Raw Dataset  
- Final Cleaned Dataset  
- Google Colab Notebook  
- Power BI Dashboard  
- Project Report

---

# Power BI Dashboard – Banking Infrastructure & Digital Payment (2022–2025)

## 📌 Project Summary
Interactive **Power BI dashboard** analyzing:
- Debit & Credit card monthly spend
- ATM distribution (Onsite vs Offsite)
- Channel efficiency & ROI ratio
- Bank category & bank‑wise performance

---
# PowerBI-Dashboard
### Data_Modelling
<img width="1099" height="620" alt="image" src="https://github.com/user-attachments/assets/02931b20-d2ff-480f-96bc-19f485b1c9cc" />

## 📊 Dashboard Output 
<img width="1472" height="810" alt="image" src="https://github.com/user-attachments/assets/c4d4e4d0-b096-4afd-92ee-41034a43799c" />

- **KPI Cards** → Total ATMs, Debit Spend, Credit Spend, Efficiency
- **Line Chart** → Year‑wise Debit Transaction Strategy
- **Bar Chart** → Monthly Debit Spend by Bank
- **Pie Chart** → Onsite vs Offsite ATM Ratio
- **Area Chart** → Credit vs Debit Card Analysis
- **Gauge Chart** → ROI Ratio (Efficiency Snapshot)

---

## 🎛️ Filters
- Date range (2022–2025)
- Bank Category (Public, Private, Payment, Small Finance, Foreign)
- Bank Name checklist
- Channel Type (ATM, POS, QR, UPI)

---

## 🚀 Usage
1. Open `.pbix` file in Power BI Desktop.
2. Apply slicers → explore trends.
3. Export dashboard → PDF/PNG for recruiter showcase.


### 🔧How to Access & Run
## How to Access in Google Colab
1. Open Google Colab → https://colab.research.google.com  
2. Upload the notebook file from `/notebooks/` (e.g., 01_preprocessing.ipynb)  
3. Make sure dependencies are installed:  
   ```bash
   pip install -r requirements.txt
   
---
## Contact & Usage

For queries, collaboration, or feedback:  
- **Author:** Yogeswari K  
- **Role:** Aspiring Data Analyst  
- **Location:** Hosur, Tamil Nadu, India  
- **Email:** kadalyoga20@gmail.com  
- **LinkedIn:** [linkedin.com/in/yogeswarik](https://www.linkedin.com/in/yogeswarikadarkarai/) 
- **GitHub:** [github.com/YogeswariK](https://github.com/Yogeswari-sri?tab=repositories)

---

### 🤝 How Recruiters Can Use This Repo
**Project Workflow:** Data cleaning → preprocessing → feature engineering → visualization → insights generation.
**Technical Skills:** Python (Pandas, NumPy, Seaborn, Matplotlib), SQL, Excel (Pivot Tables, Power Query), Power BI (DAX, dashboard design).
**Business Impact:** ROI analysis of ATM, POS, QR channels; customer loyalty metrics; digital adoption recommendations.
**Portfolio Readiness:** End‑to‑end analytics project demonstrating structured methodology, visualization, and decision‑making skills relevant for data analyst roles.  

---



