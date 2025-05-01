# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
```
#Reg_no: 212223060288
#Name: Tharun Kumaran G

class Details:
    def __init__(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

    def display_details(self):
        print("ID:", self.id)
        print("Name:", self.name)
        print("Gender:", self.gender)

class Employee(Details):
    def __init__(self, id, name, gender, company, department):
        super().__init__(id, name, gender)
        self.company = company
        self.department = department

    def display_details(self):
        super().display_details()
        print("Company:", self.company)
        print("Department:", self.department)

class Doctor(Details):
    def __init__(self, id, name, gender, hospital, department):
        super().__init__(id, name, gender)
        self.hospital = hospital
        self.department = department

    def display_details(self):
        super().display_details()
        print("Hospital:", self.hospital)
        print("Department:", self.department)

print("Enter Employee Details:")
emp_id = input("ID: ")
emp_name = input("Name: ")
emp_gender = input("Gender: ")
emp_company = input("Company: ")
emp_department = input("Department: ")

print("\nEnter Doctor Details:")
doc_id = input("ID: ")
doc_name = input("Name: ")
doc_gender = input("Gender: ")
doc_hospital = input("Hospital: ")
doc_department = input("Department: ")

employee = Employee(emp_id, emp_name, emp_gender, emp_company, emp_department)
doctor = Doctor(doc_id, doc_name, doc_gender, doc_hospital, doc_department)

print("\n--- Employee Details ---")
employee.display_details()

print("\n--- Doctor Details ---")
doctor.display_details()



```

### OUTPUT  

![image](https://github.com/user-attachments/assets/ea1f4391-0011-444e-a3fb-7f59d8e419c2)

### RESULT

Thus, the python program to get the employee and doctor details and display them using hierarchical inheritance has been executed and verified successfully.
