## Name : MOPURI ANKITHA
## Register Number: 212223040117
# Installing Python & Running Programs
<img width="548" height="238" alt="image" src="https://github.com/user-attachments/assets/878aee53-74e7-4a6d-ba61-4a6d3e5948c4" />

<img width="1492" height="747" alt="ss1" src="https://github.com/user-attachments/assets/4a273f8a-c91b-4a8f-9361-fbd7e08bfc8d" />

<img width="615" height="237" alt="image" src="https://github.com/user-attachments/assets/dbf761f4-86ef-4607-8cfa-efcc10d7e9dd" />

<img width="1919" height="959" alt="image" src="https://github.com/user-attachments/assets/73ca3be6-095a-44c6-b916-891d6b0079f8" />

<img width="478" height="207" alt="image" src="https://github.com/user-attachments/assets/e72d5eee-034c-43af-8346-f7ad41dea461" />


### verified intellisense
<img width="997" height="547" alt="image" src="https://github.com/user-attachments/assets/5c14e4c5-569d-4190-97c4-a06c7df22b62" />

### program output
<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/c3b77ede-8f5e-4265-86fe-51f9a3662d3e" />

## Data types
<img width="883" height="353" alt="image" src="https://github.com/user-attachments/assets/a4a1f6dc-9d57-4da0-b16f-f838f525dd96" />

```
def calculate_net_salary(salary, tax_rate):
    if salary < 0 or tax_rate < 0 or tax_rate > 1:
        return "Invalid salary or tax rate"

    tax = salary * tax_rate
    net_salary = salary - tax
    return net_salary

salary = 75000.5
tax_rate = 0.18

result = calculate_net_salary(salary, tax_rate)

if isinstance(result, str):
    print(result)
else:
    print(f"Net Salary: {result:.2f}")
```
<img width="1919" height="1079" alt="salary" src="https://github.com/user-attachments/assets/59fa8e2a-3f51-4152-b31a-f05324071ed2" />

## 5.variables
<img width="914" height="238" alt="image" src="https://github.com/user-attachments/assets/b9f85189-d0fb-4e13-818a-67a7493eacec" />

```
def display_coordinates(x, y):
    if not isinstance(x, (int, float)) or not isinstance(y, (int, float)):
        print("Invalid coordinates")
        return

    print(f"X Coordinate: {x}")
    print(f"Y Coordinate: {y}")

# Multiple assignment
x, y = 10, 20

display_coordinates(x, y)
```
<img width="1919" height="1073" alt="variables" src="https://github.com/user-attachments/assets/98851d61-74cb-4aac-863f-683b10372bc0" />

## Mathematical Operations
<img width="815" height="250" alt="image" src="https://github.com/user-attachments/assets/f9394e4a-2b4a-4c5c-8932-092c89135b35" />

```
def check_even_odd(number):
    if not isinstance(number, int):
        print("Invalid number")
        return

    remainder = number % 2

    if remainder == 0:
        print("Even")
    else:
        print("Odd")

number = 17

check_even_odd(number)
```
<img width="1919" height="1079" alt="modulo" src="https://github.com/user-attachments/assets/39de7181-a104-423a-8878-4ca10c7cc613" />

## 7.Floor Division
<img width="973" height="273" alt="image" src="https://github.com/user-attachments/assets/2e2c9385-fbd2-4906-a14b-99950b348e23" />

```
def calculate_share(total_bill, people):
    if total_bill < 0 or people <= 0:
        print("Invalid bill amount or number of people")
        return

    share = total_bill // people
    print(f"Individual Share: {share}")

total_bill = 1250
people = 4

calculate_share(total_bill, people)
```
<img width="1919" height="1079" alt="floor" src="https://github.com/user-attachments/assets/a6044b8d-8811-412f-8d10-26549b5ed289" />


<img width="1075" height="278" alt="image" src="https://github.com/user-attachments/assets/8af20165-15b2-4e24-8215-f1042b5cb9bb" />


