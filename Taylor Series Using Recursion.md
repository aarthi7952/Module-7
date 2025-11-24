# 📐 Taylor Series Using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

## 💻 PROGRAM:
```
def series(x,n):
    if n==0:
        return 1
    else:
        return x**n+series(x,n-1)
x=int(input())
n=int(input())
print(series(x,n))

```
## OUTPUT
<img width="947" height="261" alt="508686300-be9b72a1-cf7c-4dca-b9c5-aaa3f75bee26" src="https://github.com/user-attachments/assets/6e009f60-f246-43a2-9a62-489cffbca6bd" />

## RESULT
Thus, the program has been successfully executed.
