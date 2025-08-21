# Bank Marketing EDA & Preprocessing
An in-depth **Exploratory Data Analysis (EDA)** of the Bank Marketing dataset. This project, completed as part of the **Skillfied Mentor Internship**, demonstrates a full data science workflow including data cleaning, visualization, feature engineering, and advanced preprocessing to prepare the dataset for predictive modeling.

-----

## Table of Contents

  - [1. Project Context & Business Problem](https://www.google.com/search?q=%231-project-context--business-problem)
  - [2. Analytical Methodology & Key Findings](https://www.google.com/search?q=%232-analytical-methodology--key-findings)
  - [3. Project Structure Explained](https://www.google.com/search?q=%233-project-structure-explained)
  - [4. Technical Stack](https://www.google.com/search?q=%234-technical-stack)
  - [5. Local Setup & Replication Guide](https://www.google.com/search?q=%235-local-setup--replication-guide)
  - [6. Author & Acknowledgements](https://www.google.com/search?q=%236-author--acknowledgements)

-----

## 1\. Project Context & Business Problem

Direct marketing campaigns are a key strategy for financial institutions, but they can be costly and inefficient if not properly targeted. The business problem is to **increase the effectiveness of a bank's term deposit marketing campaign** by identifying the customer attributes most strongly associated with a subscription.

The objective of this EDA is to explore the provided dataset to understand customer behavior, identify key predictive features, and perform all necessary preprocessing steps to create a clean, balanced, and model-ready dataset. The insights from this analysis form the foundation for building a robust classification model to predict which customers are likely to subscribe.

-----

## 2\. Analytical Methodology & Key Findings

The project followed a structured analytical workflow, from initial data inspection to final preprocessing.

### Step 1: Data Cleaning & Initial Inspection

  - The dataset was loaded and inspected for initial quality issues, including missing values and incorrect data types.
  - Missing values were handled using appropriate imputation strategies to preserve the dataset's integrity.

### Step 2: Exploratory Data Analysis (EDA)

  - **Target Variable Analysis:** The analysis began by examining the target variable (`y`), revealing a **severe class imbalance**. A vast majority of customers did not subscribe to the term deposit, a critical finding that must be addressed before modeling.
      - 
  - **Bivariate Analysis:** The relationship between various features and the target variable was explored.
      - **Categorical Features:** Bar plots were used to visualize how factors like `job`, `education`, and `marital` status correlate with term deposit subscriptions.
          - 
      - **Numerical Features:** A **correlation heatmap** was generated to identify linear relationships between numerical features and to check for multicollinearity.
          - 

### Step 3: Feature Engineering & Selection

  - **Feature Importance:** A preliminary **Random Forest** model was trained to calculate feature importances, providing a data-driven view of the most influential predictors. Features like `duration`, `euribor3m`, and `age` were identified as highly significant.
      - 
  - **Log Transformation:** To handle right-skewed numerical distributions, a **log transformation** was applied to features like `campaign`, normalizing their distribution and making them more suitable for certain modeling algorithms.
      - 

### Step 4: Data Preprocessing for Modeling

  - **Categorical Encoding:** All categorical features were converted into a numerical format using **Label Encoding**.
  - **Handling Class Imbalance (SMOTE):** To address the class imbalance identified in the EDA, the **Synthetic Minority Over-sampling Technique (SMOTE)** was applied to the training data. This technique generates synthetic samples for the minority class (subscribers), creating a balanced dataset for model training.
      - 
      - 
  - **Multicollinearity Check:** The Variance Inflation Factor (VIF) was calculated for all features to ensure there was no significant multicollinearity that could negatively impact model performance.

-----

## 3\. Project Structure Explained

```
.
├── datasets/                     # Contains the raw and cleaned .csv files.
├── plots/                        # Stores all generated visualizations as image files.
├── data/                         # Holds intermediate files and final reports.
├── Bank_Marketing_Inspection_Final.ipynb # The main Jupyter Notebook with all code and analysis.
├── Bank_Marketing_EDA_Report.pdf # A PDF summary report of the findings.
├── requirements.txt              # A list of all Python dependencies.
└── README.md                     # This detailed project documentation.
```

-----

## 4\. Technical Stack

  - **Core Language:** Python
  - **Data Analysis & Manipulation:** Pandas, NumPy
  - **Data Visualization:** Matplotlib, Seaborn
  - **Machine Learning & Preprocessing:** Scikit-learn
  - **Imbalanced Data Handling:** imblearn (for SMOTE)
  - **Development Environment:** Jupyter Notebook

-----

## 5\. Local Setup & Replication Guide

To replicate this analysis on your local machine, please follow these steps.

### Step 1: Clone the Repository

```bash
git clone https://github.com/MrCoss/bank-marketing-eda.git
cd bank-marketing-eda
```

### Step 2: Create and Activate a Virtual Environment (Recommended)

```bash
# Create the environment
python -m venv venv

# Activate on Windows
.\venv\Scripts\activate

# Activate on macOS/Linux
source venv/bin/activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

This will open a new tab in your web browser. Navigate to and open the `Bank_Marketing_Inspection_Final.ipynb` file to view and run the full analysis.

-----

## 6\. Author & Acknowledgements

  - **Author:** Costas Antony Pinto
  - **Internship:** This project was completed as part of the **Skillfied Mentor Internship** program.
