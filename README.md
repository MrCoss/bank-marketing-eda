📊 BANK MARKETING DATASET – EXPLORATORY DATA ANALYSIS (EDA)

------------------------------------------------------------
Project Title  : Bank Marketing Campaign – EDA & Insights
Internship     : Skillfied Mentor Internship
Submitted By   : Costas Antony Pinto
Course         : MCA AI/ML – Manipal University Jaipur
GitHub Repo    : https://github.com/MrCoss/bank-marketing-eda
------------------------------------------------------------

🧾 OBJECTIVE:
------------
The objective of this project is to perform an in-depth exploratory data analysis on the Bank Marketing dataset to uncover meaningful insights, identify patterns, and prepare the dataset for machine learning tasks such as classification.

📁 DIRECTORY STRUCTURE:
-----------------------
Banking Data Analysis/
│
├── data/
│   ├── feature_importance.csv
│   ├── skewness_report.csv
│   ├── top_corr_features.csv
│   ├── vif_report.csv
│   ├── eda_summary.txt
│   └── Bank_Marketing_EDA_Report.pdf
│
├── datasets/
│   ├── bankmarketingdata.csv
│   └── bankmarketing_cleaned.csv
│
├── plots/
│   └── [all generated visualizations in PNG]
│
├── Bank_Marketing_Inspection_Final.ipynb
├── requirements.txt
└── README.txt

🧪 KEY STEPS PERFORMED:
-----------------------
1. Setup Environment and Folder Structure
2. Load Dataset with Safe Fallback Delimiter Check
3. Initial Inspection: Shape, Info, Description, Uniques
4. Handle Missing Values (including "unknown")
5. Impute Missing Values (Categorical → Mode, Numeric → Median)
6. Drop Duplicate Records
7. Visualize Target Variable Distribution
8. Explore Categorical Features vs Target (Barplots)
9. Encode Categorical Variables using LabelEncoder
10. Analyze Class Imbalance and Apply SMOTE
11. Feature Scaling with StandardScaler
12. Correlation Matrix and Top Correlated Features
13. Feature Importance using Random Forest
14. Boxplots & Histograms for Numeric Analysis
15. Feature Engineering (age_group, contacted_before, effective_contact)
16. Handle Skewed Features via log1p
17. Multicollinearity Check using VIF
18. Save Final Cleaned Dataset
19. Generate Text-based EDA Summary Report
20. Create Final EDA PDF Report using ReportLab

📄 FINAL OUTPUTS:
-----------------
- 📁 Cleaned CSV: `datasets/bankmarketing_cleaned.csv`
- 📊 EDA Summary: `data/eda_summary.txt`
- 📊 EDA PDF Report: `data/Bank_Marketing_EDA_Report.pdf`
- 📈 Visualizations: `plots/` (Barplots, Heatmaps, Histograms)

📦 ENVIRONMENT:
---------------
- Python 3.10+
- Key Libraries:
  - pandas, numpy, seaborn, matplotlib
  - scikit-learn, imbalanced-learn
  - reportlab, missingno, statsmodels

📌 TO SETUP LOCALLY:
--------------------
1. Clone the repository:
   git clone https://github.com/MrCoss/bank-marketing-eda

2. Create a virtual environment:
   python -m venv venv
   venv\Scripts\activate

3. Install dependencies:
   pip install -r requirements.txt

4. Open Jupyter Notebook:
   jupyter notebook Bank_Marketing_Inspection_Final.ipynb

✔️ STATUS:
---------
✅ Completed – All steps executed successfully
✅ Reports saved in both TXT and PDF formats
✅ Git repository updated and maintained

📧 CONTACT:
----------
Costas Antony Pinto  
Email: costaspinto312@gmail.com  
GitHub: https://github.com/MrCoss  

------------------------------------------------------------
This project was completed under the Skillfied Mentor Internship.
All work is original and reproducible.
------------------------------------------------------------
