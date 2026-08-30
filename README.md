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

<div align="center">

## 🛠 Tools & Technologies

**Python** (Pandas, NumPy, Matplotlib, Seaborn)  
**Power BI** (Interactive dashboards)  
**Google Colab** (Analysis environment)  
**GitHub + Git LFS** (Version control & dataset hosting)

</div>

---

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

