# Banking Infrastructure & Digital Payment Analysis using Python 2022-2025 ✅

An end-to-end Python data analytics project evaluating transaction benchmarks, physical vs. digital payment infrastructure, and channel interactions across commercial and specialized banking sectors.

---

Stored using: Git LFS (Large File Storage), since GitHub's normal file limit is 100MB)
    Size: ~350 MB
    Stored using: Git LFS (Large File Storage), since GitHub's normal file limit is 100MB


# Banking Infrastructure & Digital Payment Analysis (2022–2025)


## 📌 About This Project
A Python project analyzing Indian banking infrastructure and digital payment adoption from 2022 to 2025.  
Covers **data cleaning, visualization, and trend insights** to understand how ATMs, POS, QR, and card/UPI transactions evolved.

---

## 📊 Dataset
- **File:** Banking-Analysis-2022-2025.csv  
- **Size:** ~350 MB (replace with actual size)  
- **Stored using:** Git LFS (Large File Storage), since GitHub’s normal file limit is 100MB  

### Dataset Column Details

| Column | Description |
|--------|-------------|
| id | Unique identifier for each record |
| date | Month/Year of transaction |
| bank_category | Public / Private / Foreign |
| bank_name | Name of the bank |
| atms_crms_onsite | Onsite ATM/CRM count |
| atms_crms_offsite | Offsite ATM/CRM count |
| pos | POS terminals deployed |
| micro_atms | Micro ATM count |
| bharat_qr | Bharat QR adoption |
| upi_qr | UPI QR adoption |
| credit_cards | Credit cards issued |
| debit_cards | Debit cards issued |
| cc_pay_trns_at_pos_vol | Credit card POS transaction volume |
| dc_pay_trns_online_val | Debit card online transaction value |
| … | Other transaction metrics |

---

## ⚙️ How the Dataset Was Uploaded (Git Bash Workflow)

```bash
# 1. Configure Git identity
git config --global user.name "Yogeswari-sri"
git config --global user.email "kadalyoga20@gmail.com"

# 2. Clone repo
git clone https://github.com/<Yogeswari-sri>/Banking-Analysis-2022-2025.git
cd Banking-Analysis-2022-2025

# 3. Install Git LFS
git lfs install

# 4. Track large files
git lfs track "*.csv"
git add .gitattributes
git commit -m "Configure Git LFS tracking"

# 5. Add dataset
git add Banking-Analysis-2022-2025.csv
git commit -m "Add banking dataset via Git LFS"

# 6. Push to GitHub
git push

---

## 🔑 Analytical Objectives
### Objective 1 — Fair Comparison Using Active Cards
**Goal:** Compare banks fairly by focusing on **active debit/credit cards** rather than issued cards.  
**Key Insights:**  
- Public banks lead adoption with highest active card counts.  
- Payment banks show weakest retention.  
- Benchmarking by active cards ensures realistic engagement view.

---

### Objective 2 — Bank Category Growth Trends
**Goal:** Track year‑wise changes in active cards across categories.  
**Key Insights:**  
- **SBI consistently leads** from 2022–2025, peaking in 2023.  
- Sharp decline post‑2023 highlights retention challenges.  
- Digital adoption strategies needed to sustain growth.

---

### Objective 3 — Real vs Digital Balance
**Goal:** Evaluate digital vs branch balance across bank categories.  
**Key Insights:**  
- Small Finance Banks → extremely digital, minimal branch presence.  
- Private Banks → healthy hybrid mix.  
- Public Banks → branch‑oriented, slower digital shift.  
- Payment & Foreign Banks → weak digital adoption.

---

### Objective 4 — Channel Smart Spending Efficiency
**Goal:** Assess ROI efficiency across ATM, POS, Bharat QR, and UPI QR.  
**Key Insights:**  
- **POS + Bharat QR synergy** drives profitability.  
- **UPI QR evolves independently** as future growth engine.  
- ATM expansion supports debit base but limited ROI.

---

### Objective 5 — ATM Stress & Maintenance
**Goal:** Track ATM workload trends for maintenance planning.  
**Key Insights:**  
- Onsite ATMs → higher stress, need quarterly checks.  
- Offsite ATMs → low stress, half‑yearly maintenance sufficient.  
- Overall ATM utilization remains under 2.4%.

---

### Objective 6 — Bank Market Benchmarking
**Goal:** Compare debit vs credit spend across categories.  
**Key Insights:**  
- Private Banks → highest debit spend, strong loyalty.  
- Foreign Banks → balanced debit + credit, premium base.  
- Public Banks → wide reach but weak credit adoption.  
- Payment Banks → negligible spend.

---

### Objective 7 — Customer Loyalty Profiling
**Goal:** Identify banks with most active and engaged customers.  
**Key Insights:**  
- Private Banks lead in loyalty.  
- Foreign Banks show premium but volatile loyalty.  
- Public Banks lag in consistent engagement.

---

### Objective 8 — Risk & Safety Management
**Goal:** Screen for risk exposure in digital expansion.  
**Key Insights:**  
- High reliance on digital channels increases fraud risk.  
- Balanced adoption (hybrid model) ensures safer growth.  

---

## 📈 Business Recommendations
- **Promote POS penetration** in public banks.  
- **Invest in UPI QR** as long‑term growth driver.  
- **Hybrid adoption model** (digital + branch) ensures balanced ROI.  
- **Customer retention programs** to sustain loyalty.  
- **AI‑based monitoring** for fraud detection and anomaly alerts.

---

## 🚀 Project Status
✅ Completed — Data cleaning, feature engineering, statistical modeling, visualization, and business recommendations.

---

#DataAnalytics #Banking #DigitalPayments #PythonEDA #PowerBI #SQL #Visualization #PortfolioProject
