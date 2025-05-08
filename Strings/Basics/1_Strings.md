## 📚 **Understanding Strings in Python**

In this presentation, we will cover the basics of **Strings in Python** and delve into important concepts related to them, including **String Data Types** and **Multi-line Strings**. Let’s get started without any further delay!

### 1. **String Data Type**

### 2. **Multi-line String**

---

### **1. String Data Type in Python**

A **string** in Python is simply a sequence of characters. Strings can be enclosed in either **single quotes (' ')** or **double quotes (" ")**. Python allows flexibility in using either format, which means both are valid.

Let's go over some examples:

---

#### **Example 1: Using Double Quotes**

In the Python interactive shell, we can create a string by enclosing text in double quotes:

```python
name = "Preet"
```

Here, we have created a string `"Preet"` and assigned it to the variable `name`.

---

#### **Example 2: Using Single Quotes**

Similarly, you can use **single quotes** to define a string:

```python
name = 'Preet'
```

Both representations are perfectly valid in Python, and Python does not differentiate between single or double quotes for strings.

---

#### **Working with Quotes Inside Strings**

In certain cases, you may need to include **quotes within a string**. Let’s look at an example:

##### **Example 3: Using Single Quotes Inside a String**

If you need to include an apostrophe or a single quote inside the string, enclose the entire string in **double quotes**:

```python
statement = "Python's syntax is simple."
```

##### **Example 4: Using Double Quotes Inside a String**

Alternatively, if you want to include double quotes inside the string, enclose the entire string in **single quotes**:

```python
statement = 'He said, "Hello, world!"'
```

Both methods are valid and help you avoid syntax errors.

---

#### **Handling Mixed Quotes (Error Case)**

If you try to mix single and double quotes without proper escape, Python will throw a syntax error. Let’s see an example:

```python
statement = "Hello, I am Preet. How's your mother?"
```

This will raise a **`SyntaxError`** because Python expects either a matching set of single or double quotes.

---

#### **Escaping Quotes with Backslashes**

To avoid the above error, you can use the **backslash (`\`)** character to escape quotes within the string. Let’s fix the issue:

```python
statement = "Hello, I am Preet. How\'s your mother?"
```

Here, the apostrophe in **`How's`** is escaped with a backslash (`\`), allowing it to be included in the string without causing any syntax errors.

Similarly, you can escape **double quotes** within a string:

```python
statement = 'He said, \"Hello, world!\"'
```

The backslash tells Python to treat the quotes as characters, not delimiters.

---

### **2. Multi-line String**

In Python, a **multi-line string** is a string that spans across multiple lines. It is defined using **triple single quotes (`'''`)** or **triple double quotes (`"""`)**. The string will preserve the format and newlines.

#### **Example 1: Defining a Multi-line String**

```python
statement = """Hello, world!
This is Preet.
How are you?"""
```

When we print this, it will preserve the line breaks:

```python
print(statement)
```

Output:

```
Hello, world!
This is Preet.
How are you?
```

Notice how each line of the string is preserved as part of the multi-line string.

---

#### **Interactive Example in Python Shell**

Let's look at an example in the Python shell:

```python
statement = """Hello, world!
This is Preet.
How are you?"""
```

If you hit **Enter**, Python will use the triple quotes to indicate that the statement is not finished yet. The three dots (`...`) show that you are continuing the multi-line string. When you hit **Enter** again, Python will know that the string is complete once the closing triple quotes are entered.

Now, printing the `statement` will give the following output:

```
Hello, world!
This is Preet.
How are you?
```

The format is exactly as we wrote it, with each part of the string appearing on a new line.

---

### **Summary:**

* **Strings** in Python are sequences of characters, which can be enclosed in **single quotes (' ')** or **double quotes (" ")**.
* If you want to include quotes within a string, you can either use **escaped quotes** or choose the appropriate type of quotes to enclose the string.
* A **multi-line string** is a string enclosed with **triple quotes (''' or """)**, allowing you to span the string across multiple lines while preserving the format.

---

Thank you for watching this presentation! I hope this clarifies the concepts of **String Data Types** and **Multi-line Strings** in Python.

In the next session, we will explore more advanced string manipulation techniques and operations. Stay tuned!
