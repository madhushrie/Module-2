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
```
def print_pascals_triangle(n):
    for i in range(n):
       
        print(" " * (n - i - 1), end="")
        num = 1
        for j in range(i + 1):
            print(num, end=" ")
            num = num * (i - j) // (j + 1)
        print()
n = int(input())
print_pascals_triangle(n)

```
## Sample Output
<img width="1298" height="599" alt="image" src="https://github.com/user-attachments/assets/b65387c2-a4b7-4175-8b5a-a8a585b864b5" />

## Result
Thus the program is executed successfully.
