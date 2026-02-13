# 📊 Lab 4 -- Data Tidying, Cleaning, Imputation & Outlier Detection

## 📌 Project Overview

This notebook demonstrates essential data preprocessing techniques used
in data engineering and data science workflows. The goal of this lab is
to prepare raw data for analysis by applying structured cleaning,
transformation, and validation steps.

The notebook follows best practices for:

-   Data tidying
-   Handling missing values
-   Outlier detection and treatment
-   Data consistency improvements
-   Code documentation and reproducibility

------------------------------------------------------------------------

## 🎯 Objectives

By completing this lab, the following objectives are achieved:

1.  Improve raw dataset quality and structure.
2.  Handle missing values using appropriate imputation strategies.
3.  Detect and manage outliers using statistical and visualization
    techniques.
4.  Apply data transformation methods such as binning and smoothing.
5.  Maintain clean, well-documented, and reproducible code.

------------------------------------------------------------------------

## 🗂 Notebook Structure

### 1️⃣ Data Loading

-   Import required libraries (Pandas, NumPy, Matplotlib, etc.)
-   Load dataset from CSV file
-   Preview data using:
    -   `head()`
    -   `tail()`
    -   `info()`
    -   `describe()`

------------------------------------------------------------------------

### 2️⃣ Data Tidying

-   Rename columns (if needed)
-   Standardize formatting
-   Ensure consistent data types
-   Remove duplicate records
-   Reorganize dataset structure

------------------------------------------------------------------------

### 3️⃣ Data Cleaning

-   Identify missing values using:
    -   `isnull()`
    -   `sum()`
-   Handle inconsistent entries
-   Remove or correct invalid records

------------------------------------------------------------------------

### 4️⃣ Missing Value Imputation

Different strategies applied based on data type:

**Numeric columns** - Mean imputation - Median imputation

**Categorical columns** - Mode imputation - Most frequent value
replacement

Imputation ensures: - No null values remain - Dataset is ready for
modeling

------------------------------------------------------------------------

### 5️⃣ Outlier Detection

Outliers are identified using:

-   Boxplots
-   Statistical methods (IQR or Z-score)

#### IQR Method:

-   Calculate Q1 and Q3
-   Compute IQR = Q3 − Q1
-   Define bounds:
    -   Lower Bound = Q1 − 1.5 × IQR
    -   Upper Bound = Q3 + 1.5 × IQR

Outliers are either: - Removed - Capped - Or analyzed further

------------------------------------------------------------------------

### 6️⃣ Data Transformation

Techniques applied:

-   Binning (discretization)
-   Smoothing (if applicable)
-   Feature adjustments for better interpretability

------------------------------------------------------------------------

## 🛠 Technologies Used

-   Python 3
-   Pandas
-   NumPy
-   Matplotlib
-   Scikit-learn
-   Jupyter Notebook

------------------------------------------------------------------------

## 🔁 Reproducibility Instructions

1.  Install required libraries:

    pip install pandas numpy matplotlib scikit-learn

2.  Place the dataset file in the correct directory.

3.  Open `week5Lab.ipynb` in Jupyter Notebook or VS Code.

4.  Run all cells sequentially.

------------------------------------------------------------------------

## 📈 Key Learning Outcomes

-   Understanding difference between tidying and cleaning
-   Applying statistical techniques for outlier detection
-   Using imputation correctly for different data types
-   Writing clean, readable, and structured data engineering code
-   Improving dataset reliability before analysis or modeling

------------------------------------------------------------------------

## ✅ Final Result

The final dataset is: - Clean - Complete - Structured - Free of major
inconsistencies - Ready for visualization or machine learning tasks

------------------------------------------------------------------------

## 👤 Author

Viraj Mistry\
PROG8245 -- Data Engineering Lab\
Week 5 Assignment