```
def find_salary_range(salaries):
    if not salaries:
        print("Salary list is empty")
        return

    lowest_salary = min(salaries)
    highest_salary = max(salaries)

    print(f"Lowest Salary : {lowest_salary}")
    print(f"Highest Salary: {highest_salary}")

salaries = [50000, 75000, 62000, 95000]

find_salary_range(salaries)
```
<img width="1919" height="1079" alt="minmax" src="https://github.com/user-attachments/assets/2c2c4dfe-154f-473b-9642-39745aac6c83" />

## User Input

<img width="832" height="527" alt="image" src="https://github.com/user-attachments/assets/e694926d-c8a7-495f-a72c-df178209c65c" />

```
def greet_user():
    name = input("Enter your name: ")

    if name.strip() == "":
        print("Name cannot be empty")
        return

    print(f"Hello, {name}!")

greet_user()
```
<img width="1919" height="1079" alt="basicinput" src="https://github.com/user-attachments/assets/09f0e07d-5e90-42f3-81af-540cb0ec7d7c" />


<img width="828" height="276" alt="image" src="https://github.com/user-attachments/assets/e7be9f84-f352-44da-88c6-09d8a6e61557" />

```
def get_age():
    age = input("Enter your age: ")

    if not age.isdigit():
        print("Invalid age")
        return

    age = int(age)
    print(f"Next year you'll be {age + 1}")

get_age()
```
<img width="1919" height="1075" alt="numericinput" src="https://github.com/user-attachments/assets/4af82e43-8f84-409e-a600-0e01a5786445" />

<img width="827" height="236" alt="image" src="https://github.com/user-attachments/assets/447287d8-6899-4326-a4e3-2e9265eaf0f9" />

```
def convert_weight():
    weight = input("Enter weight in kilograms: ")

    try:
        kg = float(weight)

        if kg <= 0:
            print("Invalid weight")
            return

        lbs = kg * 2.20462
        print(f"Weight in pounds: {lbs:.2f}")

    except ValueError:
        print("Invalid input. Please enter a decimal number.")

convert_weight()
```
<img width="1919" height="1075" alt="floatinput" src="https://github.com/user-attachments/assets/2f0768ba-8386-4c5e-8611-7433426211d2" />

## Control flow
<img width="771" height="230" alt="image" src="https://github.com/user-attachments/assets/036314bf-9870-4062-a298-5645cdc0e77f" />

```
def check_pass_fail(marks):
    if marks < 0 or marks > 100:
        print("Invalid marks")
        return

    if marks >= 40:
        print("Pass")
    else:
        print("Fail")

marks = 75

check_pass_fail(marks)
```

<img width="1919" height="1077" alt="simpleif" src="https://github.com/user-attachments/assets/7e1b8b1f-2097-425d-bb80-f4d6e35fce5b" />



<img width="849" height="232" alt="image" src="https://github.com/user-attachments/assets/639af407-624f-4e1c-9c23-dc34a2b6638a" />

```
def check_even_odd(num):
    if not isinstance(num, int):
        print("Invalid input")
        return

    if num % 2 == 0:
        print("Even")
    else:
        print("Odd")

num = 8

check_even_odd(num)
```

<img width="1919" height="1078" alt="ifelse py" src="https://github.com/user-attachments/assets/9faa5955-533a-414e-99da-ecfe7870ab2f" />


<img width="969" height="570" alt="image" src="https://github.com/user-attachments/assets/f1811e76-a2f3-41b4-8028-4be8e4c65957" />

```
def assign_grade(score):
    if score < 0 or score > 100:
        print("Invalid score")
        return

    if score >= 80:
        grade = "A"
    elif score >= 60:
        grade = "B"
    else:
        grade = "C"

    print(f"Score : {score}")
    print(f"Grade : {grade}")

score = 88

assign_grade(score)
```

<img width="1919" height="1079" alt="ifelifelse" src="https://github.com/user-attachments/assets/56c7a7e0-94c7-44db-8776-86be8efe27d5" />


<img width="882" height="284" alt="image" src="https://github.com/user-attachments/assets/9abbdb4d-a531-4016-8903-600fc5884827" />

