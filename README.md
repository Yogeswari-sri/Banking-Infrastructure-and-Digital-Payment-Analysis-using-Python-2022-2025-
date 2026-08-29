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

## 🛠 Tools & Technologies
Python (Pandas, NumPy, Seaborn, Matplotlib)  
Jupyter Notebook

## 🔍 Analysis
- Data cleaning & feature engineering (digital ratio)  
- Bankwise comparison, monthly trends, ratio analysis  
- Visual insights (bar plots, line charts, pair plots) 

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
  

## 📈 Methodology
Business → Data → Modelling → Evaluation → Deployment
 

## 📑 Key Findings
- ATM vs POS adoption patterns  
- Digital ratio differences across banks  

## 💡 Recommendations
- Improve POS penetration strategies  
- Policy suggestions for digital adoption  

## ⚠️ Limitations
Dataset scope (2022–2025), missing regional/demographic variables  


## 🚀 Project Status
✅ Completed — Data cleaning, feature engineering, statistical modeling, visualization, and business recommendations.


## ✅ Final Conclusion
- Digital adoption accelerated between 2022–2025.  
- Public banks lead infra deployment, but Private banks show faster UPI adoption.  
- Debit card usage dominates, credit penetration remains weak.  
- Hybrid models (branch + digital) deliver balanced growth.  

-----

**Banking Infrastructure & Digital Payments Analysis (2022–2025)**
Project Workflow
Step 1: Data Cleaning – removed duplicates, handled missing values, standardized column names.
Step 2: Exploratory Data Analysis – studied bank category and bank name distribution, tracked time series trends for POS and UPI QR growth.
Step 3: Feature Engineering – created digital ratio feature, derived comparative metrics for ATM vs POS and Debit vs Credit.
Step 4: Statistical Analysis – performed correlation checks and built trend forecasting models.
Step 5: Insights Generation – summarized adoption patterns and highlighted ROI drivers and risk factors.

Tools Used
Python (pandas, numpy, seaborn, matplotlib) for data loading, cleaning, and analysis.
Google Colab as the cloud-based Python environment.
Git and Git LFS for version control and large file storage.
GitHub for hosting project code and dataset.

Data Preprocessing and Feature Engineering
Zero-imputation strategy: missing values in infra/transaction columns filled with 0 to preserve aggregate calculations.
Infinity and NaN neutralization: divide-by-zero artefacts converted to NaN and filled with 0 to avoid skew.
Date parsing: raw string dates converted into structured pandas datetime objects for time-series analysis.
Duplicate removal: ensured unique records for bank-wise infra and transactions.
Feature engineering included digital ratio (POS+UPI ÷ ATM), active card ratio, and categorical infra tiers using quantile segmentation.

Statistical Analysis
Mean values show baseline infra deployment across banks.
Median values lower than mean confirm right-skewed distribution.
Mode values highlight inactive banks baseline.
High standard deviation indicates large variance in infra and transaction scale.
Positive skewness shows few banks dominate infra, majority small scale.
High kurtosis confirms fat-tailed distribution and extreme outliers.

Key Takeaways
Dataset shows heavy skewness – few banks dominate infra, majority small scale.
Digital ratio feature highlights faster adoption in Private banks compared to branch-heavy Public banks.
High kurtosis confirms outlier risks such as mega-deployments and sudden spikes.

Visualization and Business Key Insights
