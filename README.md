# 📞 Telco Customer Churn Prediction (Binary Logistic Regression)

## Project Overview

This project implements a **Binary Logistic Regression model** to predict customer churn in a telecommunications company using the Telco Customer Churn dataset. The primary goal was to identify the most significant factors driving customers to leave (churn) and to build a predictive model that can inform targeted customer retention strategies.

This analysis was completed as a final project for a Categorical Data Analysis course (STAT 410).

**Data Source:** The original dataset is hosted on Kaggle: [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data].

## 📊 Key Findings

The final logistic regression model provided a strong fit (Hosmer-Lemeshow $p=0.62$, Overall Accuracy $80.32\%$) and identified several critical churn drivers:

| Feature | Key Insight | Odds Ratio (OR) Example |
| :--- | :--- | :--- |
| **Contract Type** |**Longer contracts** (One- and Two-year) are the strongest factor for reducing churn risk, with two-year contracts reducing the odds by $94\%$. | Two-year contract OR ≈ 0.06 |
| **Internet Service** | Customers using **Fiber Optic** internet are significantly more likely to churn, with churn odds over 14 times higher. | Fiber Optic OR ≈ 14.06 |
| **Tenure** | **Longer tenure** generally reduces the odds of churning (OR $\approx$ 0.95). This protective effect is strengthened by longer contracts (significant interaction). | Tenure OR ≈ 0.95 |
| **Monthly Charges** | **Higher charges** are linked to slightly lower churn risk (OR $\approx$ 0.93). | Monthly Charges OR ≈ 0.93 |

---

## ⚙️ How to Reproduce the Analysis

The analysis was performed using **R** and the **Quarto** format.

### Requirements
* **R** and **RStudio**
* **R Packages:** `tidyverse`, `car`, `corrplot`, `ResourceSelection`, `caret`, `pROC`

### Steps
1.  Clone this repository to your local machine.
2.  Download the `Telco.csv` data file from the Kaggle link above or place your copy in the `Data/` subfolder.
3.  Open the `Ololade_Akinsanola_Project.qmd` file in RStudio.
4.  Run the code chunks sequentially to reproduce the data cleaning, descriptive statistics, model fitting, and diagnostics.

---

## 📁 Files in This Repository

| File | Purpose |
| :--- | :--- |
| `README.md` | **Primary file.** Project summary, key findings, and setup instructions. |
| `Ololade_Akinsanola_Project.qmd` | **The reproducible analysis code.** Contains all R code, outputs, and visualizations. |
| `Ololade_Akinsanola_Final_Report_STAT410.pdf` | The complete written report for the course (supplementary). |
