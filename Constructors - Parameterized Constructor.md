# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
To write a Python code to create a class for a person with a parameterized constructor, which will take the `name` and `userid` of the person as parameters and print the `userid` of the person.

---

### ALGORITHM

1. Begin the program.  
2. Define a `person` class.  
3. The `person` class should have a parameterized `__init__` method that accepts two parameters: `name` and `userid`.  
4. Inside the `__init__` method, assign the `name` to `self.name` and the `userid` to `self.userid`.  
5. Print the `self.userid`.  
6. Prompt the user to enter their `name` (string) and `userid`.  
7. Create an instance `s1` of the `person` class by passing the entered `name` and `userid` to the constructor.  
8. Terminate the program.

---

### PROGRAM

```
#Reg_no: 212223060288
#Name: Tharun Kumaran G

class Person:
    def __init__(self, name, userid):
        self.name = name
        self.userid = userid
        print("User ID:", self.userid)

name_input = input("Enter your name: ")
userid_input = input("Enter your userid: ")

s1 = Person(name_input, userid_input)

```

### OUTPUT

![image](https://github.com/user-attachments/assets/ba742b91-fa2f-4908-a0a3-728b1c498c05)

### RESULT

Thus, the python code to create a class for a person with a parameterized constructor has been executed and verified successfully.
