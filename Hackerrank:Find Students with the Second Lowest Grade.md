# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---
## NAME : Shanmuga Vasanth M
## REG NO: 212223040191
## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program
~~~c
def second_lowest_grade(students_grades):
    grades = sorted(set(grade for name, grade in students_grades))
    second_lowest = grades[1]
    second_lowest_students = sorted([name for name, grade in students_grades if grade == second_lowest])

    return second_lowest_students
n = int(input("Enter the number of students: "))
students_grades = []
for _ in range(n):
    name = input("Enter student name: ")
    grade = float(input(f"Enter grade for {name}: "))
    students_grades.append((name, grade))
result = second_lowest_grade(students_grades)
print("\nStudents with the second lowest grade:")
for student in result:
    print(student)
~~~

## Output
![442488671-730f350c-d9a8-43bc-a9ed-fc31a066fdd0](https://github.com/user-attachments/assets/021a3fd3-9832-41e6-9df5-e17c62218795)


## Result
Thus the program has been executed successfully.


