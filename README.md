1. Project Overview
This project analyses a workforce dataset of 500 employees using Excel. The workbook is organised into employee, department, and performance data, with PivotTables, PivotCharts, KPI cards, and slicer-based reporting elements.

The dashboard is designed to give an HR or business user a quick view of workforce composition and provide ways to explore the data by relevant categories.
2. Dashboard KPIs
The KPI cards shown on the dashboard display:
KPI	Dataset result
Total Employees	500
Active Employees	237
Inactive Employees	263
Average Salary	77,751.25
Average Performance Rating	2.984
Average Age	41.678 (displayed rounded as 41 in the dashboard)


These figures are calculated from the complete source dataset. The average age card in the supplied dashboard displays 41; the underlying dataset average is approximately 41.68.
3. Dataset Overview
The workbook contains three source-data sheets:
Sheet	Records	Purpose
Employees	500	Employee demographics, job, salary, joining date, city and status
Departments	5	Department names and manager mapping
Performance	500	Review year, performance rating, training hours and completed projects


The EmployeeID field connects employee records with performance records. DepartmentID connects employee records with the department lookup.
Employees fields
EmployeeID, FirstName, LastName, Gender, Age, DepartmentID, JobTitle, Joining Date, Salary, City, Email, Status, plus department, joining-year and manager lookup fields.
Departments fields
DepartmentID, DepartmentName, Manager.
Performance fields
EmployeeID, ReviewYear, Rating, TrainingHours, ProjectsCompleted.
4. Key Findings from the Dataset
Employee distribution by department
Department	Employees
Sales	119
Finance	108
HR	107
IT	83
Marketing	83
Total	500


Other workforce insights
- Active employees: 237 (47.4%).
- Inactive employees: 263 (52.6%).
- Gender distribution: 251 Male and 249 Female.
- Employees are represented across five cities: Pune (108), Bengaluru (106), Delhi (98), Mumbai (98), and Kolkata (90).
- Average salary: 77,751.25 (in the dataset's salary units).
- Average age: 41.678 years.
- Average performance rating: 2.984 out of 5.
- Total training hours recorded: 15,239.
- Total completed projects recorded: 2,960.
- Joining dates span 2018–2024.
5. Analysis Questions
This dashboard and dataset can help explore questions such as:
1. What is the total employee headcount?
2. How many employees are active versus inactive?
3. Which department has the highest employee count?
4. What is the average salary and age of employees?
5. How does the average performance rating look across the workforce?
6. How are employees distributed by gender and city?
7. How many employees joined in each year?
8. How do training hours and completed projects vary across employees?
6. Excel Features Used
Feature	How it is used
Excel Tables	Structure the Employees, Departments and Performance source data
PivotTables	Summarise headcount and workforce metrics
PivotCharts	Visualise PivotTable summaries
Slicers	Filter compatible PivotTables interactively
Excel formulas	Calculate or retrieve KPI/helper values
Lookup fields	Relate employee records to department and manager information


7. Workbook Sheet Guide
Sheet	Purpose
DASHBOARD	Main dashboard presentation and KPI cards
PIVOT TABLE 1	Workforce summaries and chart support
PIVOT TABLE 2	Salary, rating, employee and other PivotTable summaries
Employees	Employee source data (tblemployees)
Departments	Department lookup data (tbldepartment)
Performance	Performance source data (tblperformance)


8. How to Use
1. Download HR_Analytics_Dashboard.xlsx.
2. Open it using the desktop version of Microsoft Excel.
3. Open the DASHBOARD sheet.
4. Use the available slicers to explore the report.
5. To update after adding records, add rows to the appropriate Excel Tables and select Data → Refresh All.
6. If a KPI or chart does not respond to a slicer, check Slicer → Report Connections and ensure the slicer is connected to the PivotTable that supplies that visual.
Important note about interactivity
A slicer only controls PivotTables that share a compatible PivotCache or Data Model connection. For the six KPI cards to respond to filters, each KPI must be linked to a helper cell or PivotTable result that is also connected to the relevant slicers. Verify this behaviour in Excel before describing every KPI as fully slicer-driven.
9. Data Quality and Privacy Notes
- The headline figures in this README are calculated from the complete 500-row source dataset, not from a currently filtered PivotTable view.
- Some PivotTables in the workbook may retain a prior filter selection. Choose (All) or clear report filters and refresh before comparing every PivotTable with the full-dataset totals.
- The workbook contains employee names and email fields. Confirm the data is synthetic or obtain permission and anonymise personal/confidential information before publishing the workbook publicly.
- The salary unit/currency is not specified in the source data, so this README reports salary values without adding a currency symbol.
- Excel PivotTables, slicers, charts and dashboard objects are best experienced in desktop Microsoft Excel.
10. Future Enhancements
- Add department-wise average salary and rating comparisons.
- Add hiring trend and employee tenure analysis.
- Add training-hours and completed-project analysis.
- Connect all six KPI cards to slicer-aware helper cells.
- Add a clear refresh and data-update process.
11. Skills Demonstrated
Data cleaning and structuring • Excel Tables • PivotTables • PivotCharts • Slicers • KPI reporting • HR analytics • Data interpretation • Dashboard design
