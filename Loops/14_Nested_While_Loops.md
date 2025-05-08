---

### **Understanding Nested While Loops**

Hello friends!
In our last presentation, we learned about **nested for loops** and how they work. In this session, we will explore another important concept — the **nested while loop** — and understand its functionality in detail.

So without any further delay, let’s get started!

---

### **What is a Nested While Loop?**

A **nested while loop** is simply a `while` loop placed inside another `while` loop.
In this structure:

* The **outer loop** controls the number of times the **inner loop** runs.
* The **inner loop** executes completely every time the outer loop runs once.

This structure allows us to iterate over more complex patterns or datasets.

---

### **Example: Iterating Over Two Lists**

Let’s understand the concept with an example.

Suppose we have two lists:

```python
list1 = [1, 2, 3]
list2 = [4, 5, 6]
```

We want to print their combinations in the following order:

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

To achieve this, we can use a nested while loop. Here’s the approach:

---

### **Step-by-Step Code Explanation**

1. **Initialize index variables**:

```python
i = 0
```

2. **Start the outer while loop**:

```python
while i < len(list1):
```

3. **Inside the outer loop, initialize `j`**:

```python
    j = 0
```

4. **Start the inner while loop**:

```python
    while j < len(list2):
        print(list1[i], list2[j])
        j += 1
```

5. **After inner loop, print a newline and increment `i`**:

```python
    print()
    i += 1
```

---

### **Full Working Code**

```python
list1 = [1, 2, 3]
list2 = [4, 5, 6]

i = 0
while i < len(list1):
    j = 0
    while j < len(list2):
        print(list1[i], list2[j])
        j += 1
    print()
    i += 1
```

---

### **Output**

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

---

### **How It Works**

* The outer loop (`i`) controls which item of `list1` we are currently using.
* The inner loop (`j`) iterates through all elements of `list2` for each item of `list1`.
* We reset `j` to `0` after each outer loop iteration to start from the beginning of `list2`.
* After printing all combinations for a single item in `list1`, we print a newline for better readability.

---

### **Conclusion**

Just like nested for loops, nested while loops are extremely useful when dealing with multiple collections or printing patterns.
They allow for a deeper level of control, especially when the number of iterations is not fixed or known in advance.

---

Thank you for watching this presentation.
I hope the concept of nested while loops is now clear to you.
See you in the next session!

---
