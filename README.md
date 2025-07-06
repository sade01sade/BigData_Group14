# BigData_Group14
#QUESTION_1

# Function to input student name and grades
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

#OUTPUT


