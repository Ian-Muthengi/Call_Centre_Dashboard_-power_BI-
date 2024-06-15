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

- What is the overall response time?
- What is the highest sentiment in calls or customer satisfaction?
- What day of the week experiences the highest volume of calls?

### Data Analysis
Features worked with:

1. SQL
```sql
-- Selecting with a condition
SELECT * FROM Call_Center
WHERE sentiment = 'Negative';
```

2. Python
```python
# Transposing data
import pandas as pd

# Replace 'input.csv' with the path to your CSV file
input_file = r'C:\Users\ian.muthengi\Downloads\Call_Center.csv'

# Read the CSV file into a pandas DataFrame
df = pd.read_excel(input_file)

# Transpose the DataFrame
df_transposed = df.transpose()

# Replace 'output_transposed.csv' with the desired output file name
output_file = 'C:/Users/ian.muthengi/Downloads/transposed_Call_Center.csv'

# Write the transposed DataFrame to a new CSV file
df_transposed.to_excel(output_file, index=True, header=False)
```

### Results/Findings
The analysis results are summarized as follows:

1. 75% of the calls were answered or responded to within that time frame.
2. The negative sentiment is dominant, with a total range of 11,063.
3. Thursday and Friday are the busiest days of the week with the highest number of calls.

### Recommendations
Based on the analysis, we recommend the following actions:

1. Aim to improve response times for the remaining 25% of cases that fall beyond the 75th percentile.his could involve optimizing processes or implementing automation for quicker responses to common queries.
2. Conduct seminars for staff on customer handling to curb negative sentiments.
3. Consider allocating more staff or resources on Thursdays and Fridays to handle the increased call volume efficiently.

### Limitations
Call center data may not capture every interaction or detail, leading to gaps in understanding customer experiences or issues.
