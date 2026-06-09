# Hierarchical Inheritance in Python

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
```
class Details:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def getName(self):
        return self.name

    def getAge(self):
        return self.age


class Employee(Details):
    def __init__(self, name, age, employee_id, department):
        super().__init__(name, age)
        self.employee_id = employee_id
        self.department = department

    def getEmployeeDetails(self):
        print("\n--- Employee Details ---")
        print("Name:", self.getName())
        print("Age:", self.getAge())
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


class Patient(Details):
    def __init__(self, name, age, patient_id, disease):
        super().__init__(name, age)
        self.patient_id = patient_id
        self.disease = disease

    def getPatientDetails(self):
        print("\n--- Patient Details ---")
        print("Name:", self.getName())
        print("Age:", self.getAge())
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


# Get input for Employee
ename = input("Enter Employee Name: ")
eage = int(input("Enter Employee Age: "))
eid = input("Enter Employee ID: ")
edept = input("Enter Department: ")

# Create Employee object and display details
emp = Employee(ename, eage, eid, edept)
emp.getEmployeeDetails()

# Get input for Patient
pname = input("\nEnter Patient Name: ")
page = int(input("Enter Patient Age: "))
pid = input("Enter Patient ID: ")
pdisease = input("Enter Disease: ")

# Create Patient object and display details
pat = Patient(pname, page, pid, pdisease)
pat.getPatientDetails()

```
## Sample Output
<img width="458" height="666" alt="image" src="https://github.com/user-attachments/assets/3d786b5b-4cbc-4db4-b6dd-9ee981d6d3fa" />

## Result
Thus, it is proved that hierarchical inheritance allows multiple derived classes (Employee and Patient) to inherit common properties and behaviors from a single base class (Details), demonstrating effective code reusability and organization.
