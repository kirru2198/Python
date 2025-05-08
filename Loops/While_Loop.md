### 🎥 **While Loop in Python – Basics Explained**

**Hello everyone!**
In this presentation, we will understand the **basics of the `while` loop** in Python. So, without any further delay, let’s get started.

---

### 🧩 **Agenda for This Session**

1. **Updating a Variable**
2. **Understanding the While Loop**

---

### 🧠 **1. Updating a Variable**

Before diving into the `while` loop, it’s important to first understand how to update a variable in Python. This concept is crucial for working with loops.

Let’s take a simple example:

```python
x = 0
x = x + 1
```

* Initially, `x` is assigned the value `0`.
* In the second line, we update `x` by **adding 1 to its current value**.
* So `x = x + 1` becomes `x = 0 + 1`, which results in `x` being updated to `1`.

This is how we update a variable in Python.

Now, let’s see what happens if we remove the initialization:

```python
x = x + 1
```

This will result in an **error** because Python does not know what the current value of `x` is. We must always **initialize a variable before updating it**.
> This will result in an error because Python does not know what the current value of x is. We must always give a variable a starting value before updating it.

🔴 **Key Takeaway**:
You **must initialize** a variable **before updating** it. This is a common source of bugs, especially when working with loops.

---

### 🔁 **2. Basics of While Loop**

The `while` loop allows us to **repeat a block of code** as long as a certain condition is `True`.
> The while loop lets us keep running some code again and again as long as a condition is true.

#### 📌 Syntax:

```python
while condition:
    # code block to repeat
```

As long as the `condition` remains true, the code block will keep executing.

---

### 🧪 **Example: Print 1 to 3 Using a While Loop**

Let’s say we want to print numbers 1, 2, and 3. Of course, we could use three `print()` statements, but that’s not scalable. What if we had to print numbers from 1 to 100? That’s where loops help.
> Let’s say we want to print numbers 1, 2, and 3. Of course, we could use three print() statements, but that wouldn’t work well if we had many more numbers to print.

Let’s see how we can do this with a `while` loop:

```python
n = 1
while n <= 3:
    print(n)
    n += 1
```

#### ✅ Step-by-step execution:

1. `n = 1` (initialization) # (starting value) - (n = 1 is giving n a starting value.)
2. Check: Is `n <= 3`? → Yes (`1 <= 3`)
3. Print `n` → prints `1`
4. Update: `n = n + 1` → `n = 2`
5. Repeat: Is `2 <= 3`? → Yes → prints `2`, then `n = 3`
6. Repeat: Is `3 <= 3`? → Yes → prints `3`, then `n = 4`
7. Repeat: Is `4 <= 3`? → No → loop stops

✅ Output:

```
1
2
3
```

---

### 💡 Summary

* Always **initialize a variable** before updating it.
* The `while` loop executes a block of code **as long as the condition is true**.
* Use `while` loops when the number of iterations is not known in advance.

---

### 👋 Closing

That brings us to the end of this session.
Thank you for watching this presentation!
I’ll see you in the next one. 😊

---

Let me know if you'd like this in slide format or with code examples visually structured!
