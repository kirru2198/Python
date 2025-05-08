### **Presentation Script: Understanding Nested For Loops**

Hello everyone,
In this presentation, we will understand the concept of **nested for loops**. So without any further delay, let’s get started!

---

### **Topics Covered**

We will cover the following two topics in this session:

1. Introduction to Nested Loops
2. Nested For Loop with Example

---

### **1. Introduction to Nested Loops**

Let’s begin with the first topic — **Introduction to Nested Loops**.

So, what is a nested loop?

A **nested loop** refers to a loop inside another loop. When we place one loop inside the body of another, this structure is called a **nested loop**.

---

### **Syntax of Nested Loops**

Here’s how a nested loop looks in Python:

```python
for outer in outer_range:
    for inner in inner_range:
        # inner loop statements
    # outer loop statements
```

* The **outer loop** is written first.
* Inside the outer loop, we write the **inner loop**, properly indented.
* Inside the inner loop, we write the statements we want to execute multiple times.
* Be sure to follow proper **indentation rules** in Python — this is important for the loop to work correctly.

---

### **2. Nested For Loop**

Now, let’s move to the second topic: **Nested For Loop**.

A **nested for loop** is simply a `for` loop inside another `for` loop. This allows us to perform repeated actions in a structured way, such as iterating over elements in two lists and printing them in combinations.

---

### **Example: Printing Combinations from Two Lists**

Let’s understand nested for loops with a practical example.

Suppose we have two lists:

```python
list1 = [1, 2, 3]
list2 = [4, 5, 6]
```

We want to print each combination of elements from `list1` and `list2` in the following order:

```
1 4
1 5
1 6

2 4
2 5
2 6

3 4
3 5
3 6
```

To achieve this output, we can use a nested for loop as shown below:

```python
list1 = [1, 2, 3]
list2 = [4, 5, 6]

for i in list1:
    for j in list2:
        print(i, j)
    print()  # To print a newline after each inner loop
```

---

### **How This Code Works**

Let’s break it down step-by-step:

1. The **outer loop** iterates over `list1`. So, the variable `i` takes the values `1`, then `2`, then `3`.
2. For each value of `i`, the **inner loop** runs completely. So for `i = 1`, `j` takes the values `4`, `5`, and `6`, and prints them as `1 4`, `1 5`, and `1 6`.
3. After the inner loop completes, we print a blank line using `print()` to separate each group.
4. This process repeats for `i = 2` and then for `i = 3`.

This nested loop helps us generate and display all possible pairwise combinations between the two lists.

---

### **Conclusion**

To summarize:

* A **nested for loop** is used when we need to loop over multiple collections or generate patterns.
* It’s especially useful for working with matrices, grids, or printing patterns.
* We saw how a nested for loop can print all combinations from two lists.

In our upcoming sessions, we’ll learn how to use nested loops to display different types of **patterns**, such as stars, numbers, and characters.

---

Thank you for watching this presentation!
I hope the concept of **nested for loops** is now clear.
I’ll see you in the next one. Until then, keep practicing!

---
