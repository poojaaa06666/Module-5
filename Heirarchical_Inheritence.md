# Hierarchical Inheritance in Python
5. Display collected information using class methods.

## Program
Add code here
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
        print("Employee Information:")
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
        print("Patient Information:")
        print("Name:", self.getName())
        print("Age:", self.getAge())
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)

emp_name = input()
emp_age = int(input())
emp_id = input()
emp_dept = input()
employee = Employee(emp_name, emp_age, emp_id, emp_dept)
pat_name = input()
pat_age = int(input())
pat_id = input()
pat_disease = input()
patient = Patient(pat_name, pat_age, pat_id, pat_disease)
employee.getEmployeeDetails()
patient.getPatientDetails()
```
## Sample Output
<img width="518" height="399" alt="image" src="https://github.com/user-attachments/assets/df66e98d-f9e4-4162-8065-8e5e156dc7bd" />

