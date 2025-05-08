## **For Loop vs While Loop in Python**

Hello everyone!
In this presentation, we will understand the **major differences between `for` loop and `while` loop** in Python. Without any further delay, let’s get started!

We will discuss **three key differences** that will help you decide when to use a `for` loop and when to use a `while` loop depending on the situation.

---

### 🔹 **Difference #1: Based on Iteration Control**

* **`for` loop**: Requires an **iterable object** to iterate over.
* **`while` loop**: Executes based on a **condition**.

#### ✅ `for` loop syntax:

```python
for variable in iterable:
    # statements
```

* The loop runs based on the iterable object.
* Example iterables: `list`, `tuple`, `dictionary`, `range()` output, etc.

#### ✅ `while` loop syntax:

```python
while condition:
    # statements
```

* The loop runs as long as the condition is `True`.
* If the condition becomes `False`, the loop terminates.

---

### 🔹 **Difference #2: Known vs Unknown Number of Iterations**

* Use **`for` loop** when the number of iterations is **known in advance**.
* Use **`while` loop** when the number of iterations is **not known in advance**.

#### ✅ Example of `for` loop:

```python
for i in range(1, 6):
    print(i)
```

* Output: `1 2 3 4 5`
* The loop clearly runs **5 times**, as defined by `range(1, 6)`.

#### ✅ Example of `while` loop:

```python
while True:
    n = input("Enter a number (Q to quit): ")
    if n == 'Q':
        break
    print(n)
```

* The number of iterations is not known in advance.
* Loop continues until the user enters `'Q'`.

---

### 🔹 **Difference #3: Both Can Run Infinitely**

* Both `for` and `while` loops can be used to create **infinite loops**.

#### ✅ Infinite `for` loop example:

```python
items = [0]
for item in items:
    print(item)
    items.append(item)
```

* Each time, `0` is printed and appended back to the list.
* The list keeps growing, so the loop never ends.

#### ✅ Infinite `while` loop example:

```python
item = 0
while True:
    print(item)
```

* Since the condition is always `True` and there’s no break condition, the loop will run forever.

---

### ✅ **Summary of Key Differences**

| Feature                   | `for` loop                 | `while` loop                        |
| ------------------------- | -------------------------- | ----------------------------------- |
| Iteration type            | Based on iterable          | Based on condition                  |
| Use case                  | Known number of iterations | Unknown number of iterations        |
| Infinite loop possibility | Yes, with dynamic iterable | Yes, with `while True` and no break |

---

### 🎯 **Conclusion**

We’ve covered the three main differences between `for` loop and `while` loop. Now you should be able to decide which loop to use depending on whether you know the number of iterations in advance or not, and based on how your logic is structured.

Thank you for watching this presentation!
I’ll see you in the next one.

---
