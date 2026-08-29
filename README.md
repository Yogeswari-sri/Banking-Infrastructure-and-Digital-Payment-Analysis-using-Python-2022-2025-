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
| dc_pay_trns_others_val | Other transaction metrics |

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

## 🐍 How the Dataset is Read in Python (Google Colab Workspace)

This section explains how the banking dataset is loaded into a Google Colab notebook directly from this GitHub repository, using Git LFS since the file exceeds GitHub's normal 100MB size limit.

# ============================================
# STEP 1: Install Git LFS (Large File Storage)
# Needed because our dataset files are too big for normal GitHub storage
# ============================================
!apt-get install git-lfs -y
!git lfs install

# ============================================
# STEP 2: Clone the GitHub repository into Colab
# This downloads all project files (code + datasets) from GitHub
# ============================================
!git clone https://github.com/<your-username>/Banking-Analysis-2022-2025.git

# ============================================
# STEP 3: Check what files actually got downloaded
# Useful to confirm the dataset file is present and full-sized (not a tiny LFS pointer file)
# ============================================
!ls -la "/content/Banking-Analysis-2022-2025/"

# ============================================
# STEP 4: Import pandas
# pandas is the main library used to read, clean, and analyze tabular data (like Excel/CSV)
# ============================================
import pandas as pd

# ============================================
# STEP 5: Load the banking dataset into a DataFrame
# A DataFrame is like a table/spreadsheet that Python can work with
# ============================================
df = pd.read_csv("/content/Banking-Analysis-2022-2025/Banking-Analysis-2022-2025.csv")

# ============================================
# STEP 6: Preview the first 5 rows
# Helps confirm the data loaded correctly and shows the column names/structure
# ============================================
df.head()

# ============================================
# STEP 7: Basic info about the dataset
# Shows column names, data types, and missing values — useful first check before analysis
# ============================================
df.info ()

# ============================================
# STEP 8: Summary statistics
# Gives count, mean, min, max, etc. for numeric columns — quick overview of the data
# ============================================
df.describe()

-----

## 📌 Project Overview
Analyze RBI dataset (2022–2025) on ATM deployment, POS expansion, and card issuance to understand digital payment adoption trends.

## 🎯 Problem Statement
Need to compare cash vs digital transaction patterns and forecast adoption.

## 🔑 Objectives
- **Fair Comparison Using Active Cards** → Compare banks using active debit/credit cards.  
- **Bank Category Growth Trends** → Track year‑wise changes in active cards.  
- **Real vs Digital Balance** → Evaluate digital vs branch presence.  
- **Channel Efficiency** → Assess ROI across ATM, POS, QR, UPI.  
- **ATM Stress & Maintenance** → Monitor workload for planning.  
- **Market Benchmarking** → Compare debit vs credit spend.  
- **Customer Loyalty Profiling** → Identify most engaged banks.  
- **Risk & Safety Management** → Screen for fraud exposure in digital expansion.  

## 📊 Dataset
Source: RBI Bankwise ATM & POS Transactions  
Variables: Bank, Date, ATM Transactions, POS Transactions  

## 🛠 Tools & Technologies
Python (Pandas, NumPy, Seaborn, Matplotlib)  
Jupyter Notebook  

## 📈 Methodology
Business → Data → Modelling → Evaluation → Deployment  

## 🔍 Analysis
- Data cleaning & feature engineering (digital ratio)  
- Bankwise comparison, monthly trends, ratio analysis  
- Visual insights (bar plots, line charts, pair plots)  

## 📑 Key Findings
- ATM vs POS adoption patterns  
- Digital ratio differences across banks  

## 💡 Recommendations
- Improve POS penetration strategies  
- Policy suggestions for digital adoption  

## ⚠️ Limitations
Dataset scope (2022–2025), missing regional/demographic variables  


------

## 📌 Project Workflow

1. **Data Cleaning**  
   - Remove duplicates, handle missing values  
   - Standardize column names  

2. **Exploratory Data Analysis (EDA)**  
   - Bank category and bank name distribution  
   - Time series trends (POS, UPI QR growth)  

3. **Feature Engineering**  
   - Create digital ratio feature  
   - Derive comparative metrics (ATM vs POS, Debit vs Credit)  

4. **Statistical Analysis**  
   - Correlation checks  
   - Trend forecasting models  

5. **Insights Generation**  
   - Summarize adoption patterns  
   - Highlight ROI drivers and risk factors

-----

---

## 🔧 Data Preprocessing & Feature Engineering

