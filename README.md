# Hospital-Performance-Analysis
High Level KPI Power BI report for the executive team based on the patient records

# Summary of the Project
The task is to build a High Level Power BI KPI report for the executive team, based on the subset of patients records. The purpose of the report is to give stakeholders visibility into the hospital recent performance, and answer the following primary questions:  
  1. How mnay patients have been admitted or readmitted over time?
  2. How long patients staying in the hospital, on average?
  3. How much is the average cost per the visit?
  4. How many procedures are covered in the insurance?
     
Tasks Performed:
1. Data Import and cleaning with power query.
2. Data modelling
3. Data Exploration based on Patients and Revenue Analysis
4. Preparing Reports and Drafting KPI Dashboard
5. Analyzing the data for Insights and Providing recommendations to increase the revenue and Patient satisfaction

# Objective:
To build a High Level Power BI KPI report for the executive team, to give visibility into the recent hospital performance and to potentially increase the revenue and patient satisfaction

# Process:
# Data Import and Cleaning using Power Query
1. Importing the data using power query through folder option and then expanding the tables one by one.
2. Checking the distribution of each and every column using column distribution feature in power query and identify the nulls/empty values
3. Modifying the data types if the default values are incorrect
4. Replacing the null values in the Reason description of Encounter/ Procedures tables:
![image](https://github.com/user-attachments/assets/2f20275a-a208-4932-90c3-ec2e752c44e5)

# Data Modeling
1. After importing the data to the power bi engine through power query, data modeling was performed and below attached are the details of the tables:
![image](https://github.com/user-attachments/assets/c8fee63e-61e2-4ff9-ad78-07d17fc2408b)
2. Cross filter direction has been set to "both" for 3 tables (encouters, procedures and patients)
3. And understand the columns of each table for report generation

# Patients Analysis
![image](https://github.com/user-attachments/assets/41336582-8f0b-46e1-b476-37830b0d3c1c)
Since data was subset of patient records, i proceeded to analyze the patient data, which was patient demographics data and then encounter reason and procedrues performed at a time.
# Insights 
1. In the span of 11 years from 2011 to 2022 (for 2022 data available only till Q1) we have overall 28K visits, which is not quite normal we will be seeing why..
2. Total distinct or unique patients visited were 974, and average age was 69 and we are seeing a down trend in the average visited.
3. since the data was skewed for the number of encounters and procedures, i have summarized using median we have 14 encounters and 20 procedures
4. we have seen a spike of patients readmission rates and admissions in 2014 due to boston public health emergency and covid-19 pandemic during 2020 and 2021.
5. Mainly ambulatory and outpatient encounter class take more than 50% of the visits and most visits end in a single encounter.
6. Most of the encounters and procedures were not classified according to the SNOMED-CT, which can be improved and excluding these, chronic congestive heart failure, hyperlipidemia and Normal pregnancy are the main encounter reasons and acute bronchitis, normal pregnancy and atrial fibrillation were the main procedures performed during these encounters

# Revenue Analysis
![image](https://github.com/user-attachments/assets/8f3390e3-c462-4100-bf9c-e3d53e7193c8)
Up next Revenue from the patients visits!
1. over the years we have generated $241.37M revenue, which is quiet less as we can understand so far since the average age of patients visited is 69 and emergency is the main encounter class but we are seeing a down trend in the average age becuase of the normal pregnancy admissions, recommendations at last!
2. Total claim cost was $101.53M and revenue per patient is $247.81K and Average cost per visit is $8.65K. As per Agency for Healthcare Research and Quality for a public hospital $550 is the average cost in U.S but compared to boston hospital prices it is reasonable.
3. Around 100M comes from the patients who do not have a insurance

# Final KPI Report
![image](https://github.com/user-attachments/assets/4455b524-71b9-456a-9b9a-227d5bf85f96)
I have took the most important KPI's from patients/Revenue Analysis for quick glance to hospital performance.

# Key Take Aways and Recommendations
1. As seen in the Analysis Average Age of the patients visited is 69, and mostly becuase of ambulatory encounters and to increase revenue, it is a must to focus on younger generation. may be ad campaign/ promotions for yonger people with more focus on pregnancy.
2. Around $100 M comes from Records related to encounters/ Procedures that were not marked according to SNOMED-CT, which will be necessary to track all the encounters/procedures it is recommended to imporve the coding, billing and Data Collection and Classification.
3. Out of all the encounter classes, the wellness and inpatient department lacks, its important to imporve the wellness department if we are going to promote for the younger generation and inpatient department inforastructure can be improved to increase the patient time spent and in turn revenue.
4. Readmission Rate is very high considering mostly aged patients visit the hospital but its suggested to check on the infra/support/crew for any improvements.
5. Around $ 100M comes from patients who don't have an insurance, its recommended to collaborate with the insurance payer for the campaigns/ Discounts.
