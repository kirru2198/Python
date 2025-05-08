### ✅ "Calling methods" means:

**Using a function that belongs to an object** (like a string, list, or number).

### 🔍 In the context of f-strings:

It means you can **run a method (function)** directly **inside the `{}`** to format or change the value.

---

### 🔧 Example:

```python
name = "alice"
print(f"Hello, {name.upper()}!")
```

* Here, `.upper()` is a **method** that turns the name into uppercase.
* `name.upper()` is **calling a method** inside the f-string.

**Output:**

```
Hello, ALICE!
```
