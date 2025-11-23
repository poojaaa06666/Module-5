# Hierarchical Inheritance in Python
        self.__company="<No Company>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,comp,dept):
        self.setData(id,name,gender)
        self.__company=comp
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__company)
        print("Department: ", self.__dept)

class Patient(Details): #Inheritance
    def __init__(self):
        self.__hospital="<No Hospital>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,hos,dept):
        self.setData(id,name,gender)
        self.__hospital=hos
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__hospital)
        print("Department: ", self.__dept)

id=int(input())
name=input()
gender=input()
comp=input()
dept=input()
id1=int(input())
nam=input()
gen=input()
hosp=input()
dep=input()

print("Doctor Object")
e=Employee()
e.setEmployee(id,name,gender,comp,dept)
e.showEmployee()
print("\nPatient Object")
d = Patient()
d.setEmployee(id1, nam, gen, hosp, dep)
d.showEmployee()
```

## Sample Output

![image](https://github.com/user-attachments/assets/45c89888-05d0-4b1f-ad2d-0e74a51cfb21)

## Result

Thus the program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details hase been executed successfully.
