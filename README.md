# DSA-Second-Project-Documentation-2
Palmora Group HR Analysis
# Introduction
The manufacturing industry has long been recognized as a sector with unique workforce
challenges. In this report, we analyze HR data from a manufacturing company with a focus
on gender distribution, performance ratings, and salary structure. The primary aim is to
uncover insights regarding gender inequality and potential pay gaps in the organization. This
analysis is particularly relevant as companies increasingly turn to data-driven decisionmaking to ensure fair HR practices and regulatory compliance across regions and
departments.
The dataset under review comprises employee information with attributes such as Name,
Gender, Department, Salary, Location, and Rating. Special attention is given to issues related
to missing or inconsistent data. For example, some entries have blank or missing Gender
values and some contain the literal string “NULL” for department. In addition to providing an
in-depth exploratory data analysis (EDA), this report examines whether the company meets.
the new regulation mandating a minimum salary of $90,000, by analyzing salary distributions
in $10,000 bands across different regions.
This report is structured into several sections. First, we describe the data cleaning steps
taken to prepare the dataset for analysis. Thereafter, we examine the distribution of gender
across the organization overall, as well as within distinct departments and regions. We then
analyze performance ratings as they correlate with gender, moving on to a detailed study of
salary structures and pay gaps. Although a bonus calculation is mentioned in the case
study, the absence of a bonus rule dataset prevents us from performing this part of the
analysis. The report concludes with key .
# Data Cleaning and Preparation
A rigorous EDA begins with thoroughly cleaning the data to ensure that subsequent
analyses are accurate and reective of the true state of the organization. The cleaning
process was guided by the following specic tasks:
1. Handling Missing Gender Values:
Many employee records contained blank entries in the Gender column. To provide a
unied approach to analysis, all missing or blank values have been recategorized under
the new generic status “Unspecied.” This categorization helps in maintaining
consistency in subsequent counts and comparisons while ensuring that the inuence
of missing data is acknowledged.
2. Filtering Out Employees with Missing Salary:
Employees who do not have a recorded salary—most likely representing former
employees or incomplete records—were removed. Salary being a critical quantitative
measure, its absence could otherwise lead to inaccurate computations in salary
distribution and pay gap analyses.
3. Removing Incomplete Departmental Data:
There were multiple records in which the Department eld was recorded as “NULL.”
Since department afliation plays a key role in understanding gender distributions and
compensation patterns, these rows were eliminated to avoid skewing any departmentspecic insights.
![image](https://github.com/user-attachments/assets/bc2f9b67-dbe7-4142-b683-791f995eb764)
![image](https://github.com/user-attachments/assets/bfcdce00-82b2-4039-bf41-9506a026070b)

## Gender Distribution Analysis
Understanding gender distribution is pivotal for identifying discrepancies in workforce
composition, a key factor for both internal HR policies and external regulatory compliance.
This section examines the overall gender distribution, how it varies by region, and its
manifestation in different departments.
3.1 Overall Gender Distribution
The analysis begins with a count of all unique employee records after the data cleaning
procedure. The Gender column now contains three categories: "Male," "Female," and
"Unspecied." Although male and female genders are explicitly recorded, a signicant
proportion of employees initially had missing Gender data. By assigning these records to
the “Unspecied” category, the complete picture of gender distribution is made available.
Some key observations from the overall gender counts include:
A considerable number of employee records now fall in the “Unspecied” category,
highlighting potential issues with data collection or employees’ reluctance to disclose
personal information.
The counts for “Male” and “Female” provide a basis for calculating percentages. These
percentages are essential for comparing departmental and regional distributions later in
the analysis.

