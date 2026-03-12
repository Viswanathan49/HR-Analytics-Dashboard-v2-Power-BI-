Here’s a complete README you can paste and tweak (replace Vignesh InfoTech / dates if needed).

HR Analytics Dashboard v2 – Power BI (Virtual Internship Week 4)
This repository contains my Week 4 Power BI virtual internship project: an enhanced HR Analytics Dashboard built on an employee dataset. It focuses on clean dark‑theme design, interactive slicers, and key HR KPIs such as headcount, gender distribution, geography, and average salary.

🚀 Project Overview
The dashboard is designed for HR and leadership teams to quickly understand the workforce structure and composition. It allows users to slice the data by department, country, and employee, and explore how headcount and salary metrics change across different segments.

Key questions this report helps answer:

What is our total headcount and gender split?

How is headcount distributed across departments and countries?

How has headcount changed over hire years?

How does headcount vary across age groups?

📊 Dashboard Features
KPI Cards

Total Employees

Total Male Count and Male %

Total Female Count and Female %

Average Salary

Interactive Slicers

Department

Country

Employee Name (with search)

Visuals

Headcount by Department and Gender (clustered bar chart)

Headcount by Gender (donut chart)

Headcount by YoY – headcount by hire year (line chart)

Headcount by Age Group (column chart)

Navigation / Summary using a decomposition tree for Country, City, Business Unit, and Gender

Design

Dark theme with consistent color palette

Clean layout with a left filter panel and central analytics area

Readable typography and spacing suitable for presentations or management reviews

🧾 Dataset
File: Employee-Sample-Data.xlsx

Main columns used:

Employee ID, Full Name

Job Title, Department, Business Unit

Gender, Ethnicity, Age

Hire Date

Annual Salary, Bonus %

Country, City

The dataset represents current employees and is used only for educational and portfolio purposes.

🧮 Key DAX Measures
Some of the core measures used in this report:

text
Total Employees =
COUNTROWS ( 'Employee Data' )

Total Male Count =
CALCULATE (
    [Total Employees],
    'Employee Data'[Gender] = "Male"
)

Total Female Count =
CALCULATE (
    [Total Employees],
    'Employee Data'[Gender] = "Female"
)

Male % =
DIVIDE ( [Total Male Count], [Total Employees] )

Female % =
DIVIDE ( [Total Female Count], [Total Employees] )

Average Salary =
AVERAGEX ( 'Employee Data', 'Employee Data'[Annual Salary] )
(You can add more measures here later if you extend the project.)

🛠️ Tools & Skills
Tool: Microsoft Power BI Desktop

Skills demonstrated:

Data cleaning and modeling

DAX measures for KPIs

Dashboard layout and dark‑theme UI design

Use of slicers, decomposition tree, donut, bar, line, and column charts

Storytelling with HR analytics

📂 Project Structure
Employee-Sample-Data.xlsx – source dataset

HR_Analytics_Dashboard.pbix – Power BI report file (add when uploaded)

screenshots/ – exported dashboard images for quick preview

README.md – project documentation

✅ How to Use
Clone this repository.

Open HR_Analytics_Dashboard.pbix in Power BI Desktop.

If needed, update the file path for Employee-Sample-Data.xlsx.

Interact with slicers and visuals to explore the HR metrics.

🔗 Related Work
This is the Week 4 version of my HR analytics project.
You can also see my earlier Week 3 HR Analytics Dashboard here:

HR Analytics Dashboard – Week 3

📣 Feedback
I’m actively improving my Power BI and data analytics skills.
If you have suggestions on design, KPIs, or DAX, feel free to open an issue or reach out!
Contact : viswanathansk49@gmail.com
