# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

## 💻 PROGRAM:
```
python

def fun(n):
    if n > 0: fun(n-2); print(n, end=" ")

x = int(input())
fun(x if x % 2 == 0 else x - 1)
```

## OUTPUT
<img width="948" height="247" alt="446831269-0d26f5fe-9e30-4e5c-a175-c130f693849c" src="https://github.com/user-attachments/assets/f90861c4-6da3-4823-812b-99af6923e487" />

## RESULT
Thus, the program has been successfully executed.
# 🔁 Recursion:Palindrome Checker Using Recursion in Python

## 🎯 AIM:
To write a Python program to check whether a given string is a **palindrome** using **recursion**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `is_palindrome(word)`
   - **Base Case:** If the string length is less than 1, return `True`
   - **Recursive Case:** If the first and last characters match, call the function recursively on the substring without first and last characters
   - Else, return `False`
3. Get input from the user
4. Call the recursive function
5. Print whether the string is a palindrome
6. **Stop**

---

## 💻 PROGRAM:
```
  def is_palindrome(word):
      if len(word) <= 1:
          return True
      else:
          return word

  str=input()
  if str==str[::-1]:
      print("String is a palindrome")
  else:
      print("String is not a palindrome")
```
## OUTPUT
<img width="626" height="261" alt="442670732-373e1f74-b1a3-4205-b424-37fb2b52447a" src="https://github.com/user-attachments/assets/34cf4c4a-27df-4a7c-9f5d-a8e093b367b2" />

## RESULT
Thus, the program has been execueted successfully.
# # 🔁 Recursion:Sum of Digits using Recursion in Python

## 🎯 AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## 💻 PROGRAM:
```
l=[]
def SUM(n):
   if n==0:
      return 1
dig=n%10
l.append(dig)
SUM(n//10)
n=int(input())
SUM(n) print(sum(l))
```
## OUTPUT
<img width="1172" height="212" alt="442052734-2164457f-bc53-4484-8abc-42c3ab314603" src="https://github.com/user-attachments/assets/c9522828-e009-408a-ab94-c377403ada5c" />

## RESULT
Program successfully verified.
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
# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:
```
def series(x,n):
    if n==0:
        return x
    return x**(2*n+1)/fact(2*n+1)+series(x,n-1)
def fact(n):
    if n==0:
        return 1
    return n*fact(n-1)
x=int(input())
n=int(input())
result=series(x,n)
print(result)
```

## OUTPUT
<img width="1137" height="269" alt="508686428-295b8bd9-7aa5-4471-9f38-6df4675a5aaf" src="https://github.com/user-attachments/assets/bb73437a-7307-4aa1-ad59-124e362538aa" />

## RESULT
Thus, the program has been successfully executed.
