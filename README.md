# Overview  
Create a set of classes and an interface for managing employees at a company.  The payroll system stores employee names, ID numbers, and information for calculating the employees' weekly paycheck.  

# Requirements  
Each time a new employee is hired, an new object of the appropriate employee type is created and added to an ArrayList of ALL employees.  
For SalariedEmployee, the constructor should look like:  
SalariedEmployee(name, ID#, annualSalary)  
example: SalariedEmployee("Arshad Khan", 1234, 50000)  

For HourlyEmployee, the constructor should look like:  
HourlyEmployee(name, ID#, hourlyRate)  
example: HourlyEmployee("Arshad Khan", 1234, 15.75)  

name is a String, the ID# is an int, and all pay rate information will be doubles.  

Each class should have a getName, getID, and getWeeklyPay method.

Weekly pay will be calculated differently for salaried employees and hourly employees.  Salaried employees will calculate their weekly pay by dividing their salary by 52.  For simplicity, we'll assume that the hourly employee work 40 hours each week. 

# Structure  
You will need to create two additional files.  

An interface that describes the methods listed above.  

A parent class that does the tasks that both types of employees 
The parent class will fall between the interface and the other two classes.  The parent class should implement the interface you created.  The other classes will inherit from the parent class

# Demo  
In Demo.main() , create several employees (some of each type) and store them in the same list to demonstrate polymorphism.  
Use the list to calculate the total amount the company will pay to its employees in a week.  

Add another employee and perform the same payroll summary calculation.  It might make sense to create a helper method for the calculating the total weekly payroll amount.  
