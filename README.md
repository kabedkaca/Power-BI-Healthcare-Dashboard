# Power-BI-Healthcare-Dashboard
An ongoing project from AtoZ for Healthcare Dashboard Development Process

#### Process
<details>

<summary>**1. Requirement Gathering Phase**</summary>

- Identify Stakeholder
  > establish point of contact (user who use dashboard, clarify your doubt)
- Understand business objective
  > meeting & communication, set objective & goal,
- Data study
  > data source, column desc, data type, volume/frequency & Data quality
- Define Scope
  > doc KPI, timeline, expectation

Never forget to document your step
80: 20 rule
keep 80 buffer
always overdeliver

_Let's understand the project_

Project Goal: 
1. Track curent status of patient waiting list
2. Analyze historical monthly trend of waiting list in Inpatient & Outpatient categories
3. Detail speciality level and age profile analysis

Metric:
1. Avg & Median of waiting list
2. Current total wait list

Views required:
1. Summary sheet
2. Detail page of granular analysis
   
</details>



<details>

<summary>**2. Data Collection**</summary>

Data connectors: excel, csv, sql db, Azure, JSON, Web

we use central folder connecteor
multiple excel file, form relationship
https://www.youtube.com/watch?v=G8ikAJele_s&list=WL&index=4&t=19s


when there are multiple file, check:
1. Column count are the same
2. Column header are the same

load the data


</details>

<details>

<summary>**3. Data Transformation & Modelling**</summary>

_What you need to check_
1. Data type (is correct with column content)
2. Date column (double check)
3. Split, add, merge when needed
4. total rows (transform>count row>remove at applied step(to not be confused)) tally with csv
5. form join by rename column that is the same thing
6. add column
7. Append table (combine to be new table)

dont forget to close and apply

hiding view the inpatient/outpatient table to avoid confusion (in modelwindow)




</details>

<details>

<summary>**Insert Here**</summary>

</details>



this is still ongoing, will be updated from time to time
