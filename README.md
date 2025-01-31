# Credit Score Analysis

---

## Data Cleaning Strategy and Financial Analysis

###### By: Jennifer Mancheno

The dataset, sourced from Kaggle’s Credit Score Classification dataset, originally contained two CSV files with 150,000 rows of data. These were merged to create a concatinated dataset, resulting in enhanced analysis. Over 11,000 unique customer records were identified, and efforts were made to retain as much credit score data as possible.
The cleaned dataset can be found in Resources, cleaned_data.csv. 

### Key Cleaning Steps:

* **Handling Missing Values:**

  * Customer information with multiple NaN values was filled based on `<span>customer_id</span>` mapping, ensuring data consistency.
* **Occupation Column Cleaning:**

  * Some customers had occupation data with typos or missing values. The most common occupation associated with a `<span>customer_id</span>` was used for consistency.
* **Loan Data Cleaning:**

  * Loan data contained typos, underscores, symbols, and negative numbers.
  * Since the number of loans must be an integer greater than 0, erroneous values were corrected using `<span>customer_id</span>` mapping and a function with `<span>lambda</span>` to ensure positive values.
* **Credit History Age Standardization:**

  * The original dataset contained credit history age in years and months.
  * A new column, `<span>credit_history_age_months</span>`, was created to convert this information into numerical months for easier analysis.



The financial analysis of quarterly reports was conducted in Project 3 - quarterly_reports_analysis.ipynb, to generate insights that drive effective critical change management.

---

## Age Group Analysis

###### By: Khlood Azam

### Age Group 18-25:

* **1,556** "Good" credit scores
* **3,564** "Poor" credit scores
* **5,583** "Standard" credit scores
* **Insight:** A significant portion of younger individuals have "Poor" and "Standard" credit scores. This suggests they are either in the early stages of building their credit or struggling with financial management.

### Age Group 26-35:

* **2,081** "Good" credit scores
* **4,716** "Poor" credit scores
* **7,380** "Standard" credit scores
* **Insight:** Credit scores show a slight improvement as individuals move into their 30s. However, financial challenges such as loans continue to result in a high number of "Poor" credit scores.

### Age Group 36-45:

* **2,051** "Good" credit scores
* **4,576** "Poor" credit scores
* **7,464** "Standard" credit scores
* **Insight:** Gradual progress is evident, with more individuals improving their credit scores. However, a significant number still have "Poor" credit, likely due to ongoing financial commitments.

### Age Group 46-55:

* **1,932** "Good" credit scores
* **1,044** "Poor" credit scores
* **3,565** "Standard" credit scores
* **Insight:** Credit management improves significantly, with a sharp decline in "Poor" credit scores. Many individuals in this group likely benefit from debt repayment and better financial habits.

### Age Group 56-65:

* **175** "Good" credit scores
* **50** "Poor" credit scores
* **331** "Standard" credit scores
* **Insight:** Strong credit stability is observed, with very few individuals having "Poor" credit scores. This suggests increased financial security leading up to retirement.

### Age Group 66-75:

* **286** "Good" credit scores
* **1,670** "Poor" credit scores
* **2,088** "Standard" credit scores
* **Insight:** A spike in "Poor" credit scores is noticeable, likely due to retirement and reduced income, leading to financial instability.

---


# Occupation Credit Scores Over Time

###### By: Deniza Robinson

## Overview

This project visualizes how credit scores fluctuate for various occupations throughout the year. Each occupation is categorized into one of three credit score levels:

* **Good (Green)**
* **Standard (Blue)**
* **Poor (Red)**

### Key Insights:

* **Good Credit Scores:**
  * Occupations like **Accountants, Doctors, and Architects** consistently maintain high credit scores, particularly in May, October, and November.
* **Standard Credit Scores:**
  * Occupations such as **Engineers and Mechanics** display stable, standard credit scores, especially in July.
* **Poor Credit Scores:**
  * Professions like **Teachers, Media Managers, and Lawyers** show poor credit scores in months like February and June. This suggests possible seasonal financial stress or variable income trends.

## Conclusion

The data indicates that professions with higher earnings and financial literacy, such as **Accountants and Doctors**, tend to maintain better credit scores over time. Conversely, some occupations struggle to maintain good credit scores during specific months, likely due to income variability or external financial pressures.

---

# Research Questions Addressed

###### By: Sukhwinder Singh

1. **How does credit score vary by occupation?**
2. **How does payment behavior impact credit score?**

### Findings:

* Occupations such as **Architects, Engineers, Entrepreneurs, Mechanics, Scientists, and Writers** tend to have lower credit scores.
* Individuals with **high spending but medium-value payments** are more prone to poor credit scores.

This analysis provides a clearer understanding of financial behavior across different demographics and professions, offering insights into credit score management and financial stability trends.
