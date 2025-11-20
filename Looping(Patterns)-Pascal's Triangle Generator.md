# 2(d) Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## Algorithm

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

##  Program
```
n=int(input())

for i in range(n):
    print(" " * (n-i-1), end="")
    num = 1
    row = []
    for j in range(i+1):
        row.append(str(num))
        num = num * (i-j) // (j+1)
    print(" ".join(row))

```

## Sample Output
<img width="867" height="552" alt="image" src="https://github.com/user-attachments/assets/fedffe89-ccb5-4f4b-8772-5c4e62588bf5" />


## Result
programme executed successfully