```
def validate_login(user, pwd):
    if user == "" or pwd == "":
        print("Username or password cannot be blank")
        return

    if user == "admin":
        if pwd == "pass123":
            print("Login Successful")
        else:
            print("Incorrect Password")
    else:
        print("Invalid Username")

user = "admin"
pwd = "pass123"

validate_login(user, pwd)
```

<img width="1919" height="1079" alt="nestedif py" src="https://github.com/user-attachments/assets/804bc5f9-d1e2-4676-a5a0-2af4153bc87a" />


<img width="903" height="259" alt="image" src="https://github.com/user-attachments/assets/39027556-dbd4-40e2-a862-a737d542f070" />

```
def print_numbers(count):
    if count <= 0:
        print("Invalid loop count")
        return

    for i in range(5):
        print(i + 1)

count = 5

print_numbers(count)
```

<img width="1919" height="1079" alt="forloop" src="https://github.com/user-attachments/assets/b35b7c24-e6bb-42e2-a30e-068d9d891626" />


<img width="882" height="263" alt="image" src="https://github.com/user-attachments/assets/8e0324bf-3676-4c04-ba17-431346eabdbe" />

```
def countdown(count):
    if count <= 0:
        print("Invalid count value")
        return

    while count > 0:
        print(count)
        count -= 1

count = 5

countdown(count)
```

<img width="1917" height="1073" alt="whileloop" src="https://github.com/user-attachments/assets/e827f5d5-f218-4e2b-a56a-16e3e1147038" />


<img width="885" height="289" alt="image" src="https://github.com/user-attachments/assets/648c5939-c1f1-44cf-9f2f-5ba41768b765" />

```
def find_first_even(range_size):
    if range_size <= 0:
        print("Invalid range size")
        return

    for i in range(1, range_size + 1):
        if i % 2 == 0:
            print(f"First even number: {i}")
            break

range_size = 10

find_first_even(range_size)
```
<img width="1919" height="1077" alt="break" src="https://github.com/user-attachments/assets/63cf8972-0627-4919-a186-0a8467e71aeb" />



<img width="872" height="588" alt="image" src="https://github.com/user-attachments/assets/df26019c-10f0-4ce1-b735-f5fe59754595" />

```
def sum_odd_numbers(limit):
    if limit <= 0:
        print("Invalid range")
        return

    total = 0

    for i in range(10):
        if i % 2 == 0:
            continue

        total += i

    print(f"Sum of odd numbers: {total}")

sum_odd_numbers(10)
```

<img width="1919" height="1079" alt="continue" src="https://github.com/user-attachments/assets/70165c9e-cf1c-42a9-a746-3eba8e5e2473" />


<img width="893" height="268" alt="image" src="https://github.com/user-attachments/assets/fb3f6bc3-0e54-4b6b-85db-bfac50f0b189" />

```
def my_function():
    pass

my_function()

print("Function defined")
```


<img width="1919" height="1076" alt="pass" src="https://github.com/user-attachments/assets/fe87d9ec-fbb2-41b6-945a-a05c2a6fdfad" />


## WhiteSpace Importance

<img width="808" height="285" alt="image" src="https://github.com/user-attachments/assets/31bdf6b9-62c1-4be3-bdf0-e0a67aa96ecd" />

```
def check_conditions():
    condition1 = True
    condition2 = True

    if condition1:
        if condition2:
            print("Nested")

    print("Confirmation message")

check_conditions()
```

<img width="1919" height="1079" alt="intendation" src="https://github.com/user-attachments/assets/06c3fd48-551c-4395-83e4-1097de75e71a" />


## Organizing Programs

<img width="830" height="271" alt="image" src="https://github.com/user-attachments/assets/c9e33767-a0f5-4a86-89ac-39dbfd3cd918" />

