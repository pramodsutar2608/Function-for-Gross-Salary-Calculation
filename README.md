# Function-for-Gross-Salary-Calculation

Project Name: Gross Salary Calculator

PL/SQL Gross Salary Calculation Function:

Implemented a PL/SQL stored function (f1) to calculate gross salary based on specified conditions, taking employee number (empno) as a parameter.
Dynamic Component Calculation:

Dynamically computed house rent allowance (hra), dearness allowance (da), and provident fund (pf) based on percentages of the monthly salary (sal) retrieved from the emp1 table.
Gross Salary Formula:

Utilized the formula gross = sal + hra + da - pf to calculate the gross salary, ensuring accurate and consistent results for each employee.
Example Usage:

Demonstrated the functionality of the function by querying the gross salary for a specific employee (e.g., employee number 7902) using the select f1(7902) from dual statement.
