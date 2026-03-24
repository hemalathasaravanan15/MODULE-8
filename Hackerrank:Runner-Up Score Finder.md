# 🏆 Hackerrank:Average of marks array

## 🎯 AIM:
To write the python program to find the average of the marks array for the student name provided, showing 2 places after the decimal.

---

## 🧠 ALGORITHM:

1. Read integer n (number of students).
2. Create empty dictionary student_marks.
3. For each student (repeat n times):
Read name and scores.
Store in dictionary with name as key and scores as values.
4. Read query_name.
5. Get that student’s scores from dictionary.
6. Calculate sum of scores and divide by number of subjects.
7. Print average with 2 decimal places.

---

## 💻 PROGRAM:
~~~
n=int(input())
student_marks={}
for _ in range(n):
    line=input().split()
    name,scores=line[0],line[1::]
    scores=map(float,scores)
    student_marks[name]=scores
query_name=input()
marks=0
for i in student_marks[query_name]:
    marks=marks+i
avg=marks/3
print("%.2f"%avg)
~~~

## OUTPUT
<img width="423" height="222" alt="image" src="https://github.com/user-attachments/assets/78bc1664-8aed-4298-ace3-126f5f372724" />


## RESULT
Thus the output is verified.
