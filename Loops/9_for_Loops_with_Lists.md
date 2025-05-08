## 📘 **Understanding `for` Loops with Lists in Python**

Hello everyone, and welcome to this presentation.
In this session, we will understand how the `for` loop works with **lists** in Python.

Without any further delay, let’s get started!

---

### 🔹 Topics Covered:

1. **Iterating over a list using `for` loop**
2. **Iterating over a list using `for` loop and `range()` function**
3. **Using list comprehension**

---

### ✅ **1. Iterating Over a List Using `for` Loop**

We can use a `for` loop to iterate through each item in a list. This is useful when we want to process or display each item individually.

#### Example:

```python
cars = ["Audi", "BMW", "Toyota"]

for car in cars:
    print(car)
```

#### Explanation:

* The list `cars` contains three elements.
* The `for` loop uses the variable `car` to access each element one at a time.
* Each car name is printed on a new line.

#### Output:

```
Audi
BMW
Toyota
```

📝 **Tip:** Use a meaningful singular name (like `car`) when iterating over a list (like `cars`).

---

### ✅ **2. Iterating Over a List Using `for` Loop and `range()` Function**

Instead of iterating directly over the list, we can use indices.
This is done using the `range()` function along with the `len()` function.

#### Example:

```python
cars = ["Audi", "BMW", "Toyota"]

for i in range(len(cars)):
    print(cars[i])
```

#### Explanation:

* `len(cars)` returns the number of items (3).
* `range(3)` gives a sequence: `0, 1, 2`
* `cars[i]` accesses elements using their index.

#### Output:

```
Audi
BMW
Toyota
```

This method is useful when you need to know the index of each item during iteration.

---

### ✅ **3. Using List Comprehension**

List comprehensions allow us to write compact code to perform operations on list items.

#### Example:

```python
cars = ["Audi", "BMW", "Toyota"]

[print(car) for car in cars]
```

#### Explanation:

* This is a list comprehension that executes `print(car)` for each item in the list.
* It’s more concise but should be used with care, especially when not returning a new list.

#### Output:

```
Audi
BMW
Toyota
```

🛑 **Note:** List comprehensions are meant for creating new lists. Using them for side effects like printing is possible, but not always recommended for production code.

---

### 🎯 Summary

* `for` loops allow easy traversal of lists.
* You can use `in` to iterate directly or `range(len(...))` to iterate via indices.
* List comprehensions offer a compact syntax for simple operations.

---

### 🙏 Thank You!

This concludes our presentation on using `for` loops with lists in Python.
Thank you for watching, and I’ll see you in the next session!

---
