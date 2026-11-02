# Machine Learning CIE 2 – Activity 1
## Dataset Preparation and Exploratory Data Analysis (EDA)

### 📌 Project Overview
This project is part of the **Machine Learning CIE 2 Activity – Unit I: Foundations & Data Preparation**.

The objective of this activity is to inspect a real-world dataset, identify data-quality issues, handle missing values, perform Exploratory Data Analysis (EDA), encode categorical features, scale numerical features, and prepare a cleaned dataset for future Machine Learning workflows.

No prediction model is developed in this activity.

### 🎯 Objectives
- Select and understand a real-world dataset.
- Load and inspect the dataset using Python.
- Identify missing values and data-quality issues.
- Perform basic statistical analysis.
- Handle missing values appropriately.
- Detect duplicate records and outliers.
- Create meaningful data visualizations.
- Apply One-Hot Encoding to categorical features.
- Apply StandardScaler to numerical features.
- Save the prepared dataset in CSV format.

### 📊 Dataset Information

**Dataset Name:** Dirty Cafe Sales Dataset

**Domain:** Business / Retail / Sales Analytics

**Dataset Source:** Kaggle

**Source Link:** https://www.kaggle.com/datasets/ahmedmohamed2003/cafe-sales-dirty-data-for-cleaning-training

**Original File:** `dirty_cafe_sales.csv`

**Original Dataset Shape:**
- Rows: 10,000
- Columns: 8
- File Format: CSV

### 📋 Dataset Columns

| Column | Description |
|---|---|
| Transaction ID | Unique transaction identifier |
| Item | Cafe product name |
| Quantity | Number of items purchased |
| Price Per Unit | Price of one item |
| Total Spent | Total transaction amount |
| Payment Method | Method of payment |
| Location | In-store or takeaway |
| Transaction Date | Date of transaction |

### 🛠️ Technologies and Libraries Used

- Python
- Google Colab / Jupyter Notebook
- Pandas – Data manipulation
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Feature scaling
- KaggleHub – Dataset downloading

### 🔍 Activities Performed

**1. Dataset Loading and Inspection**
- Loaded the Cafe Sales dataset.
- Examined the first and last records.
- Checked dataset shape, column names and data types.
- Generated basic descriptive statistics.

**2. Missing Value Analysis and Handling**
- Identified missing values in all relevant columns.
- Calculated missing-value percentages.
- Converted numerical columns into appropriate numeric formats.
- Used median imputation for numerical columns.
- Used mode imputation for categorical columns.

**3. Data Cleaning**
- Checked data consistency.
- Identified duplicate records.
- Examined numerical outliers using box plots.
- Applied the IQR method to filter outliers in Total Spent.

**4. Exploratory Data Analysis (EDA)**
Performed statistical analysis and created visualizations, including:
- Box Plot
- Correlation Heatmap
- Bar Chart for Total Spent by Cafe Item

**5. Categorical Encoding**
Applied One-Hot Encoding to:
- Item
- Payment Method
- Location

This converts categorical values into numerical binary columns.

**6. Feature Engineering**
Converted Transaction Date into:
- Day
- Month
- Year
- Quarter
- Day of Week

**7. Feature Scaling**
Applied StandardScaler to numerical features:
- Quantity
- Price Per Unit
- Total Spent

The Transaction ID column was removed because it is an identifier rather than a useful numerical feature.

### 📈 Key Results

| Parameter | Result |
|---|---:|
| Original Rows | 10,000 |
| Original Columns | 8 |
| Original Missing Values in Location | 3,265 |
| Original Missing Values in Payment Method | 2,579 |
| Final Rows | 10,000 |
| Final Columns | 27 |
| Final Missing Values | 0 |

The final dataset contains 27 columns after categorical encoding, date feature extraction and removal of the transaction identifier.

### 📁 Project Structure

```text
ML-CIE2-Activity1-2119/
│
├── ML_CIE_ACT_UT1.ipynb
├── dirty_cafe_sales.csv
├── README.md
│
└── dataset/
    └── Original dataset source link
```

### 💡 Conclusion

In this activity, the Dirty Cafe Sales dataset was successfully inspected and prepared for future Machine Learning applications.

Missing values were handled using median and mode imputation. Outliers were examined, categorical features were encoded using One-Hot Encoding, and numerical features were standardized using StandardScaler.

Date information was also extracted into separate features to make the dataset more useful for analysis.

The activity helped develop practical knowledge of data preprocessing, data cleaning, exploratory data analysis and feature engineering.

### 👨‍🎓 Student Information

- **Name:** Krishna Bhegade
- **Branch:** Artificial Intelligence and Data Science (AI&DS)
- **College:** Zeal College
- **Section:** AIDS-A
- **Roll Number:** 3119

### 🙏 Faculty Acknowledgement

This project was completed as part of the Machine Learning CIE 2 activity.

Faculty reference and Machine Learning learning resources:

**[Princy2129 – GitHub Faculty Profile](https://github.com/Princy2129)**

### ⭐ Acknowledgement

"This project was completed as part of the Machine Learning CIE 2 activity. Faculty reference and Machine Learning learning resources: https://github.com/Princy2129"

---

**Thank you for visiting this repository!**
