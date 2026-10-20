# Employee-Compensation-and-Salary-Equity-Analysis
Excel • Power Query • HR Analytics • Data Quality • Dashboard

## 📊 Project Overview
This project analyzes employee compensation data to identify salary patterns and examine how compensation varies across gender, department, job role, tenure, and education level.
The project focuses not only on compensation analysis but also on data quality and validation. The original dataset contained duplicates, missing values, inconsistent categories, mixed date formats, compensation calculation discrepancies, and salary-band inconsistencies.
Using Excel and Power Query, I transformed the raw dataset into a validated analytical dataset and developed an Excel dashboard to communicate the findings.
> **Portfolio focus:** Data quality → transformation → analysis →
> visualization → business insights → recommendations
---
## 🎯 Business Objective
The analysis was designed to answer questions such as:
* What does the overall compensation structure look like?
* How does average and median salary vary across departments?
* Which job roles have the highest and lowest average base salaries?
* How does compensation vary with tenure?
* How does compensation vary across education levels?
* Are there observable differences in average compensation between male and female employees?
* What data-quality issues need to be addressed before compensation analysis can be trusted?
The analysis is descriptive and identifies patterns that could be investigated further.

---
## 🗂️ Dataset
Attribute          Details
---
* Original records   5,000
* Cleaned records    4,990
* Variables          15
  
### Primary tools      Excel & Power Query
### Analysis           Excel formulas & PivotTables
### Visualization      Excel charts & dashboard

**Key Variables**
* Employee ID
* Gender
* Age
* Department
* Job Role
* Education Level
* Years at Company
* Years in Role
* Performance Rating
* Employment Type
* Base Salary
* Bonus
* Total Compensation
* Salary Band
* Hire Date

---
### 🧹 Data Preparation & Quality Checks
The raw dataset was audited and transformed using Excel Power Query.
**Key issues identified**
* 10 duplicate Employee ID records:
* Missing department values
* Missing education levels
* Missing and invalid Years in Role values
* Missing bonus values
* Total Compensation calculation mismatches
* Inconsistent employment-type labels
* Mixed Hire Date formats
* Invalid performance-rating values
* Salary-band inconsistencies
* Salary outliers

### Key cleaning actions:

* Duplicates: 10 duplicate Employee ID records were removed, resulting in 4,990 unique employee records.
* Missing values: Missing values were investigated individually. Where reliable source information allowed a value to be resolved, it was corrected. Where no reliable correction was possible, the value was retained as null rather than introducing an unsupported assumption.
* Compensation validation: Total Compensation was validated and recalculated using: `Base Salary + Bonus`
Missing bonus values were resolved where Total Compensation provided sufficient information.
* Salary-band validation: Salary bands were checked against defined salary ranges and inconsistent classifications were corrected.
* Date standardization: Mixed Hire Date formats were converted into a consistent Date format.
* Outlier analysis: Base Salary outliers were identified using the Interquartile Range (IQR) method. Identified outliers were retained where there was insufficient evidence that they represented data-entry errors.
* Final validation: The cleaned dataset contains 4,990 employee records with no Power Query errors.

---
### 📈 Key Findings
Overall Compensation
Metric                          Result
---
* Total employees                  4,990
* Average base salary            €83,201
* Median base salary             €81,900
* Average bonus                   €7,632
* Average total compensation     €90,833
* Median total compensation      €89,100
* Compensation by Department
### Average base salary ranged from:
* Marketing: €79,217
* HR: €80,990
* Operations: €81,443
* Finance: €83,368
* Sales: €85,945
* IT: €87,796
* Sales had the highest median base salary at €89,700.
  
### Compensation by Job Role
Average base salary varied substantially by job role.

### Job Role                  Average Base Salary
---
* Sales Representative                  €63,695
* Marketing Specialist                  €65,351
* HR Specialist                         €69,098
* Operations Specialist                 €69,357
* IT Specialist                         €73,474
* HR Analyst                            €74,371
* Operations Analyst                    €75,707
* Accountant                            €75,798
* Marketing Analyst                     €76,120
* Financial Analyst                     €76,122
* Data Analyst                          €80,142
* Account Manager                       €95,634
* Software Developer                    €92,889
* Marketing Manager                     €97,243
* Sales Manager                         €97,734
* HR Manager                            €98,379
* Operations Manager                    €99,871
* Finance Manager                      €100,556
* IT Manager                           €103,334
* The highest average base salary was observed for IT Managers (€103,334), while the lowest was observed for Sales Representatives (€63,695).
* These differences are descriptive and should not be interpreted as evidence that job role alone causes the observed salary differences.

