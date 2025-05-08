Here’s a properly structured and clear version of your explanation for the **program to calculate the sum of the first *n* natural numbers using a while loop**:

---

### **Program 1: Sum of First *n* Natural Numbers (Using Conditionals and Loops)**

#### **Introduction**

In this presentation, we will learn how to write a Python program to calculate the **sum of the first *n* natural numbers** using **conditionals and loops**.
Let’s get started!

---

### **What Are Natural Numbers?**

Natural numbers are all **positive integers starting from 1** and going up to infinity.
Examples:
`1, 2, 3, 4, 5, 6, ...`

---

### **Problem Statement**

We need to write a Python program that:

* Takes an input *n* from the user
* Calculates the sum of the first *n* natural numbers
* Prints the result

---

### **Example**

If the user enters `n = 5`, the program should calculate:

`1 + 2 + 3 + 4 + 5 = 15`
So, the output should be:
`Sum is 15`

---

### **Steps to Solve**

#### **Step 1: Take Input from the User**

```python
n = int(input("Enter the value of n: "))
```

* The `input()` function reads input as a string.
* The `int()` function converts it to an integer.

#### **Step 2: Initialize a Variable for the Sum**

```python
sum = 0
```

We start the sum at 0. We will add values to it using a loop.

#### **Step 3: Use a While Loop to Calculate the Sum**

```python
while n > 0:
    sum += n
    n -= 1
```

* The loop continues while `n > 0`.
* Each time, it adds `n` to `sum`, then decreases `n` by 1.

#### **Step 4: Print the Final Result**

```python
print(f"Sum is {sum}")
```

---

### **Complete Code**

```python
n = int(input("Enter the value of n: "))
sum = 0

while n > 0:
    sum += n
    n -= 1

print(f"Sum is {sum}")
```

---

### **Output Example**

**Run 1:**

```
Enter the value of n: 5
Sum is 15
```

**Run 2:**

```
Enter the value of n: 10
Sum is 55
```

---

### **Conclusion**

* You now know how to use a while loop to calculate the sum of the first *n* natural numbers.
* Always initialize variables before using them in loops.
* The `input()` function is used to take user input, and `int()` is used to convert it into an integer.

---
