# 👥$${\color{red}GROUP\14\Members:\red.}$$

 1. RUTARO NGABONZIZA Didace 26591


 2.Akariza Gasana Leslie    27413  


 3. Iteka Laure Gabriella   22718


 4.SADE George Sade         26915


 5.MURUNGI DEBORAH           26020

## Instructor: Dr. Eric Maniraguha Institution: Adventist University of Central Africa Course Name: Introduction to Big Data Analytics Course Code: INSY 8413. Date: 6th, July,2025.

# 🧠 Python Work – Big Data Analytics (INSY 8413)
This project contains two questions we did as group14 which are Qn1 and Qn2.

## ❓ Question I: CREATE STUDENT MANAGEMENT SYSTEM FUNCTION

### ✅ Requirements:
* inputs student information
* calculates the average of the marks
* stores and displays the student's information along with their average grade
* uses separate functions for each operation

### 🧾 Solution (Python):
```python # Function to input student name and grades
def input_student_data():
    name = input("Enter the student's name: ")
    num_courses = int(input("Enter number of courses (2 or 3): "))
    grades = []

    for i in range(num_courses):
        grade = float(input(f"Enter grade for course {i + 1}: "))
        grades.append(grade)

    return name, grades

# Function to calculate average
def calculate_average(grades):
    return sum(grades) / len(grades)

# Function to determine letter grade
def get_letter_grade(average):
    if average >= 90:
        return "A"
    elif average >= 80:
        return "B"
    elif average >= 70:
        return "C"
    elif average >= 60:
        return "D"
    else:
        return "F"

# Function to display student info
def display_student_result(name, grades, average, letter):
    print("\n--- Student Report ---")
    print(f"Name: {name}")
    print(f"Grades: {grades}")
    print(f"Average Grade: {average:.2f}")
    print(f"Letter Grade: {letter}")

# Main function to run everything
def student_management_system():
    name, grades = input_student_data()
    average = calculate_average(grades)
    letter_grade = get_letter_grade(average)
    display_student_result(name, grades, average, letter_grade)

# Run the function
student_management_system()
```



### ✨OUTPUT
![question_1](https://github.com/user-attachments/assets/fe9321e5-cd12-400b-8145-bcf42b107e9e)


## ❓ Question II: Palindrome Checker

### Description:
Write a function that asks the user to input a string and checks if the string is a palindrome (reads the same forwards and backwards).Print "Yes,it is a palindrone" or "No, it is not a palindrone"

### ✅ Requirements:
* Use input() to get user input.
* Use a function to perform the task.
  
### 🧾 Solution (Python):
```python def check_palindrome():
    text = input("\nEnter a string to check if it's a palindrome: ")
    clean_text = text.replace(" ", "").lower()
    if clean_text == clean_text[::-1]:
        print("Yes, it is a palindrome")
    else:
        print("No, it is not a palindrome")

check_palindrome()
```
    

### ✨OUTPUT
![Question_2](https://github.com/user-attachments/assets/c00b4358-2072-487b-a5ee-8aa2086c3d65)




