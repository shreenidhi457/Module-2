# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
~~~
def pas(n):
    for i in range(n):
        print(" "*(n-1-i),end="")
        a=1
        for j in range(i+1):
            print(a,end=" ")
            a=a*(i-j)//(j+1)
        print()
n=int(input())
pas(n)
~~~

## Sample Output
<img width="575" height="621" alt="Screenshot 2026-03-26 110835" src="https://github.com/user-attachments/assets/93176be4-7afe-43d0-8883-72315dce9a7c" />

## Result
The program successfully generates Pascal's Triangle with the specified number of rows, using the appropriate formula for combination values.

