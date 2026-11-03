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
"This project was completed as part of the Machine Learning CIE 2 activity. Faculty reference and Machine Learning learning resources: https://github.com/Princy2129"
**Thank you for visiting this repository!**


# 🏠 Simple House Price Prediction using Linear Regression

## 📌 Project Overview

This project is developed as part of **Machine Learning – CIE 2, Activity 2 (Unit II: Supervised Learning – Regression)**.

The main objective of this activity is to build a Machine Learning model using **Simple Linear Regression** to predict house prices based on property features.

The project demonstrates the complete regression workflow, including data collection, data preprocessing, visualization, model training, prediction, and performance evaluation.

## 🎯 Objectives

- Understand and explore a house price dataset.
- Identify suitable input features (X) and target variable (y).
- Perform data cleaning and preprocessing.
- Visualize the relationship between property features and prices.
- Split the dataset into training and testing sets.
- Build and train a Linear Regression model.
- Predict house prices using test data.
- Evaluate the model using MAE, MSE, RMSE, and R².
- Predict the price of a new property.

## 📂 Dataset Information

- **Dataset Name:** House Price Prediction Dataset
- **Dataset Source:** [Kaggle – House Prices Dataset](https://www.kaggle.com/datasets)
- **Description:** The dataset contains property-related information that can be used to understand and predict house prices.

### Selected Variables

| Variable | Description |
|---|---|
| Input Feature (X) | Area of the house (square feet) |
| Target Variable (y) | House Price |

*Note: The final feature selection depends on the dataset used in the notebook.*

## 🛠️ Technologies Used

- Python
- Google Colab / Jupyter Notebook
- Pandas – Data manipulation
- NumPy – Numerical calculations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Machine Learning model

## ⚙️ Project Workflow

1. **Dataset Collection:** Select and load a suitable house price dataset.
2. **Data Exploration:** Examine records, columns, data types, and statistical information.
3. **Data Preprocessing:** Handle missing values, invalid values, and duplicate records.
4. **Feature Selection:** Select house area as the input feature and price as the target.
5. **Data Visualization:** Create scatter plots to understand the relationship between area and price.
6. **Train-Test Split:** Divide the dataset into 80% training data and 20% testing data.
7. **Model Training:** Train a Simple Linear Regression model.
8. **Prediction:** Predict house prices using unseen test data.
9. **Model Evaluation:** Calculate MAE, MSE, RMSE, and R².
10. **Visualization:** Compare actual and predicted house prices.
11. **New Prediction:** Estimate the price of a new house using the trained model.

## 📐 Linear Regression Equation

The Simple Linear Regression equation is:

**y = mx + c**

Where:

- **y:** Predicted house price
- **x:** House area (input feature)
- **m:** Regression coefficient (slope)
- **c:** Intercept

The model learns the slope and intercept from the training dataset.

## 📊 Model Evaluation Metrics

The model performance is evaluated using the following metrics:

| Metric | Description |
|---|---|
| MAE | Mean Absolute Error |
| MSE | Mean Squared Error |
| RMSE | Root Mean Squared Error |
| R² Score | Measures how well the model explains the variation in house prices |

The evaluation results are available in the completed Jupyter Notebook.

## 📈 Visualizations

The project includes:

- Scatter plot of house area vs. actual price.
- Actual vs. predicted house price comparison.
- Perfect prediction reference line.
- Graphical representation of the relationship between input features and target values.

## 🔮 New House Price Prediction

The trained Linear Regression model is used to predict the price of a new house based on its area.

The predicted value is generated using the learned regression equation.

## 📝 Conclusion

In this activity, a Simple Linear Regression model was developed to predict house prices using property-related features.

The project helped demonstrate the practical implementation of supervised learning and regression techniques.

The model was evaluated using MAE, MSE, RMSE, and R² score to understand its prediction performance.

**Limitation:** House prices depend on several factors, including location, area, number of rooms, construction quality, and nearby facilities. A simple Linear Regression model using only one feature may not capture all these factors accurately.

## 📁 Repository Structure

```text
Simple-House-Price-Prediction/
│
├── House_Price_Prediction.ipynb
├── README.md
└── dataset.csv
```

## 👨‍🎓 Academic Information

- **Student Name:** Krishna Bhegade
- **Roll Number:** 2119
- **Branch:** Artificial Intelligence and Data Science (AI&DS)
- **Section:** AIDS-A
- **College:** Zeal College
- **Subject:** Machine Learning
- **Activity:** CIE 2 – Activity 2
- **Unit:** Unit II – Supervised Learning: Regression

## 👩‍🏫 Faculty Reference & Acknowledgement

This project was completed as part of the Machine Learning CIE 2 activity.

Faculty reference and Machine Learning learning resources:

[Princy2129 – GitHub Faculty Profile](https://github.com/Princy2129)

## 🚀 How to Run This Project

1. Clone or download this repository.
2. Open Google Colab or Jupyter Notebook.
3. Upload the dataset file.
4. Open `House_Price_Prediction.ipynb`.
5. Execute all cells sequentially.
6. Review the model predictions, evaluation metrics, and visualizations.

---

⭐ **Thank you for visiting my project repository!**

**Machine Learning | Supervised Learning | Linear Regression | Python**
