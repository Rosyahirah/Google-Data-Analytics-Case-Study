# Google-Data-Analytics-Case-Study

# Case Study 2: How Can a Wellness Technology Company Play It Smart?

# Introduction

In this case study, I will perform real-world tasks of a junior data analyst that are working for Bellabeat, a high-tech manufacturer of health-focused products for women, and meet different characters and team members. 
In order to answer the key business questions, I will follow the steps of the data analysis process: ask, prepare, process, analyze, share, and act. 

# Scenario

Bellabeat is a successful small company, but they have the potential to become a larger player in the global smart device market. Urška Sršen, cofounder and Chief Creative Officer of Bellabeat, believes that analyzing smart device fitness data could help unlock new growth opportunities for the company. I have been asked to focus on one of
Bellabeat’s products and analyze smart device data to gain insight into how consumers are using their smart devices. The insights that I discover will then help guide marketing strategy for the company. 

# Ask

1. Identify the business task:
To analyse Bellabeat's competitor's smart devices usage data in order to identify potential growth opportunities and recommedations for marketing strategy based on the trends found in the analysis.

2. Consider key stakeholders:
- Primary Stakeholder: Urška Sršen (Bellabeat’s cofounder and Chief Creative Officer), Sando Mur (Mathematician and Bellabeat’s cofounder), key member of the Bellabeat executive team
- Secondary stakeholder: Bellabeat marketing analytics team

3. Questions for the analysis:
- What are some trends in smart device usage?
- How could these trends apply to Bellabeat customers?
- How could these trends help influence Bellabeat marketing strategy?

# Prepare

Data Source: 30 participants FitBit Fitness Tracker Data from Mobius: [https://www.kaggle.com/arashnic/fitbit](https://www.kaggle.com/datasets/arashnic/fitbit)

The dataset has 18 CSV. I will use ROCCC to figure out if this data has any problems with bias or credibility:

- Reliability : LOW – dataset was collected from 30 individuals who have been tracked for just 1 month. There are missing key indicators such as gender, age and lifestyle.
- Originality : LOW – third party data collected using Amazon Mechanical Turk.
- Comprehensive : LOW - The data are not complete because they are missing some information that would help make a more accurate analysis (e.g., sex, age, height, etc.).
- Current : MEDIUM – data is 7 years old. Data is not current so the users habit may be different now.
- Cited : HIGH – data collector and source is properly documented.

Overall the analysis we discuss the data now here is finding some insight into Bellabeat future marketing strategy.

# Process

I have downloaded, extracted the files and used appropriate file-naming conventions.

Firstly, I will clean the data for duplicate and error by using Excel.
The following steps were taken within each dataset:

1. Sorted and filtered data by Id to obtain how many unique users there were within the dataset.
2. Checked for duplicate data using the ‘duplicate data’ tool in Excel
3. Formatted date data into MM/DD/YY date format
4. Formatted all numerical data into Number format with either no decimals or up to 2 decimals.
5. Add a new file in which we add Activity Column in Daily_Activity_Merged then save as a new file DailyActivity_Merged_Weekday. So,the formula below is used to add days names from the date we can easily analyze by days and weekends through this column:
=CHOOSE(WEEKDAY(B2),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")

I am using Biguery for data analyses which is called Bigquery Sandbox and each files are uploaded each file one by one. 



