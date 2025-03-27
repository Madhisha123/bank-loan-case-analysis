# Bank Loan Case Study - Payment Difficulty Prediction

> **Objective:** Identify patterns indicating whether a customer is likely to face difficulty in paying loan installments. This project helps in making data-driven decisions such as loan approval, adjusting loan amounts, or applying higher interest rates to risky applicants.

---

## 🟣 Overview

This project aims to analyze customer loan application data and identify potential indicators of payment difficulties. By detecting patterns associated with financial risk, the business can:
- Make informed lending decisions
- Reduce financial losses due to defaults
- Adjust loan terms for risky applicants

The analysis is conducted using **Microsoft Excel** for data cleaning, preprocessing, and exploratory analysis.

---

## 🟡 Problem Statement

The bank wants to predict:
- Whether a client will have payment difficulties
- The relationships between customer attributes and repayment issues
- The factors most correlated with risk

---

## 🟢 Solution Approach

### 1. Missing Value Handling
- Identified missing data using `COUNTBLANK()` and `COUNT()` formulas.
- Columns with **less than 50%** data were removed if irrelevant.
- Columns with **more than 55%** missing values were treated:
   - **Numerical columns:** Imputed using mean or median.
   - **Categorical columns:** Imputed using mode.

---

### 2. Outlier Detection
- Outliers were detected using:
   - Quartile 1 (Q1), Quartile 3 (Q3)
   - Interquartile Range (IQR)
   - Upper & Lower bounds (UpperForm & LowerForm)
- Outliers were flagged for further analysis.

---

### 3. Data Imbalance Analysis
- Evaluated the imbalance between:
   - **Class 0**: No payment difficulty (≈ 92%)
   - **Class 1**: Payment difficulty (≈ 8%)
- Visualized class imbalance using **pie charts**.
- Calculated imbalance ratio.

---

### 4. Exploratory Data Analysis (EDA)

#### a) Univariate Analysis
- Studied distributions of individual variables (e.g., Income, Credit Amount).

#### b) Segmental Univariate Analysis
- Compared distributions under different scenarios (e.g., default vs. no default).

#### c) Bivariate Analysis
- Explored relationships between variables and the target variable using:
   - Cross-tabulation
   - Income Bin vs. Target
   - Credit vs. Applicants
   - Average Amount Credit vs. Income Bin
- Visualized using **bar charts**.

---

### 5. Correlation Analysis
- Performed segment-wise correlation analysis:
   - Clients with payment difficulty vs. others.
   - Identified top correlations for both segments.
- Color-coded the correlation heatmap:
   - Low: Red
   - Medium: Yellow
   - High: Green

---

## 🛠️ Tools Used
- **Microsoft Excel**
   - Data Cleaning
   - Outlier Detection
   - Data Imbalance Detection
   - Exploratory Data Analysis
   - Correlation Analysis

---

## ✅ Results
- Identified significant patterns related to:
   - Loan defaults.
   - Correlation between income, credit, and payment difficulties.
- Detected a severe **data imbalance**.
- Generated actionable insights for adjusting lending strategies based on customer profiles.

---

## 📂 Repository Structure

