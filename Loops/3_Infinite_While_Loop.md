## **Understanding Infinite While Loops in Python**

Hello everyone!
In this presentation, we will learn about **infinite while loops** in Python. Without any further delay, let’s get started.

---

### **Topics Covered**

1. Introduction to Infinite While Loop
2. Breaking an Infinite While Loop

---

### **1. Introduction to Infinite While Loop**

Let’s begin by understanding what an infinite while loop is.

A **while loop** in Python repeatedly executes a block of code as long as the given condition is `True`. But what happens if the condition **never becomes `False`**?

In that case, the loop runs **infinitely**, meaning it will never stop on its own. This is called an **infinite loop**, and it can lead to wasted time and system resources if not handled properly.

---

#### **Example of an Infinite Loop**

```python
n = 100
while True:
    print(n)
    n -= 1
```

In this example:

* We set `n = 100`.
* The loop condition is `True`, which **always evaluates to true**, so the loop **never stops**.
* Inside the loop, we print `n` and then decrement it by 1.
* This will keep printing numbers: 100, 99, 98... into the negatives, **forever**.

---

### **How to Stop an Infinite Loop in Visual Studio Code**

When running such a loop in Visual Studio Code, you can stop it manually:

* On **Windows**, press `Ctrl + C`.
* On **Mac**, press `Command + C`.

This sends a **keyboard interrupt** to stop the execution.

---

### **2. Breaking an Infinite While Loop (Programmatically)**

Sometimes, you may **intentionally use** an infinite loop when the exit condition is not known in advance (e.g., waiting for user input). In such cases, we can use the **`break` statement** to exit the loop when a certain condition is met.

#### **Example with User Input**

```python
while True:
    line = input("Enter a line (or type 'Q' to quit): ")
    if line == 'Q':
        break
    print(line)
```

In this example:

* The loop runs infinitely using `while True`.
* We prompt the user to enter a line.
* If the input is `'Q'`, we use `break` to **exit** the loop.
* Otherwise, the line is printed, and the loop continues.

---

### **Demo in Visual Studio Code**

1. Create a file named `breaking_while_loop.py`.
2. Add the above code.
3. Run the file using the terminal:

   ```bash
   python breaking_while_loop.py
   ```

**Sample Run:**

```
Enter a line (or type 'Q' to quit): Hello
Hello
Enter a line (or type 'Q' to quit): Python
Python
Enter a line (or type 'Q' to quit): Q
```

* The loop ends when `'Q'` is entered.

---

### **When to Use Infinite While Loops**

Infinite loops are useful in scenarios like:

* Waiting for user input
* Listening for events (in GUIs or servers)
* Repeated tasks where the stop condition is dynamic

However, always ensure that **a way to exit the loop** is implemented, either manually or programmatically.

---

### **Conclusion**

In this session, we learned:

* What an infinite while loop is
* How to stop it manually
* How to break it programmatically using the `break` statement
* When it is appropriate to use infinite loops

---
