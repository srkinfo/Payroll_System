Quick README for the Payroll System
Overview:
This Java program simulates an employee payroll system where different types of employees can be added, and their payroll can be processed. Employees can be categorized as Full-Time, Part-Time, or Contract employees, each with different salary calculation methods.

Classes Overview:
Main (Payroll System):

Manages the overall payroll system.

Allows adding employees, displaying employee details, and processing payroll.

Employee (Abstract Class):

Common base class for all employee types.

Contains properties like name, emp_id, and baseSalary.

Defines an abstract method calculate_salary() for calculating an employee's salary.

FulltimeEmployee (Subclass of Employee):

Represents full-time employees.

Inherits from Employee and adds properties for bonus and tax deduction.

Salary is calculated as: baseSalary + bonus - taxDeduction.

Parttime_emp (Subclass of Employee):

Represents part-time employees.

Inherits from Employee and adds properties for hoursWorked and hourlyRate.

Salary is calculated as: hoursWorked * hourlyRate.

contract_Emp (Subclass of Employee):

Represents contract employees.

Inherits from Employee and adds property for contractAmount.

Salary is simply the contractAmount.

Functionality:
Add Employee:

Users can choose the type of employee (Full-Time, Part-Time, Contract) and enter relevant details (e.g., name, ID, salary-related details).

Display Employees:

Displays a list of all employees with their details such as name, ID, and base salary.

Process Payroll:

Computes and displays the salary for each employee based on their type.

Exit:

Exits the payroll system.

Example Usage:
Add Employee:

The system will prompt to choose an employee type and input details. For example:

For a Full-Time Employee, the system asks for base salary, bonus, and tax deduction.

For a Part-Time Employee, the system asks for hours worked and hourly rate.

For a Contract Employee, the system asks for the contract amount.

Display Employees:

Displays the list of employees with their ID, name, and base salary.

Process Payroll:

The payroll system will calculate the salary for each employee based on their details.

Example Output:
mathematica
Copy
Edit
=== Employee Payroll System ===
1. Add Employee
2. Display Employees
3. Process Payroll
4. Exit
Enter Choice: 1

Choose Employee Type:
1. Full Time Employee
2. Part Time Employee
3. Contract Employee
Enter Choice: 1
Enter Employee Name: John Doe
Enter Employee id: 101
Enter base salary: 50000
Enter Bonus: 5000
Enter Tax deduction: 2000
Employee Added Successfully!

=== Employee Payroll System ===
1. Add Employee
2. Display Employees
3. Process Payroll
4. Exit
Enter Choice: 3

Processing Payroll...
Salary for John Doe (ID: 101) -> Rs 53000.0
Output Example (for compiled classes):
mathematica
Copy
Edit
=== Employee Payroll System ===
1. Add Employee
2. Display Employees
3. Process Payroll
4. Exit
Enter Choice: 1

Choose Employee Type:
1. Full Time Employee
2. Part Time Employee
3. Contract Employee
Enter Choice: 2
Enter Employee Name: Jane Smith
Enter Employee id: 102
Enter hoursworked: 30
Enter hourslyRate: 20
Employee Added Successfully!

=== Employee Payroll System ===
1. Add Employee
2. Display Employees
3. Process Payroll
4. Exit
Enter Choice: 2

Employee Details:
ID :102 Name :Jane Smith Salary :0.0

=== Employee Payroll System ===
1. Add Employee
2. Display Employees
3. Process Payroll
4. Exit
Enter Choice: 3

Processing Payroll...
Salary for Jane Smith (ID: 102) -> Rs 600.0
