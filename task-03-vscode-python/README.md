# Task 03 — VS Code Setup and Python Execution

**Due:** 2026-06-22

This task covers setting up a professional Python development environment using VS Code, installing the Python extension, and writing and running Python programs — including a bonus AI-assisted feature built with OpenCode.

---

## 1. Install VS Code

VS Code (Visual Studio Code) is a free, lightweight but powerful source code editor. It is the most widely used IDE for Python and AI development due to its rich extension ecosystem, built-in terminal, and seamless Git integration.

**Steps:**
1. Go to https://code.visualstudio.com/
2. Download the installer for your OS (Windows / macOS / Linux)
3. Run the installer and follow the setup steps
4. Launch VS Code once installation is complete

---

## 2. Install the Python Extension

Out of the box, VS Code is a general-purpose editor. The **Python extension by Microsoft** adds everything needed for Python development: syntax highlighting, IntelliSense (auto-complete), linting, debugging, and the ability to run Python files directly inside VS Code.

**Steps:**
1. Open VS Code
2. Click the **Extensions** icon in the left sidebar (or press `Ctrl+Shift+X`)
3. Search for **"Python"**
4. Select the extension published by **Microsoft** and click **Install**
5. VS Code will prompt you to select a Python interpreter — choose your installed Python version

Once installed, VS Code recognises `.py` files, highlights errors as you type, and provides a **Run** button to execute your code without touching the terminal.

---

## 3. Create and Run a Simple Python Program

### Purpose

The goal of this program is to demonstrate the core Python concepts of **user input**, **string formatting**, and **console output** — the building blocks of any interactive application.

### Core Program — Personalised Greeting

Manually created a Python file `greeting.py` inside VS Code:

```python
name = input("Enter your name: ")
print(f"Hi {name}, Welcome to Python!")
```

**What each line does:**
- `input(...)` — pauses the program and waits for the user to type their name, then stores it in the variable `name`
- `print(f"...")` — uses an **f-string** to embed the variable directly into the output string and prints it to the console

**How to run it in VS Code:**
1. Open the file in VS Code
2. Click the **Run** button (▷) in the top right, or press `Ctrl+F5`
3. The built-in terminal opens and the program executes

**Output:**
```
Enter your name: Raj
Hi Raj, Welcome to Python!
```

---

## Bonus — AI-Assisted Time-Sensitive Greeting with OpenCode

### Purpose

This bonus demonstrates the power of **AI coding agents** in a real development workflow. Rather than writing boilerplate logic manually, I used **OpenCode** — an AI coding agent — to generate an extended version of the greeting program that adapts based on the time of day.

This mirrors how professional developers use AI tools to accelerate development: describe what you want in plain English, review and run the generated code, and ship faster.

### What OpenCode Generated

From a simple natural language prompt, OpenCode produced the following code:

```python
import datetime

name = input("Enter your name: ")

hour = datetime.datetime.now().hour

if hour < 12:
    greeting = "Good Morning"
elif hour < 17:
    greeting = "Good Afternoon"
else:
    greeting = "Good Evening"

print(f"{greeting} {name}, Welcome to Python!")
```

**What each part does:**
- `import datetime` — imports Python's built-in `datetime` module, no installation needed
- `datetime.datetime.now().hour` — gets the current hour (0–23) from the system clock
- `if / elif / else` — checks the hour and assigns the right greeting:
  - `0–11` → Good Morning
  - `12–16` → Good Afternoon
  - `17–23` → Good Evening
- `print(f"...")` — combines the greeting, name, and welcome message into one output

**Output examples depending on time of day:**
```
Enter your name: Raj
Good Morning Raj, Welcome to Python!
```
```
Enter your name: Raj
Good Afternoon Raj, Welcome to Python!
```
```
Enter your name: Raj
Good Evening Raj, Welcome to Python!
```

### Key Takeaway

OpenCode wrote the complete time-based logic from a single prompt — no manual lookup of the `datetime` API, no writing conditional branches by hand. This is a practical example of how AI coding agents reduce development time and let engineers focus on what actually matters: the problem, not the syntax.

---

## Video Evidence

Watch the full setup and demo here:  
[VS Code Setup and Python Execution — June Super 30](https://www.youtube.com/watch?v=Rv71CHqc3rw)

---

## Evidence Links

| Item | Link |
|---|---|
| This document | https://github.com/rajvin-cn/SP30-GenAI/blob/main/task-03-vscode-python/README.md |
| Video | https://www.youtube.com/watch?v=Rv71CHqc3rw |
| Repo | https://github.com/rajvin-cn/SP30-GenAI/tree/main/task-03-vscode-python |
