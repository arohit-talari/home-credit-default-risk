<p align="center">
  <img src="images/home_credit_group.png" width="400">
</p>

<h1 align="center">Home Credit Group - Characteristics of Default Behavior </h1>

<h1 align="center">Project Overview</h1>

Home Credit Group is a global consumer finance company specializing in loans to underbanked borrowers — a population largely excluded from traditional credit markets due to limited or nonexistent credit histories. Without conventional credit scores, the core underwriting challenge is identifying which borrower characteristics reliably predict repayment behavior.

That challenge defines this project:

> **What combination of borrower characteristics separates low-risk borrowers from high-risk ones?**

The dataset spans 307,511 loan applications across 122 columns — covering borrower demographics, income and employment profile, housing status, external risk scores, and credit history indicators. Column scoping was the first and most consequential decision. Working from understood variables outward, then filling gaps through research into Home Credit's specific lending context, 97 columns were excluded across three groups: property-related columns averaging 58% missingness, contact flag columns with near-zero analytical variance, and credit bureau inquiry columns with correlations near zero against the default outcome. Several columns initially flagged for removal were retained — as the basis for flag logic, segmentation bins, or derived metrics the analysis would depend on. The 25-column working dataset was deliberately constructed, not simply reduced.

Seven distinct missingness scenarios required resolution before analysis could begin — each handled on its own terms rather than through uniform imputation.

The project ran across two phases: data cleaning and transformation to resolve structural, missingness, and encoding issues, followed by exploratory data analysis to isolate the patterns defining borrower risk.

The analysis identified a clear high-risk profile. Borrowers who are under 40, Low or Mid income, living in unstable housing, and carrying a debt-to-income ratio above 0.20 default at **14.30%** — 77% above the **8.07%** portfolio benchmark. The low-risk profile defaults at **5.42%**. The **8.88 percentage point spread** directly answers the core question. Seven findings followed — spanning demographic risk signals, financial ratio thresholds, and composite borrower profiles — each with direct implications for credit underwriting decisions.

---
<h1 align="center">Skills Demonstrated</h1>

---
<h1 align="center">Dataset</h1>

---
<h1 align="center">Data Cleaning Approach</h1>

--- 
<h1 align="center">Key Findings</h1>

---
<h1 align="center">Scripts</h1>

- **[Data Cleaning Script](scripts/home_credit_data_cleaning.sql)**: Prepares the dataset for analysis by resolving missing values, correcting data inconsistencies, applying type conversions, and constructing derived variables.

- **[Exploratory Data Analysis (EDA) Script](scripts/home_credit_eda.sql)**: Analyzes the cleaned dataset to identify borrower risk patterns, quantify default rate drivers, and generate the key findings presented in this project.

---
<h1 align="center">Tools Used</h1>

<div align="center">

![MySQL](https://img.shields.io/badge/MySQL-9.x-blue)
![SQL](https://img.shields.io/badge/SQL-Data%20Analysis-lightgrey)

</div>

- **MySQL (v9.5.0)** — data cleaning, transformation, and analysis
- **SQL** — query development and exploratory analysis
