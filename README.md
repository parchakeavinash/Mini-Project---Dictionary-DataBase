# Mini-Project---Dictionary-DataBase
Beginners Python Mini Projects Coding A Simple Data Base. In This Project You Will Learn How To Create Functions, Get user Input, Use The Python Len Function In Combination With The And Operator, Create A Python Dictionary, Update The Dictionary, Clear The Dictionary, Print The Dictionary And Use A For Loop In Python.

print("Mini Project - Dictionary DataBase")

students = {"Avinash": "AI", "Prajwal": "IT", "Mohit": "Ds"}

def intro():
    print("Welcome to the Data Base \n")
    print("To get access enter your password")
    enter_password()

def enter_password():
    password = "123abc"
    entry1 = input("Enter password: ")
    if (len(entry1) < 3 and (entry1 != password)):
        print("Access Denied")
    else:
        print("Access Granted")

        data_base()
def data_base():
    x = int(input("Clear(1), Update(2) , Print(3):  "))

    if x == 1:
        students.clear()
        print(students)
        print("Database cleared!!")
    elif x == 2:
        update_dictionary()
        print("Database Updated!!")
    elif x ==3:
        print(students)
    else:
        print("Invalid choice ")

def update_dictionary():
    name = input("Enter name: ")
    branch = input("Enter branch: ")
    students[name] = branch
    print(students)

intro()
