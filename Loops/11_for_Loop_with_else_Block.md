## 📘 **Understanding `for` Loop with `else` Block in Python**

Hello everyone, and welcome to this presentation!
In this session, we will learn how the `for` loop works with the `else` block in Python.

So, without any further delay, let’s get started!

---

### 🔹 Topics Covered:

1. Introduction to `for` loop with `else` block
2. Use of `for` loop with `else` block

---

### ✅ **1. Introduction to `for` Loop with `else` Block**

You might already be familiar with the `else` block used with a `while` loop. The concept remains the same when using it with a `for` loop.

#### Key Concept:

* The `else` block executes **only when** the loop **completes normally** (i.e., it does **not encounter a `break` statement**).
* If the loop is **terminated early using `break`**, the `else` block is **skipped**.

#### Syntax:

```python
for item in sequence:
    # Statements inside the for loop
else:
    # Statements inside the else block (executed only if the loop completes without a break)
```

📝 **Important:**

* The `else` clause is **not** a fallback for the `if` inside the loop.
* It is tied to the loop's **completion status**.

---

### ✅ **2. Use of `for` Loop with `else` Block**

Let’s understand the practical use of the `else` block in a `for` loop through an example.

---

#### 🎯 Problem Statement:

We have a list of favorite programming languages.
We want to check if `"Java"` is present in the list.

* If **Java is found**, print: `I like Java`
* If **Java is not found**, print: `I don't like Java`

---

#### 📌 Step-by-Step Code Example:

```python
fave_languages = ["Python", "C", "Java", "Ruby"]

for language in fave_languages:
    if language == "Java":
        print("I like Java")
        break
else:
    print("I don't like Java")
```

---

#### 🧠 Explanation:

* The `for` loop iterates through each language in the `fave_languages` list.
* If `"Java"` is found, the message `"I like Java"` is printed, and the loop is terminated early using `break`.
* If the loop completes without finding `"Java"`, the `else` block is executed, printing `"I don't like Java"`.

---

#### 🔄 Execution Flow:

1. **First iteration:** language = `"Python"`

   * `"Python" == "Java"` → `False` → continue

2. **Second iteration:** language = `"C"`

   * `"C" == "Java"` → `False` → continue

3. **Third iteration:** language = `"Java"`

   * `"Java" == "Java"` → `True`
   * Output: `I like Java`
   * Loop exits due to `break`

4. **`else` block is skipped** because the loop terminated **abnormally** via `break`.

---

#### ✅ Output:

```
I like Java
```

📝 **If Java was not in the list**, the loop would complete normally, and the output would be:

```
I don't like Java
```

---

### 🎯 Summary

| Condition                   | Output            |
| --------------------------- | ----------------- |
| Java **is in** the list     | I like Java       |
| Java **is NOT in** the list | I don't like Java |

🧩 **Use Case:**
The `for...else` construct is especially useful for **searching** scenarios where an action must be taken only if the search **fails completely**.

---

### 🙏 Thank You!

This brings us to the end of this presentation on the `for` loop with the `else` block in Python.
Thanks for watching, and I’ll see you in the next session!

---
