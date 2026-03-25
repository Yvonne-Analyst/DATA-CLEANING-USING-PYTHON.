# DATA-CLEANING-USING-PYTHON.
**MARKETING CAIMPAIGN DATA CLEANING PROJECT.**
 
**Overview**
This project focuses on cleaning and preparing a messy marketing campaign dataset using Python in a Jupyter Notebook.
The goal was to transform raw, inconsistent data into a structured and analysis-ready dataset by applying practical data cleaning techniques.



**Tools & Technologies**

Python, 
Jupyter Notebook, 
Pandas,
NumPy


**Dataset**
File: marketing_campaign_data_messy.csv

Contains campaign-level data such as:
Campaign ID,
Campaign Name,
Channel,
Spend,
Impressions & Clicks,
Start & End Dates,
Campaign Status (Active/Inactive)


**Data Cleaning Steps**
1. Column Standardization
Converted column names to lowercase
Replaced spaces with underscores
Removed extra whitespace
2. Spend Column Cleaning 
Removed currency symbols (e.g. $)
Converted values to numeric format
3. Channel Name Fixes 
Corrected inconsistent naming:
Facebok → Facebook
Insta_gram → Instagram
Gogle → Google Ads
Tik_Tok → TikTok
E-mail → Email
Replaced invalid values (N/A) with nulls
4. Boolean Conversion 
Standardized the active column:
Converted values like Yes, Y, 1 → True
Converted No, 0 → False
5. Date Formatting 
Converted start_date and end_date to datetime format
Handled invalid dates using coercion
6. Duplicate Columns Removal
Removed duplicated columns from the dataset
7. Data Quality Checks 
a) Logical Errors
Identified cases where:
clicks > impressions (invalid scenario)
b) Date Issues
Fixed campaigns where:
end_date < start_date
Solution:
Adjusted end date to be 30 days after start date
8. Outlier Treatment 
Used IQR method to detect extreme spend values
Capped outliers at the upper limit
9. Feature Engineering 
Extracted season information from campaign names


**Final Output**
Clean, structured dataset ready for:
Data analysis
Visualization
Machine learning


**Key Learnings**
Handling messy real-world data
Data validation and cleaning strategies
Feature engineering techniques
Working with dates, strings, and numeric conversions


**Author**
Yvonne Mumbia