```
def calculate_total_salary():
    # Define the base salary
    base_salary = 50000

    # Define the bonus amount
    bonus = 10000

    # Calculate the total salary
    total_salary = base_salary + bonus

    # Display the total salary
    print(f"Total Salary: {total_salary}")

calculate_total_salary()
```
<img width="1919" height="1079" alt="comment" src="https://github.com/user-attachments/assets/630e9934-079e-463a-8be7-63696b268569" />

## Modules

<img width="938" height="541" alt="image" src="https://github.com/user-attachments/assets/ad7d5def-390e-43da-860f-408e36c830ba" />


```
import math

def calculate_area(radius):
    if radius <= 0:
        print("Invalid radius")
        return

    area = math.pi * radius ** 2
    print(f"Area of Circle: {area:.2f}")

radius = 5

calculate_area(radius)
```

<img width="1919" height="1079" alt="module" src="https://github.com/user-attachments/assets/17d36c93-3970-4e0c-8bd2-579405b86ca8" />


<img width="887" height="290" alt="image" src="https://github.com/user-attachments/assets/53394dd4-a0bf-41ca-a881-5286f29c9558" />

```
from math import *

def math_operations(number):
    if number < 0:
        print("Invalid input")
        return

    print(f"Square Root: {sqrt(number):.2f}")
    print(f"Power (number²): {pow(number, 2):.2f}")
    print(f"Value of Pi: {pi:.2f}")

number = 16

math_operations(number)
```

<img width="1917" height="1079" alt="import" src="https://github.com/user-attachments/assets/65667359-e4af-47e1-9dd4-ca3341ecd959" />


## Functions

<img width="848" height="256" alt="image" src="https://github.com/user-attachments/assets/b529c57f-ed14-400e-86bb-fc3bf1d31d7e" />


```
def add(a, b):
    if not isinstance(a, (int, float)) or not isinstance(b, (int, float)):
        print("Invalid input")
        return None

    return a + b

result = add(5, 3)

if result is not None:
    print(f"Sum: {result}")
```

<img width="1919" height="1079" alt="parameters" src="https://github.com/user-attachments/assets/ae90f409-4dbf-48f1-ba21-47141bf27dd8" />


<img width="889" height="264" alt="image" src="https://github.com/user-attachments/assets/dc2c28e8-33f4-4b36-b11a-e7b3785c91c4" />

```
def area(length, width):
    if length <= 0 or width <= 0:
        print("Invalid dimensions")
        return None

    return length * width

result = area(5, 3)

if result is not None:
    print(f"Area: {result}")
```


<img width="1919" height="1079" alt="multiple py" src="https://github.com/user-attachments/assets/c49a47e2-7384-4d13-84a1-868aeac26562" />



# Built-in Functions

<img width="812" height="298" alt="image" src="https://github.com/user-attachments/assets/1c0f83d0-59ba-4720-9c13-013fa1189ebb" />


```
def string_length(text):
    if text.strip() == "":
        print("Invalid string")
        return

    print(f"Length: {len(text)}")

text = "Hello World"

string_length(text)
```

<img width="1919" height="1079" alt="len" src="https://github.com/user-attachments/assets/0a373235-dad6-4e62-b6c4-c3eac3ee87c9" />


## File I/O

<img width="802" height="254" alt="image" src="https://github.com/user-attachments/assets/d7330fcf-add9-4f03-bf6e-2d63b08e519b" />


```
def write_greeting():
    with open("greeting.txt", "w") as file:
        file.write("Hello World")

    print("Message written to file successfully")

write_greeting()
```

<img width="1919" height="1079" alt="wtofile" src="https://github.com/user-attachments/assets/e4696890-b8c0-4e86-a495-ae8c154c5f73" />


<img width="815" height="275" alt="image" src="https://github.com/user-attachments/assets/86e2afd4-5cab-4582-9165-d6046daca37a" />

```
def read_file():
    try:
        with open("greeting.txt", "r") as file:
            content = file.read()
            print("File Content:")
            print(content)

    except FileNotFoundError:
        print("File not found")

read_file()
```

<img width="1919" height="1079" alt="rff" src="https://github.com/user-attachments/assets/492b92ce-297b-4fde-a185-428fec72f474" />


