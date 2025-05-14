# 🏆 Hackerrank:Runner-Up Score Finder in Python
## NAME : Shanmuga Vasanth M
## REG NO: 212223040191
## 🎯 AIM:
To write a Python program that takes a list of scores from participants and finds the **runner-up score** (i.e., the second-highest score), eliminating any duplicates.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a variable `n` and get its value from the user (number of participants)
3. Read the list of `n` scores from the user using `input().split()` and convert them to integers
4. Store the scores in a list
5. Use `set()` to remove any duplicate scores
6. Convert the set back to a list and sort it in ascending order
7. Print the second-last element of the sorted list (i.e., the runner-up score)
8. **Stop**

---

## 💻 PROGRAM:
~~~c
def find_runner_up(scores):
    unique_scores = list(set(scores))  
    unique_scores.sort(reverse=True)  
    return unique_scores[1] 
n = int(input("Enter the number of participants: "))
scores = []
for _ in range(n):
    score = int(input(f"Enter score for participant {_+1}: "))
    scores.append(score)
runner_up = find_runner_up(scores)
print(f"\nThe runner-up score is: {runner_up}")
~~~

## OUTPUT
![442488909-b783abab-1f87-416f-a850-1cea87847cb2](https://github.com/user-attachments/assets/69e94e17-e2b2-425e-970c-7380c3560ddc)


## RESULT
Thus the program has been executed successfully.
