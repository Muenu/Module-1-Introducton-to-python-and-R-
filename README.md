# Module-1-Introducton-to-python-and-R-
Assignment 1_ Highridge Construction Company Payment Slips

##Introduction For this project we will be using both Python and R programming languages to create random payment payslips for Highridge Company Employees. 
The main objective is to gain better understanding of the differences and similarities in both applications how they can be use in data analysis.

### Python & R Programming
1. When working on this project i found that the language and syntax in  python  is easy to use and understand as it is in English language.
2. [image](https://github.com/Muenu/Module-1-Introducton-to-python-and- R-/assets/115622275/da9419bd-87d5-4ef1-8da6-dd2d87d8a906)

### R Programing
1. I found R syntax to be a bit challenging since its my first time to really get to use it

### How to use the codes generated in Python and R code
# Python
Step 1: Import the library
As per the assignment we were not dealing with a given data so we needed to generate random data for us to use.We used import random.

import random

Step 2:  For Loop
We were required to generate random mumbers for the 400 employees as instruted to. For loops enables creation of random numbers contnuously

#Utilize a for loop to generate payment slips for each of the 400 workers.
employees = []
for _ in range(400):
    employee = {
        "name": f"employee{_+1}",
        "gender": random.choice(["Male", "Female"]),
        "salary": random.uniform(5000, 30000)
    }
    employees.append(employee)

    
Step 3:  Implementing conditional statements using if, elif and else statements
If statement _It is used to decide whether a certain statement or  statements will be executed or not.
If-else statement-we can use the else statement with the if statement to execute
a block of code when the if condition is false.
If-Elif-Else Statement- The if statements are executed from the top down.As soon as one of the conditions controlling the if is true, the statement
associated with that if is executed, and the rest of the ladder is bypassed. If none of the conditions is true, then the final “else” statement will 
be executed.(Geeks for geeks)

for employee in employees:
    try:
       
        if 10000 < employee["salary"] < 20000:
            employee["level"] = "A1"
        elif 7500 < employee["salary"] < 30000 and employee["gender"] == "Female":
            employee["level"] = "A5-F"
        else:
            employee["level"] = "Other"

        # Display payment slip
        print(f"Name: {employee['name']}, Salary: ${employee['salary']}, Level: {employee['level']}")
        
 
Step 4: Exception handling helps to handle potential errors_Exceptions are raised when the program is syntactically correct, but the code results in an
error. This error does not stop the execution of the program, however, it changes the normal flow of the program.
(https://www.geeksforgeeks.org/python-exception-handling/?ref=lbp)

#Add exception handling to your Python code to address potential errors.       

    except Exception as e:
        print(f"Error processing {employee['name']}: {str(e)}")

## Challenges:
1.It was really time consuming and working and trying to understand
R as compared to Python. So i had to do some extensive research on the for the R code to run on R as compared to Python.

2. Also Github is new to me but there is quite alot of information on how to create a repository on Github as well as to do a README
file. I still feel with more practice i will be able to create
a good READ me file.


