# **String Formatting in Python – Part 2: f-Strings**

Hello and welcome!
Let's continue our discussion on string formatting in Python. In this presentation (Part 2), we will focus on a single but powerful topic: **f-Strings**.

---

## **What Are f-Strings?**

An **f-string** (formatted string literal) is a feature in Python used to format strings in a concise and readable way.

### **Syntax:**

```python
f"your string here {expression}"
```

* Prefix the string with an `f` or `F`.
* Inside the string, use `{}` to include variables or expressions that should be evaluated.
> * Inside the string, use {} to include variables or expressions that should be calculated or replaced with their value.

### **Example:**

```python
name = "Jaspreet"
city = "Delhi"
print(f"My name is {name} and I live in {city}")
```

**Output:**

```
My name is Jaspreet and I live in Delhi
```

You can also use single quotes `'` instead of double quotes `"`, and both lowercase `f` and uppercase `F` work the same.

---

## **Calling Methods Within f-Strings**

You can call string methods directly within the `{}`.

### **Example:**

```python
name = "Jaspreet"
city = "Delhi"
print(f"My name is {name.upper()} and I live in {city.upper()}")
```

**Output:**

```
My name is JASPREET and I live in DELHI
```

---

## **Multiline f-Strings**

For better readability, f-strings can span multiple lines. There are three ways to do this:

### **1. Using Backslashes:**

```python
introduction = f"My name is {name} and I am {age} years old. " \
               f"I live in {city} and I am a {gender}."
```

### **2. Using Parentheses:**

```python
introduction = (
    f"My name is {name}.\n"
    f"My age is {age}.\n"
    f"I am a {gender}."
)
```

### **3. Using Triple Quotes:**

```python
introduction = f"""My name is {name}.
My age is {age}.
I am a {gender}."""
```

**Note:** Triple-quoted strings preserve newline characters `\n`, tabs `\t`, and white spaces.

---

## **Quotation Marks in f-Strings**

You can mix and match different types of quotation marks:

### **Examples:**

```python
f"My name is '{name}'"
f'She said, "{name}"'
f'''Hello, {name}'''
f"""Welcome, {name}"""
```

---

## **Escaping Quotation Marks**

To include quotes inside your string, use a backslash `\`:

### **Example:**

```python
print(f"I am \"{name}\" and I live in \"{city}\".")
```

**Output:**

```
I am "Jaspreet" and I live in "Delhi".
```

---

## **Including Curly Braces in Output**

To display literal curly braces in the output, double them:

### **Example 1:**

```python
x = 10
y = 20
print(f"The result of {{x + y}} is {x + y}")
```

**Output:**

```
The result of {x + y} is 30
```

### **Example 2 – Wrapping Evaluated Expression:**

```python
print(f"The result is {{{x + y}}}")
```

**Output:**

```
The result is {30}
```

---

## **Summary of f-Strings Features**

✅ Format strings with embedded expressions
✅ Call methods on variables directly
✅ Support multi-line string formatting
✅ Allow any type of quotation marks
✅ Let you escape characters using `\`
✅ Use `{{` and `}}` to display curly braces

---

### ✅ With that, you now have a complete understanding of f-strings in Python!

Thank you for watching this presentation.
I'll see you in the next one.

---

Would you like me to convert this into a PDF or slides for easy revision?
