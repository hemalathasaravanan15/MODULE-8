## EX 8 (A) Hackerrank: Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## Algorithm

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

## PROGRAM:
```
marks = eval(input())
total = 0
total_marks = marks.copy()
for key,val in marks.items():
    total = sum(val)
    total_marks[key] = total
print(total_marks)
max = 0
topper = ''
for key,val in total_marks.items():
    if val>max:
        max = val
        topper = key
print("Topper is: ", topper, "with marks = ",max)
```
## OUTPUT
<img width="1230" height="147" alt="image" src="https://github.com/user-attachments/assets/dd9ae7e7-100d-4a99-82f2-9e02abf82fdc" />

## RESULT
  Thus, the Python program that determine the **top-performing student** based on the total marks across five subjects has been executed successfully.

## EX 8 (B) Hackerrank : Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---

## Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## Algorithm

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


## Program
```
def wrap(string, max_width):
    wrapped_lines = []  # list to store each line
    for i in range(0, len(string), max_width):
        part = string[i:i+max_width]
        wrapped_lines.append(part)
    return '\n'.join(wrapped_lines)  
string, max_width = input(), int(input())
print(wrap(string, max_width))
```

## Output
<img width="833" height="293" alt="image" src="https://github.com/user-attachments/assets/4ac61ebc-84e3-4120-ae66-12c0a9e6c6d2" />

## Result
  Thus, the Python program defines a function that **wraps a long string into multiple lines** is executed successfully.

## EX 8 (C) Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---
## Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## Program
```
N=int(input())
students=[]
for i in range(N):
    name = input()
    score =float(input())
    students.append([name,score])
    
scores = sorted(set(score for _, score in students))
second_lowest_score=scores[1]

second_lowest_students= sorted([name for name,score in students if score == second_lowest_score])

for students in second_lowest_students:
    print(students)
```

## Output
<img width="394" height="403" alt="image" src="https://github.com/user-attachments/assets/16748459-f506-40dd-aae2-9b8a9db2528d" />

## Result
  Thus, the python program to find students with the second lowest grade has been executed successfully.

## EX 8 (D) Hackerrank:Runner-Up Score Finder in Python

## AIM:
To write a Python program that takes a list of scores from participants and finds the **runner-up score** (i.e., the second-highest score), eliminating any duplicates.

---

## ALGORITHM:

1. **Start**
2. Create a variable `n` and get its value from the user (number of participants)
3. Read the list of `n` scores from the user using `input().split()` and convert them to integers
4. Store the scores in a list
5. Use `set()` to remove any duplicate scores
6. Convert the set back to a list and sort it in ascending order
7. Print the second-last element of the sorted list (i.e., the runner-up score)
8. **Stop**

---

## PROGRAM:
```
n = int(input())
scores = list(map(int, input().split()))
unique_scores = set(scores)
unique_scores.remove(max(unique_scores))
runner_up = max(unique_scores)
print(runner_up)
```


## OUTPUT
<img width="424" height="171" alt="image" src="https://github.com/user-attachments/assets/cd2c105c-26ba-413c-876c-f4c5d9829266" />

## RESULT
  Thus, the python program to find the **runner-up score** from a list of scores has been executed successfully.

## EX 8 (E) Hackerrank:Python Program to Check if a String Ends with a Numeric Digit

This Python program checks whether the last character of a given input string is a **numeric digit (0–9)**.

---
## Aim

To write a Python program that checks if a given string ends with a number using Python's built-in string methods.

---

## Algorithm

1. **Start the program.**
2. **Input** a string from the user.
3. **Access** the last character using indexing (`string[-1]`).
4. **Check** if the last character is a digit using the `.isdigit()` method.
5. **If true**, print that the string ends with a number.
6. **Else**, print that the string does not end with a number.
7. **End the program.**

---

##  Program
```
string=input()
if(string[-1].isdigit()):
     print(True)
else:
     print(False)
```

## Output
<img width="441" height="204" alt="image" src="https://github.com/user-attachments/assets/b7425eaf-f986-4184-87b2-827807bfe488" />

## Result
  Thus, the python program to check if a string ends with a numeric digit has been executed successfully.
