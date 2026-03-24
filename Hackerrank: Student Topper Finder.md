# # 🔢 Hackerrank:# 🏆 Elements from list

## 🎯 Aim

To display elements from a list, present at odd index positions

---

## 🧠 Algorithm

1. Start the program.
2. Input an integer n → number of strings to read.
3. Initialize an empty list l.
4. Repeat n times:
5. Read a string lst.
6. Append lst to the list l.
7. Loop through the indices of list l:
8. If the index i is odd (i % 2 != 0), then:
9. Print the string at position l[i] without newline (use end='').
10. End the program.

---

## 💻 PROGRAM:
~~~
n=int(input())
l=[]
for i in range(n):
    lst=input()
    l.append(lst)
for i in range(len(l)):
    if i%2!=0:
        print(l[i],end='')
~~~

## OUTPUT
<img width="417" height="328" alt="image" src="https://github.com/user-attachments/assets/69062ed7-7210-47e5-96f7-c2ce7fce96f3" />


## RESULT
Thus the output is verified.
