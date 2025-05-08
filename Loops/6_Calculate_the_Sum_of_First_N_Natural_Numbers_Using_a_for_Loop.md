**Presentation: Program to Calculate the Sum of First N Natural Numbers Using a `for` Loop**

Hello everyone,
In this presentation, we will discuss **Program Number 2 on Conditionals and Loops**. Specifically, we will write a Python program to calculate the sum of the first *n* natural numbers using a `for` loop. Let’s get started.

---

### **Program Overview**

Previously, we learned how to calculate the sum of the first *n* natural numbers using a `while` loop. Today, we'll explore how to do the same using a `for` loop.

---

### **Step 1: Getting User Input**

The first step is to receive the value of *n* from the user, as we need to calculate the sum of the first *n* natural numbers. We will use the `input()` function to prompt the user for the value of *n*.

```python
n = input("Enter the value of n: ")
```

By default, the `input()` function returns the value as a string. Since we need an integer, we will typecast the input using the `int()` function:

```python
n = int(input("Enter the value of n: "))
```

Now, if the user enters `5`, the value of *n* will be 5.

---

### **Step 2: Initialize the Sum Variable**

Next, we need a variable to store the sum of the first *n* natural numbers. Let’s initialize this variable `sum` to 0.

```python
sum = 0
```

---

### **Step 3: Use `for` Loop with `range()` Function**

We can use the `range()` function to generate numbers from `1` to *n*. The `range(start, stop)` function generates numbers from `start` to `stop-1`. To get numbers from `1` to *n*, we will set `start=1` and `stop=n+1`:

```python
for i in range(1, n + 1):
    sum += i
```

This loop will iterate through all numbers from `1` to *n*, adding each number to the `sum` variable.

---

### **Step 4: Print the Result**

After the loop completes, we can print the sum using an f-string for better readability:

```python
print(f"Sum of first {n} natural numbers is {sum}")
```

---

### **Step-by-Step Execution**

Let’s break down the execution process.

1. The program asks the user to input the value of *n*. If the user inputs `5`, then `n` will be 5.
2. The `for` loop runs from `1` to `5`. On each iteration:

   * For `i = 1`, `sum` becomes `0 + 1 = 1`.
   * For `i = 2`, `sum` becomes `1 + 2 = 3`.
   * For `i = 3`, `sum` becomes `3 + 3 = 6`.
   * For `i = 4`, `sum` becomes `6 + 4 = 10`.
   * For `i = 5`, `sum` becomes `10 + 5 = 15`.
3. Finally, the program prints:

   ```
   Sum of first 5 natural numbers is 15
   ```

---

### **Example 1: Execution in Visual Studio Code**

Let's now execute this code in Visual Studio Code. I've created a file called `natural_sum.py` in my Python folder. Here's how the code looks:

```python
n = int(input("Enter the value of n: "))
sum = 0
for i in range(1, n + 1):
    sum += i
print(f"Sum of first {n} natural numbers is {sum}")
```

Now, let's open the terminal in Visual Studio Code, navigate to the folder containing the file, and execute it:

```bash
python natural_sum.py
```

* **Input 1**: If the user enters `5`, the output will be:

  ```
  Sum of first 5 natural numbers is 15
  ```

* **Input 2**: If the user enters `10`, the output will be:

  ```
  Sum of first 10 natural numbers is 55
  ```

---

### **Conclusion**

As demonstrated, we can easily calculate the sum of the first *n* natural numbers using a `for` loop and the `range()` function in Python. The `for` loop iterates over the numbers, summing them up and giving us the final result.

That’s all for this presentation. I hope the concept is clear now.

Thank you for watching!
See you in the next one!

---
