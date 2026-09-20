# Hierarchical Inheritance in Python
## NAME: JANARTHANI R
## REF NO: 25017541
This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
class Details:

    def __init__(self):
    
        self.name = input("Enter name: ")
        
        self.age = int(input("Enter age: "))

    def getName(self):
    
        print("Name :", self.name)

    def getAge(self):
    
        print("Age :", self.age)

class Employee(Details):

    def __init__(self):
    
        super().__init__()
        
        self.employee_id = input("Enter employee ID: ")
        
        self.department = input("Enter department: ")

    def getEmployeeDetails(self):
    
        print("\n--- Employee Details ---")
        
        self.getName()
        
        self.getAge()
        
        print("Employee ID :", self.employee_id)
        
        print("Department :", self.department)

class Patient(Details):

    def __init__(self):
    
        super().__init__()
        
        self.patient_id = input("Enter patient ID: ")
        
        self.disease = input("Enter disease: ")

    def getPatientDetails(self):
    
        print("\n--- Pa

## Sample Output
Enter Employee Information

Enter name: Rahul

Enter age: 30

Enter employee ID: E101

Enter department: HR

Name : Rahul

Age : 30

Employee ID : E101

Department : HR

Enter Patient Information

Enter name: Anitha

Enter age: 25

Enter patient ID: P205

Enter disease: Fever


Name : Anitha

Age : 25

Patient ID : P205

Disease : Fever
## Result
Thus, a Python program demonstrating Hierarchical Inheritance using a base class Details and derived classes Employee and Patient was successfully written and executed.