### **Data Cleaning Steps**

- **Zero-Imputation Strategy: ** Missing values in infra/transaction columns filled with `0` to preserve aggregate calculations.  
- **Infinity & NaN Neutralization: ** Divide-by-zero artefacts (`np.inf`) converted to `NaN` and filled with `0` to avoid skew.  
- **Date Parsing: ** Raw string dates converted into structured `pandas datetime` objects (`year_month`) for time-series analysis.  
- **Duplicate Removal :** Ensured unique records for bank‑wise infra and transactions.  

### **Feature Engineering**

- **Digital Ratio (POS+UPI ÷ ATM): ** Derived feature to measure digital adoption intensity.  
- **Active Card Ratio: ** Debit vs credit active usage ratio for fair comparison.  
- **Categorical Infra Tiers: ** Stratified banks into quadrants (High‑Infra‑Low‑Digital vs Low‑Infra‑High‑Digital) using `pd.qcut()`.  

---

## 📊 Statistical Analysis

### **Statistical Summary Matrix**

## 📊 Statistical Summary Matrix

## 📊 Statistical Summary Matrix

| Metric            | ATM Transactions | POS Transactions | Digital Ratio | Interpretation                                
|-------------------|-----------------|-----------------|---------------|-------------------------------------------------|
| **Mean**          | 12,450          | 18,320          | 1.47          | Baseline average infra deployment               |
| **Median (50%)**  | 2,100           | 3,250           | 0.92          | Lower than mean → right‑skewed                  |
| **Mode**          | 0               | 0               | 0             | Baseline for inactive banks                     |
| **Std Deviation** | 45,200          | 62,800          | 2.15          | High variance across banks                      |
| **Skewness**      | +4.12           | +5.34           | +3.87         | Heavy positive skew (few mega‑deployments)      |
| **Kurtosis**      | +28.05          | +35.12          | +22.40        | Fat‑tailed distribution, extreme outliers       |



---

## ✅ Key Takeaway
- Dataset shows **heavy skewness** → few banks dominate infra, majority small scale.  
- **Digital ratio feature** highlights faster adoption in Private banks vs branch‑heavy Public banks.  
- High kurtosis confirms **outlier risks** (mega‑deployments, sudden spikes).

-----


## 📊 Visualization & Business Key Insights

### **Fair Comparison Using Active Cards**
Bar chart shows public banks lead in active card usage; Payment banks weakest retention.  
**Business Insight: ** Benchmarking by active cards ensures realistic engagement view.

---

### **Bank Category Growth Trends**
Line chart tracks year‑wise active card changes; SBI peaks in 2023, decline after.  
**Business Insight: ** Sustained digital adoption strategies needed to retain growth.

---

### **Real vs Digital Balance**
Stacked chart compares branch vs digital infra; Small Finance highly digital, Public branch‑heavy.  
**Business Insight: ** Hybrid mix (Private banks) offers balanced growth.

---

### **Channel Efficiency**
Comparative plots of ATM, POS, Bharat QR, UPI QR.  
**Business Insight: ** POS + Bharat QR synergy drives ROI; UPI QR future growth engine.

---

### **ATM Stress & Maintenance**
Bar chart of onsite vs offsite ATM workload.  
**Business Insight: ** Onsite ATMs need quarterly checks; offsite half‑yearly sufficient.

---

### **Market Benchmarking**
Debit vs credit spend comparison across categories.  
**Business Insight: ** Private banks strong debit loyalty; Public banks weak credit adoption.

---

### **Customer Loyalty Profiling**
Charts highlight active customer ratios.  
**Business Insight: ** Private banks lead loyalty; Foreign banks premium but volatile.

---

### **Risk & Safety Management**
Trend chart of digital vs fraud exposure. 
**Business Insight: ** High digital reliance increases risk; hybrid adoption safer.

----

## 🛠 Tools Used
- **Python (pandas, numpy, seaborn, matplotlib)** — data loading, cleaning, and analysis  
- **Google Colab** — cloud-based Python environment  
- **Git & Git LFS** — version control and large file storage  
- **GitHub** — hosting project code and dataset  


-----

## 🚀 Project Status
✅ Completed — Data cleaning, feature engineering, statistical modeling, visualization, and business recommendations.


---

## ✅ Final Conclusion
- Digital adoption accelerated between 2022–2025.  
- Public banks lead infra deployment, but Private banks show faster UPI adoption.  
- Debit card usage dominates, credit penetration remains weak.  
- Hybrid models (branch + digital) deliver balanced growth.  

-----


