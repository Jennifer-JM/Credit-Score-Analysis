# Project-3


#Credit Score Distribution by Age Group 

•    Age Group 18-25:
o    1,556 "Good" credit scores.
o    3,564 "Poor" credit scores.
o    5,583 "Standard" credit scores.
o    Insight: A large portion of younger individuals have "Poor" and "Standard" credit scores, indicating that many may be in the early stages of building their credit or struggling with managing finances.
•    Age Group 26-35:
o    2,081 "Good" credit scores.
o    4,716 "Poor" credit scores.
o    7,380 "Standard" credit scores.
o    Insight: A slight improvement in credit scores is seen as people move into their 30s, but financial challenges, such as loans, still result in high numbers of "Poor" credit scores.
•    Age Group 36-45:
o    2,051 "Good" credit scores.
o    4,576 "Poor" credit scores.
o    7,464 "Standard" credit scores.
o    Insight: This age group shows gradual progress, with more individuals moving toward better credit. However, "Poor" credit scores are still common, likely due to ongoing financial commitments.
•    Age Group 46-55:
o    1,932 "Good" credit scores.
o    1,044 "Poor" credit scores.
o    3,565 "Standard" credit scores.
o    Insight: Credit management improves significantly in this group, with a sharp decline in "Poor" credit scores. Individuals likely benefit from having paid off debts and managing credit more effectively.
•    Age Group 56-65:
o    175 "Good" credit scores.
o    50 "Poor" credit scores.
o    331 "Standard" credit scores.
o    Insight: This group shows strong credit stability, with very few individuals having "Poor" credit scores. Financial stability is likely leading up to retirement.
•    Age Group 66-75:
o    286 "Good" credit scores.
o    1,670 "Poor" credit scores.
o    2,088 "Standard" credit scores.
o    Insight: There is a spike in "Poor" credit scores, likely due to retirement and reduced income, which challenges financial stability in this age group.




#Data Cleaning Strategy 

By extracting the data from Kaggle, the Credit Score Classification dataset, that contains two csvs’ having 150,000 rows of data, the csvs’ were concatenated into one to create a unified dataset which results in an enhanced analysis. There are over 11k unique records of customers. Ensuring the majority of customer credit score data was not deleted, was prioritised. Some challenges faced were, where there were multiple NaN values in the columns, info was filled in based on their customer_id mapping. Customer_id mapping is based on previous records of a customer_id. This assured that the dataset is accurate.For example:

Occupation column
Some customer’s occupation info varies with it having typos or NaN. The data was cleaned by using the most common occupation of the customer, as their occupation info Num of loans

Some customer’s data had various typos with underscores, or symbols, and negative numbers. Number of loans can only be greater than 0 and an int. The data was cleaned by using the cumstomer_id mapping and removing discrepancies through a function and using lambda to assure positive numbers were greater than 0. (edited) 

# Occupation Credit Scores Over Time
## Overview
This project visualizes the credit scores of various occupations across a year, focusing on month-to-month variations. Each occupation is categorized into one of three credit score levels:
- **Good (Green)**
- **Standard (Blue)**
- **Poor (Red)**
The visualization offers insights into how different occupations fare in terms of credit score stability and fluctuation throughout the year.
 Key Insights
1. Good Credit Scores:
   - Occupations like **Accountants**, **Doctors**, and **Architects** consistently maintain high credit scores, especially during months such as **May**, **November**, and **October**.
2. Standard Credit Scores:
   - Occupations such as **Engineers** and **Mechanics** display steady, standard credit scores across the year, notably in **July**.
3. Poor Credit Scores:
   - Professions like **Teachers**, **Media Managers**, and **Lawyers** experience poor credit scores in months like **February** and **June**. This may suggest seasonal financial stress or variability in income during those periods.
 Conclusion
The data indicates that higher-paying or financially literate professions, such as Accountants and Doctors, tend to have better financial stability and credit scores over time. Conversely, some occupations face challenges in maintaining good credit scores during certain months, potentially due to variable income or external financial factors.


We format our data set by creating certain new columns such as we create new columns for different types of loans as we got a single column with different types of loans in available data set.
In the original data set we have a column of credit history age with info in form of years and months. We convert It to new column named credit history age month with a numeric value of months so that it can use further for analysis of data.
Questions:
I tried to address two questions from this data set:
Que. 1: What is a credit score by Occupation?
Ques 2. How the Payment Behaviour affect the Credit Score?
Conclusions:
Occupations such as Architect, Engineers, Entrepreneurs, Mechanics, Scientists and writers are more tilt towards poor credit score.
High spent medium value payments behaviour is more prone to poor credit score
