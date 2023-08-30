# lab_03_assignment
first commit
## A new line added inside vs code...
class Employee:
def __init__(self, emp_id, name, age, salary):
self.emp_id = emp_id
self.name = name
self.age = age
self.salary = salary
class EmployeeDatabase:
def __init__(self):
self.employees = []
def add_employee(self, emp):
self.employees.append(emp)
def search_by_age(self, age):
result = []
for emp in self.employees:
if emp.age == age:
result.append(emp)
return result
def search_by_name(self, name):
result = []
for emp in self.employees:
if emp.name == name:
result.append(emp)
return result
def search_by_salary(self, operator, amount):
result = []
for emp in self.employees:
if operator == ">" and emp.salary > amount:
result.append(emp)
elif operator == "<" and emp.salary < amount:
result.append(emp)
elif operator == ">=" and emp.salary >= amount:
result.append(emp)
elif operator == "<=" and emp.salary <= amount:
result.append(emp)
return result
def main():
database = EmployeeDataba