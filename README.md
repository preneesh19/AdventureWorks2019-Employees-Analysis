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

**Power BI Process**


**Conclusion**


**Source**

https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms
