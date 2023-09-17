# Employee Class

This Java class, `Employee`, represents factory employees and provides methods for calculating their salaries.

## Attributes

- `name`: Employee's name.
- `salary`: Employee's salary.
- `workHours`: Weekly working hours.
- `hireYear`: Year of employment.

## Methods

- `Employee(name, salary, workHours, hireYear)`: Constructor that initializes the employee's attributes.
- `tax()`: Calculates the tax based on the salary.
    - No tax is applied if the salary is less than 1000.
    - If the salary is 1000 or more, 3% of the salary is taxed.
- `bonus()`: Calculates bonus payments based on overtime work.
    - For each hour worked beyond 40 hours in a week, an additional 30 TL is paid.
- `raiseSalary()`: Calculates a salary raise based on years of employment.
    - If the employee has worked for less than 10 years, a 5% raise is applied.
    - For employees with 10 or more years and less than 20 years of experience, a 10% raise is applied.
    - For employees with 20 or more years of experience, a 15% raise is applied.
- `toString()`: Overrides the default `toString()` method to display employee information.

## Example Usage

```java
Employee employee = new Employee("John Doe", 1200, 45, 2005);
employee.raiseSalary(); // Calculate and apply the salary raise
System.out.println(employee); // Display employee information
```
## Author

This class is authored by Serhat Acar.