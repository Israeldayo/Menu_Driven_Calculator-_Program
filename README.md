# Menu_Driven_Calculator_Program

# 🧮 Python Campus Toolkit — Task 2

> Two practical Python programs built for the classroom: a smart calculator and a student grade manager.

## 📁 Contents

| Program | Description |
|--------|-------------|
| `Campus Calculator` | A menu-driven arithmetic calculator with loop-based UX |
| `Class Result Assistant` | A student score tracker with grade assignment and summary display |

## 🔢 Program 1 — Campus Calculator

A simple but clean interactive calculator that keeps running until the user decides to quit.

### ✨ Features
- Supports **addition, subtraction, multiplication, and division**
- Handles **division by zero** gracefully with an error message
- Validates non-numeric inputs using `try/except`
- Loops continuously with a clean menu until the user exits

### 🚀 Sample Interaction

=== Campus Calculator ===
1. Add
2. Subtract
3. Multiply
4. Divide
5. Exit
Choose an operation (1–5): 1
Enter first number: 2
Enter second number: 3
Result: 5.0

### 🧠 How It Works

```python
def add(a, b):      return a + b
def subtract(a, b): return a - b
def multiply(a, b): return a * b
def divide(a, b):
    if b == 0:
        return "Error: Division by zero is not allowed."
    return a / b

The main loop accepts a menu choice, prompts for two numbers, calls the appropriate function, and prints the result — repeating until `5` (Exit) is selected.


## 📊 Program 2 — Class Result Assistant

A teacher-facing tool to input student test scores, automatically calculate averages, assign grades, and display a formatted summary table.

### ✨ Features
- Add **multiple students**, each with a custom number of test scores
- Validates scores are within the **0–100 range**
- Automatically calculates **averages** (rounded to 2 decimal places)
- Assigns **letter grades** based on a standard scale
- Displays a **neatly formatted results table**

### 🎓 Grading Scale

| Average Score | Grade |
|--------------|-------|
| 70 and above | A |
| 60 – 69 | B |
| 50 – 59 | C |
| 40 – 49 | D |
| Below 40 | F |

### 🚀 Sample Output

======================================================================
                       STUDENT RESULTS SUMMARY                        
======================================================================
Name                 Scores                    Average    Grade
----------------------------------------------------------------------
Oyebade Israel       [80.0, 75.0, 85.0]        80.0       A    
Israel Dayo          [70.0, 75.0, 80.0]        75.0       A    
Juliet Dada          [65.0, 60.0, 75.0]        66.67      B    
Brown Joe            [50.0, 55.0, 58.0]        54.33      C    
Johnson Gabriel      [45.0, 40.0, 48.0]        44.33      D    
Duke Mike            [40.0, 35.0, 30.0]        35.0       F    
======================================================================

### 🧠 Key Functions

| Function | Purpose |
|----------|---------|
| `calculate_average(scores)` | Returns the mean of a list of scores |
| `assign_grade(average)` | Maps an average to a letter grade |
| `add_student(students_data)` | Prompts for name + scores, stores result |
| `display_results(students_data)` | Renders a formatted results table |
| `main()` | Drives the menu loop |


## ▶️ How to Run

Make sure you have **Python 3** installed, then run the notebook in Jupyter:

```bash
jupyter notebook "OYEBADE_ISRAEL_EKUNDAYO_TASK_2.ipynb"
```

Or copy individual cells into a `.py` file and run directly:

```bash
python campus_calculator.py
python class_result_assistant.py


## 🛠️ Built With

- **Python 3** — core language
- **Jupyter Notebook** — development and presentation environment
- **No external libraries** — pure Python standard library only


## 👨‍💻 Author

**Oyebade Israel Ekundayo**  
