# 🔄 Hackerrank : # 📦 Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---
## NAME : Shanmuga Vasanth M
## REG NO: 212223040191
## 🎯 Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.

---


## 🧪 Program
~~~c
import textwrap
def wrap_string(long_string, width):
    wrapped_text = textwrap.fill(long_string, width)
    return wrapped_text
long_string = input("Enter a long string: ")
width = int(input("Enter the desired width for wrapping: "))

wrapped_string = wrap_string(long_string, width)

print("\nWrapped String:")
print(wrapped_string)
~~~

## Sample Output
![442488320-de47b27c-df7e-4e2d-928c-b35169b3e311](https://github.com/user-attachments/assets/bd931651-7acd-4868-86ba-2ddbac32bacb)

## Result
Thus the program has been executed successfully.