### Compensation by Tenure
* Tenure           Average Base Salary

* 0--2 years                   €76,758
* 3--5 years                   €79,275
* 6--8 years                   €82,926
* 9--11 years                  €87,351
* 12--14 years                 €88,903
Average base salary increased across the observed tenure groups.

### Compensation by Education
Education Level     Average Base Salary
---
* High School                     €78,375
* Bachelor's                      €81,648
* Master's                        €86,222
* PhD                             €88,654
* The difference between the High School and PhD groups was €10,279.
This is a descriptive association and should not be interpreted as evidence that education level alone determines compensation.

---
## ⚖️ Gender Compensation Analysis
The analysis found:
* Female average base salary: €83,112
* Male average base salary: €83,291
* Observed average difference: approximately €180
* Median difference: €200
* This is an unadjusted descriptive comparison, not an adjusted gender
* pay-gap analysis.
  
The analysis does not control for factors such as:
* Job role
* Tenure
* Education
* Performance
* Employment type
Other potentially relevant employee characteristics

Therefore, the observed difference should not be interpreted as evidence of a particular cause. A logical next step is an adjusted compensation analysis to determine whether differences remain after accounting for relevant workforce characteristics.

---
## 📊 Dashboard
The Excel workbook includes a dashboard covering:
* Total Employees
* Average Base Salary
* Median Base Salary
* Average Total Compensation
* Compensation by Gender
* Compensation by Department
* Compensation by Job Role
* Compensation by Tenure
* Compensation by Education
  
* Key Insights
* Recommendations
* Data Quality & Methodology
* Dashboard Preview

<img width="908" height="458" alt="image" src="https://github.com/user-attachments/assets/97565566-ecaa-43d2-8a65-d1b1b0d7b207" />

------
## 💡 Recommendations

* Investigate Gender Pay Differences at Job-Role Level.
* Review Compensation Differences Across Departments.
* Review Salary Progression and Tenure.
* Investigate Salary Differences Across Education Levels.
* Strengthen Compensation Data Quality and Monitoring .
* Review Job Roles with Unusual Salary Patterns.
---
## 🛠️ Tools & Skills Demonstrated

### Tools

* Microsoft Excel
* Power Query
* PivotTables / PivotCharts
* Excel formulas
* Excel charts
* Dashboard design
* Analytical Skills
* Data auditing
* Data cleaning
* Data validation
* Missing-value assessment
* Duplicate detection
* Outlier analysis
* Compensation analysis
* Descriptive statistics
* Comparative analysis
* Data visualization
* Business recommendations

---
### ⚠️ Limitations

This project is a descriptive compensation analysis. It does not establish causality or determine whether observed
compensation differences are explained by discrimination or any single factor. The dataset does not provide all information required for a comprehensive compensation-equity assessment, such as:

* Detailed job level
* Promotion history
* Performance history over time
* Location
* Relevant professional experience
* Individual salary-band position
* Hiring salary
* Salary increase history
  
The findings should therefore be interpreted as patterns requiring further investigation, rather than definitive explanations of compensation differences.

---
## 🚀 Next Steps

Future development could include:
* Adjusted compensation analysis using relevant employee characteristics.
* Salary-band positioning analysis.
* Promotion and salary progression analysis.
* Time-based compensation analysis if historical salary records become available.

---
## 📁 Repository Structure

```text
Employee-Compensation-Salary-Equity/
│
├── README.md
│
├── data/
│   └── employee_compensation_salary_equity.xlsx
│
├── dashboard/
│   └── employee_compensation_dashboard.xlsx
│
├── presentation/
│   └── executive_summary.pptx
│
├── images/
│   └── dashboard.png
│
└── documentation/
    └── methodology.md
```
## 📌 Project Takeaway

This project demonstrates an end-to-end analytics workflow:

**Raw Data → Data Audit → Power Query Cleaning → Validation → Analysis → Visualization → Business Insights → Recommendations**

The project demonstrates how Excel and Power Query can transform a messy employee dataset into a structured compensation analysis that supports further HR investigation and data-driven decision-making.

---
## Author

**Barbara**

Data Analyst with a passion for transforming data into actionable business insights using SQL, Python, and data visualization tools.

If you found this project interesting or have feedback, feel free to connect or reach out.


