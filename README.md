# Power-BI-Healthcare-Dashboard
An ongoing project from AtoZ for Healthcare Dashboard Development Process

#### Process
<details>

<summary>1. Requirement Gathering Phase</summary>

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

<summary>2. Data Collection</summary>

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

<summary>3. Data Transformation & Modelling</summary>

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

<summary>4. Data Visualization Blueprint</summary>

You are expected to get a clear understanding about your data thru
- Transformation
- Modelling
- Gaining domain expertise

at this stage this is where we will hold meeting etc

and make a blueprint for our dashboard

there are2 pages; summary & detail

divide into 4 section: top left, top right,middle and bottom section

</details>


<details>

<summary>5. Dashboard layout & design</summary>

_Tips:_ In view taskbar, enable gridline and snapping

**We will be using DAX**
- as to create dynamic data and create new measure

i. As we want to put total wait list at any latest month (top left)

For DAX, we will count the sum of wait list for the maximum date from the dataset
> Latest Month Wait List = Calc(Sum(all_data(total))), All_data(Archive Date) = Max(All_data(Date))
> to simplify, this is a calculation for the total wait list and filter it according to the latest month
> and for previous year, use EDATE before max and minus 12 (for last year)

ii. This is a section for avg wait list value for particular measure
>but,there are an issue wth outliers, which is why we will also be using median

a. we will ad toggle function (slicer) by adding blank table for avg and median
>this will be a dummy table which does not hold any value apart from that two avg med

b. add a measure to let us interact to switch between avg and median
>basically,when we click avg, it will make a calculation with avg, and vice versa

_add legend to main division,and add values if there is a filter or toggle, eg: for donut chart case type_

on time bands

_if there are too many duplicate values/; TRIM_

_if there are similar values but different name, replace values_


</details>




<details>

<summary>Insert Here</summary>

</details>



this is still ongoing, will be updated from time to time
