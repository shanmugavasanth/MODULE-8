# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---
## NAME : Shanmuga Vasanth M
## REG NO: 212223040191

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻 PROGRAM:
~~~c
students_marks = {
    'Alice': [85, 92, 78, 88, 91],
    'Bob': [72, 65, 80, 79, 69],
    'Charlie': [95, 99, 92, 97, 94],
    'David': [60, 70, 72, 65, 68]
}
total_marks = {}

for student, marks in students_marks.items():
    total_marks[student] = sum(marks)
topper = max(total_marks, key=total_marks.get)
print("Total Marks:")
for student, total in total_marks.items():
    print(f"{student}: {total}")
print("\nTopper:", topper)
print("Topper's Total Marks:", total_marks[topper])
~~~

## OUTPUT
![442488019-61d4ea50-e831-4806-8d2f-89e779576330](https://github.com/user-attachments/assets/4d12d3ac-2832-46a6-8d64-c8a9a78762fa)


## RESULT
Thus the program has been executed successfully.
