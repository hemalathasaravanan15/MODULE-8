# 🔄 Hackerrank : # 📦 Python counting vowels and consonants

## 🎯 Aim

To count the number of vowels and consonants from the given string.

---

## 🧠 Algorithm
1. Start and take a string s as input.
2. Initialize vowel count cc = 0 and consonant count cv = 0.
3. For each character in s, check if it is a vowel (aeiouAEIOU).
4. If yes → increment cc, else → increment cv.
5. Print the values of cc (vowels) and cv (consonants).
---


## 🧪 Program
~~~
def fun(s,cc=0,cv=0):
    v='aeiouAEIOU'
    for i in s:
        if i in v:
            cc+=1
        else:
            cv+=1
    print("Number of Vowels:",cc)
    print("Number of Consonants:",cv)
s=input()
~~~

## Sample Output
<img width="780" height="186" alt="image" src="https://github.com/user-attachments/assets/f61f2be6-8adf-4bd9-8e46-fd1e6e541f67" />


## Result
Thus the output is verified.
