# Task 03 — VS Code Setup and Python Execution

**Due:** 2026-06-22

---

## 1. Install VS Code

1. Go to https://code.visualstudio.com/
2. Download the installer for your OS (Windows / macOS / Linux)
3. Run the installer and follow the setup steps
4. Launch VS Code once installation is complete

---

## 2. Install the Python Extension

1. Open VS Code
2. Click the **Extensions** icon in the left sidebar (or press `Ctrl+Shift+X`)
3. Search for **"Python"**
4. Select the extension published by **Microsoft** and click **Install**
5. VS Code will prompt you to select a Python interpreter — choose your installed Python version

---

## 3. Create and Run a Simple Python Program

### Core Program — Personalised Greeting

Manually wrote a Python file `greeting.py` that asks for the user's name and prints a welcome message:

```python
name = input("Enter your name: ")
print(f"Hi {name}, Welcome to Python!")
```

**Output:**
```
Enter your name: Raj
Hi Raj, Welcome to Python!
```

Program was created and executed directly inside VS Code using the built-in terminal.

---

## Bonus — AI-Assisted Time-Sensitive Greeting with OpenCode

As a bonus, I used **OpenCode** — an AI coding agent — to extend the program with a time-sensitive greeting. This demonstrates the power of AI coding assistants in accelerating development.

OpenCode generated the following code from a natural language prompt:

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

Rather than writing this logic manually, OpenCode generated the full solution from a simple prompt — showing how AI coding agents can handle boilerplate logic instantly, freeing the developer to focus on higher-level problems.

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
