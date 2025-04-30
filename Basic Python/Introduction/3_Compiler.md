# 📘 Introduction to Compiler in Programming

In the previous session, we explored the **definition of Python programming**. Now, we are ready to understand **what a compiler is**. Let’s dive in!

---

## 📝 Topics Covered

This presentation will cover the following two topics:

1. **Why do we need a translator?**
2. **What is a compiler?**

---

## 🔄 Why Do We Need a Translator?

### 🧠 Human vs Machine Understanding

- Programs are generally written in **high-level programming languages** (e.g., Python, C, C++, Java) which **humans can understand easily**.
- Computers, however, can only understand **binary language** (a low-level language made of 0s and 1s).

### ⚠️ Communication Gap

There is a **gap** between what humans understand and what machines understand:

| Humans Understand | Machines Understand |
|-------------------|---------------------|
| High-Level Language (e.g., Python, C) | Low-Level Language (Binary: 0s and 1s) |

### 🔧 Role of a Translator

A **translator** is required to bridge this gap:
- It **converts high-level language code** into **binary code** that machines can understand.

There are **two types of translators**:

1. **Compiler** (covered in this presentation)
2. **Interpreter** (will be covered in the next session)

---

## 🛠️ What Is a Compiler?

### 📌 Definition

A **compiler** is a **complex software program** that:
- Converts **source code** (human-readable) into **machine code** (binary) **in one go**.
- Produces an **executable file** that can run independently on a machine.

> ⚠️ Note: A compiler is **not hardware**, it is **software**.

### 🔁 Example Using C Language

Let’s understand with a C program (since C is a **compiled language**).

```c
#include <stdio.h>
#include <conio.h>

int main() {
    int a = 10, b = 20, sum;
    sum = a + b;
    printf("%d", sum);
    getch(); // To hold the screen
    return 0;
}
```

### 💡 Why C and Not Python?

Python is an **interpreted language**, whereas C uses a **compiler**. Since this presentation is about compilers, C is more appropriate for the demonstration.

---

## 🖥️ Compilation and Execution Process

### 🏗️ Step-by-Step:

1. **Write source code** (e.g., `sum.c`).
2. **Use compiler** to compile the code.
3. Compiler converts it to an **executable file**:
   - On Windows: `.exe`
   - On Mac: `.app`
4. **Executable can be shared and run** on any compatible system **without the source code**.

---

## 🧪 Real-Time Demo (Using Code::Blocks IDE)

### 📂 Folder Setup

- File: `sum.c`
- Location: `Desktop/C Programs/`
- Use `getch()` to keep the window open until a key is pressed.

### 🧑‍💻 Compilation Output

After building in Code::Blocks:
- You get:
  - `sum.exe` (Executable)
  - `sum.o` (Object file — not important for now)

### ▶️ Running the Executable

1. Double-click on `sum.exe`.
2. Output shows: `30`
3. A blinking cursor waits for input.
4. Press any key (e.g., `h`) — the program window closes.

### 🔁 Sharing the Executable

- If your friend also has a **Windows machine**, they can **run the `.exe` file** directly.
- They **don’t need the `.c` source code** or compiler.
- This shows that the **compilation happens once**, and the executable can be reused.

---

## 🧠 Summary

### ✅ What We Learned

- A **translator** is required to convert high-level code to machine code.
- A **compiler**:
  - Is a **software**.
  - Converts code **in one go**.
  - Produces an **executable file**.
  - That executable can run independently on compatible systems.

---

## 🔜 Next Topic

In the **next presentation**, we will cover:

- 🧾 **What is an Interpreter?**
- 🔄 **Differences between Compiler and Interpreter**

---

## 🙏 Thank You

Thank you for following this presentation! See you in the next session on **Interpreters**.
