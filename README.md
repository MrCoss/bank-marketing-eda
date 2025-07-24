## Bank Marketing EDA – Skillfied Mentor Internship

This project presents an in-depth Exploratory Data Analysis (EDA) of the Bank Marketing dataset using Python. The analysis includes data cleaning, visualization, feature engineering, and preparation for modeling. The insights help understand customer behavior toward term deposit subscriptions.

## Project Structure

- `datasets/` – Raw and cleaned data
- `plots/` – Visualizations
- `data/` – Reports and intermediate files
- `Bank_Marketing_Inspection_Final.ipynb` – Main EDA Notebook
- `Bank_Marketing_EDA_Report.pdf` – Final Report
- `requirements.txt` – Required Python packages

## Key Visualizations

### 1. Target Variable Distribution
![Target Distribution](plots/target_distribution.png)

### 2. Correlation Heatmap
![Correlation Heatmap](plots/correlation_heatmap.png)

### 3. Feature Importance (Random Forest)
![Feature Importance](plots/feature_importance_rf.png)

### 4. Class Distribution – Before and After SMOTE
![Before SMOTE](plots/class_distribution_before_smote.png)
![After SMOTE](plots/class_distribution_after_smote.png)

### 5. Categorical Features vs Target
![Job vs Target](plots/barplot_job_y.png)
![Education vs Target](plots/barplot_education_y.png)
![Marital vs Target](plots/barplot_marital_y.png)

### 6. Log Transformation Example
![Log Transform – Campaign](plots/log_transform_campaign.png)

## Summary

- Missing values handled and imputed
- Class imbalance addressed with SMOTE
- Label encoding and scaling applied
- Top features identified via correlation and feature importance
- Skewness treated and VIF calculated
- Cleaned dataset and reports saved for modeling

## Setup & Usage
git clone https://github.com/MrCoss/bank-marketing-eda
cd bank-marketing-eda
pip install -r requirements.txt

Open the notebook to explore the full analysis:

jupyter notebook Bank_Marketing_Inspection_Final.ipynb

Author

Costas Antony Pinto
MCA AI & ML |
Manipal University Jaipur  
Skillfied Mentor Internship

---
