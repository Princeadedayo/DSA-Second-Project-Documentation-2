# DSA-Second-Project-Documentation-2
Palmora Group HR Analysis
-  Power Bi [Download here](https://www.microsoft.com/en-us/download/details.aspx?id=58494)
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

3.2 Gender Distribution by Region
The regional breakdown of employee data provides insight into location-specic workforce
trends. By grouping the records based on the “Location” eld, we can observe how gender
distributions vary across different regional ofces or manufacturing sites.
Initial ndings indicate regional disparities in how many employees self-identify as male,
female, or remain unspecied. For instance, while some regions exhibit a relatively balanced
gender representation, others may have a larger proportion of “Unspecied” or may lean
more heavily toward one gender than the other. This divergence could be a function of local
labor practices, regional recruitment strategies, or cultural factors inuencing disclosure

Visual inspection of region-based gender differences was also facilitated by a pie chart
representation, which further highlighted that some regions had a signicant presence of
“Unspecied” genders. Such discrepancies warrant further investigation to determine if
data collection improvements or regional-specic policies are needed.

3.3 Gender Distribution by Department
Departmental analysis is integral to HR analytics, as diverse trends may emerge when
examining specic functional areas. Departments in the manufacturing sector may range
from production and engineering to quality assurance and administrative functions. The
cleaned dataset, having excluded records with incomplete department information, allowed
for a clear breakdown by department.
Preliminary analysis shows that some departments demonstrate a higher ratio of one
gender over the others. For example, production departments might traditionally see higher
male representation, while administrative units may show a higher count of female
employees. Additionally, departments with signicant “Unspecied” entries could indicate
areas where gender disclosure is either not well-tracked or an employee might choose to
avoid providing personal details. 

4. Performance Ratings Analysis by Gender
Performance ratings are key indicators of employee contribution and are often used for
salary determination, promotions, and other HR decisions. In this analysis, we segmented
performance ratings by gender categories to identify any patterns or potential biases.
Key steps in this analysis included:
## Categorizing Performance Metrics:
Each employee is assigned a performance rating (e.g., “Very Good,” “Good,” “Average,”
tc.). The distribution of these ratings was tallied across the “Male,” “Female,” and
“Unspecied” groups.
## Comparative Assessment:
Comparison of rating distributions among gender categories revealed whether one group
tends to have consistently higher ratings than another. A skewed distribution might
suggest either systemic bias or variations in performance evaluation criteria across
departments.
## Graphical Visualization:
A histogram and grouped bar charts were created to depict the percentage distribution
of each rating across the three gender categories. For example, if “Male” employees have
a higher proportion of “Very Good” ratings compared to “Female” employees, this may
warrant further review in performance evaluation procedures.
In the analysis of the cleaned dataset, it was observed that while the overall performance
ratings did not diverge signicantly between genders, subtle differences existed in some
regions and departments, suggesting potential areas for further investigation. This analysis
not only contributes to understanding current performance trends but also provides an
essential baseline for assessing the fairness of promotions and other HR decisions.

5. Salary Structure and Gender Pay Gap Analysis
The analysis of salary data is central to determining whether potential gender pay gaps
exist within the organization. This section offers a comprehensive overview of the
organization’s salary structure, examines compliance with regulatory standards for
minimum wages, and investigates differences in salary averages by gender across various
departments and regions.
5.1 Overall Salary Structure and Regulatory Compliance
Salary data from our cleaned dataset shows an extensive range of values. One of the
preliminary checks was to determine compliance with the new regulation, which mandates
a minimum salary of $90,000. This section highlights the following key points:
## Compliance Check:
A count was performed to determine the percentage of employees receiving a salary
below $90,000 in each region. This examination is critical because persistent
noncompliance in any region could lead to regulatory penalties or require corrective HR
actions.
## Descriptive Statistics:
Basic descriptive statistics (mean, median, and range) for salary were computed. These
statistics help capture the central tendency and dispersion of salary distributions overall
and by gender. Trends in these statistics across the different gender categories (Male,
Female, Unspecied) offer initial indications of a possible pay gap.
## Visualization of Salary Distribution:
A box plot was generated to compare salary ranges among the gender categories. The
visualization clearly marked outliers, interquartile ranges, and median salaries.
Observations from the box plot include differences in median salary values, which may
signal systematic disparities.
5.2 Salary Bands and Regional Distributions
To further analyze salary structures, salaries were grouped into $10,000 bands. This
approach not only highlights pay distribution but also enables a direct assessment of how
many employees fall below the regulatory benchmark of $90,000 in each region.
The process involved creating numeric intervals such as:
$20,000–$29,999
$30,000–$39,999
$110,000–$119,999
By mapping each employee’s salary to one of these bands, we derived the frequency of
employees per band for every region. 
5.3 Detailed Gender Pay Gap Examination
The central question of this research is to determine whether a gender pay gap exists
within the manufacturing company, and if so, under what conditions (departmental and
regional differences).
The approach followed includes:
## Comparative Average Salary Analysis:
Average and median salary gures were computed for male and female employees
(excluding “Unspecied” as a separate category) across the entire dataset as well as
within individual departments and regions. Any consistent difference in these averages
may indicate a pay gap that is correlated with gender.
## Departmental and Regional Segmentation:
To account for differences in job functions and geographical cost-of-living variations,
salary comparisons were segmented by both department and region. For instance, if
male employees in the Engineering department earn on average 10% more than female
employees in the same department, this difference might not be attributable solely to
differing skill levels but could reect inequities in pay structures.
## Visualizing the Pay Gap:
A series of side-by-side bar charts were constructed to compare male and female salary
statistics. One chart displays average salaries by department, while another shows these
averages by region.

# Conclusions and Recommendations

This detailed EDA of HR analytics in a manufacturing company has provided several key
insights into gender distribution, performance ratings, and salary structures. The analysis
not only reveals the current state of affairs but also highlights areas for potential
organizational improvement. 
A summary of the main insights is provided below:

### Data Cleaning Imperative:

• Missing or blank Gender values have been systematically recategorized as “Unspecied”
to ensure consistency.

• Records with missing Salary or Department data (marked as “NULL”) were removed,
assuring that further analysis is based on complete, reliable information.

## Gender Distribution Observations:

• Overall gender counts indicate a signicant presence of “Unspecied” entries,
suggesting a need for improved data collection protocols.

• Analysis by region shows variations in gender composition, which may be inuenced by regional labor market conditions or recruitment practices.

• Departmental breakdown indicates that certain functional areas exhibit imbalances,
possibly reecting traditional gender roles within the organization.
## Performance Ratings by Gender:

• While aggregate performance ratings are largely similar between male and female
employees, slight differences—observable in some regions and departments—highlight
the need for further qualitative review of evaluation criteria.

• An objective and consistent performance evaluation system is paramount to ensure
fairness and reduce any unintentional bias.

## Salary Structure and Gender Pay Gap:

• Descriptive salary statistics reveal that a non-negligible number of employees earn
below the mandated minimum of $90,000.

• Salary bands, segmented in $10,000 intervals, demonstrate that a considerable
proportion of employees fall within lower salary ranges, particularly in certain regions.


• Detailed departmental and regional comparisons point to a modest but consistent pay
gap between male and female employees, with male employees generally receiving
higher average salaries.

• The absence of bonus rule data limits the full exploration of total compensation
disparities; therefore, further analysis including bonus data is recommended.

## Final Remarks
This report provides a comprehensive HR analytics framework for assessing gender
distribution and pay gaps in a manufacturing environment. By following robust data
cleaning, visualization, and analysis practices as outlined above, organizations can identify
key areas of disparity and work proactively towards fostering an equitable workplace.
Although the present study is limited by the absence of bonus rule data, the insights gained
from base salary and performance ratings analysis lay the groundwork for future, more
comprehensive compensation reviews.
A deep-dive continuous monitoring strategy is recommended, where periodic EDA updates
and iterative renements can help the organization achieve sustained improvements in
gender equity and pay fairness. The methodologies applied herein can also be adapted to
other datasets or sectors, thereby serving as a model for data-driven human resource
optimization in today’s competitive business environment.
By investing in systematic data collection, rigorous analysis, and proactive policy
adjustments, manufacturing organizations can not only meet regulatory standards but also
build diverse, high-performing teams that drive innovation and long-term success.
