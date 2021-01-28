# AdventureWorks2019 Employees Analysis

**Files**

AdventureWorks Employees.sql - Main file used for analysis of Employees

AdventureWorks Employees Analysis.pbix - Employees Analysis Dashboard

Employees Dashboard.png - Image of Dashboard

**Introduction**

Hello! Welcome to my project! Here I will be discussing the process on how I did my analysis, what I found, and how I displayed my findings. In this project I used the AdventureWorks2019 database from Microsoft. For this project, I had decided to focus my analysis on the employees from this database. 

**SQL Process**

The goal was to improve from my last project by writing more queries and using multiple tables. Going through the database, I decided to use five tables for my analysis of the employees. The tables that were used were HumanResources.Department, HumanResources.Employee, HumanResources.EmployeeDepartmentHistory, HumanResources.EmployeePayHistory, amd Person.Person. After brainstorming questions for myself that I wanted to find the answers to, I started writing the queries. 

Before beginning my analysis, I had to clean the data so that I would have the relevant columns for analysis. For the Person.Person table, I had replaced the null values in the Title column with 'MISSING' and replaced the null values for the column MiddleName with 'N/A' to make it cleaner. I had to also use the WHERE clause to filter the data so that only the employees from the data would be displayed. I then consolidated HumanResources.Employee table by selecting the relevant columns. Both of these tables output were sent to a new table by using INTO. 

I had used INTO in my previous project as well and I wanted to improve on that by considering query performance and storage space. I used CREATE VIEW to create a virtual table so that it would not take as much storage as a physical table. I had named my first virutal table as [Employees Hired] which contains the employees hired each year, grouped by gender. This was done using CASE, SUM, and COUNT to isolate each year and finding the count for each year. I had also found the count of employees hired each year.

The next virtual table I created documented the Employees that are active. The employees that were working there were NULL values and so I replaced it with 'Employed' using CASE. I had found there were 290 active employees. 

On my next virtual table, I had joined four tables together to get good practice with joining tables. I used MAX in order to get the max hourly pay for each employee since six employees had gone through three different hourly rates which indicates a promotion. I had also filtered it by NULL so that only the active employees will be in the table which is 290. I will also use this virtual table that is named [Employee Pay] to do further analysis. 

By using the [Employee Pay] virtual table, I found the moving average by department, this was more done as practice to help refine using windows function. The more useful analysis was finding how many people are in a certain pay range. I had found that 50 females and 136 males made between $0 - $15 per hour, 24 females and 54 males made between $15.01 - $30 per hour and finally 10 females and 16 males made over $30 per hour. It can be inferred from this that too many employees are paid too low and should be given a pay raise. I had found the average pay for females to be $19.23 and for males to be $17.76. There are 206 males and 84 females that working at this company. The company should look towards hiring for females in the future since the numbers are skewed heavily to male hires. The average pay by department was also found with the Executive having the highest average at $92.80 and the lowest was Shipping and Receiving at $10.87. The second highest average was Research and Development at $43.68. There looks to be an uneven distribution of pay that is heavily skewed towards the top, while at the bottom the pay is either below or at minimum wage. I then went on to do more analysis for fun and practice by find the highest pay and lowest pay by gender, the top ten people with the highest hourly rate and the ten people that were payed the lowest. 

I also wanted to get more practice with joins, so I used INNER JOIN again to connect two tables to find ten people with the most vacation hours and the ten people with the most sick leave hours. I had also found the total vacation and sick leave hours by gender. Then finally, for extra query practice, I found all the employees that work there who were born in 1988 and later, I also had to join two tables here as well. 

**Power BI Process**


**Conclusion**


**Source**

https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms
