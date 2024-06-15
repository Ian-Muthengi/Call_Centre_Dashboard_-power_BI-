# Call Centre Analysis

## Table of Contents

- [Project Overview](#project-overview)
- [Tools](#tools)
- [Data Analysis](#data-analysis)
- [Recommendations](#recommendations)

### Project Overview

This project involves analyzing the call center performance of a particular company. Our objective is to explore response times, reasons for calls, and customer satisfaction. By thoroughly examining different aspects of the call center data such as quality, convenience, and response times, we aim to gain a holistic understanding of the company's performance. This analysis will provide actionable insights to improve strategic decision-making processes.

<img width="590" alt="Call center dashboard picture" src="https://github.com/IanLiam/Call_Centre_Dashboard/assets/117744677/93121823-ba54-45ba-b8d6-fdd323c8b626">


### Data Sources
The data set used for this analysis is the "Call_center_data.csv" file, which contains comprehensive details about every call made to the company.

### Tools
- Excel - Data Cleaning  [Download here](https://www.microsoft.com/en-us/microsoft-365/download-office)
- Python - Data Cleaning  [Download here](https://www.anaconda.com/download)
- MYSQL - Data Analysis [Download here](https://www.mysql.com/)
- PowerBI - Creating reports  [Download here](https://powerbi.microsoft.com/en-us/downloads/)

### Data cleaning/ Preparation
In the initial data preparation phase, we performed the following tasks:

1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting.

### Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions, such as:

- What is the overall sales trend?
- Which products are top sellers?
- What are the peak sales periods?

### Data Analysis
Features worked with:

1. SQL
```sql
-- Selecting with a condition
SELECT * FROM Sales
WHERE cond = 2;
```

2. Python
```python
# Transposing data
import pandas as pd

# Replace 'input.csv' with the path to your CSV file
input_file = r'C:\Users\ian.muthengi\Downloads\Sales.xlsx'

# Read the CSV file into a pandas DataFrame
df = pd.read_excel(input_file)

# Transpose the DataFrame
df_transposed = df.transpose()

# Replace 'output_transposed.csv' with the desired output file name
output_file = 'C:/Users/ian.muthengi/Downloads/transposed_sales.xlsx'

# Write the transposed DataFrame to a new CSV file
df_transposed.to_excel(output_file, index=True, header=False)
```
3. Power BI

### Results/Findings
The analysis results are summarized as follows:

1. The company's sales have been steadily increasing as from 2021 to 2022, with a noticeable peak during the holiday season.
2. Product41 is the best-performing category in terms of sales.
3. Direct sales account for the highest percentage in terms of sales type.

### Recommendations
Based on the analysis, we recommend the following actions:

1. Invest in marketing and promotions during peak sales seasons to maximize revenue.
2. Focus on expanding and promoting products41.
3. Emphasize expanding and promoting direct sales.

### Limitations
I had to remove all zero values from buying price and selling price columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both buying price and number of votes with selling price.
