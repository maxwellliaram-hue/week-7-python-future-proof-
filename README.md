 week-7-python-future-proof-
  💰 Menu-Driven Expense Manager

A simple Python command-line expense manager that allows users to add, view, filter, and analyze their daily expenses.

This project demonstrates the use of lists, dictionaries, functions, loops, conditional statements, exception handling, list comprehensions, and f-strings.

  Project Overview

The Expense Manager is a menu-driven command-line application designed to help users keep track of their expenses.

Each expense is stored as a dictionary inside a Python list:

```python
{
    "amount": 500.00,
    "desc": "Lunch",
    "category": "Food"
}
```

The application provides five main options:

1. Add Expense
2. List All Expenses
3. Filter by Category
4. View Expense Summary
5. Quit

---

  Project Objectives

The main objectives of this week's milestone are to:

* Build a complete menu-driven Python application.
* Store data using a list of dictionaries.
* Validate user input.
* Handle invalid numeric input using `try/except`.
* Use functions to organize the program.
* Use list comprehensions for filtering.
* Calculate useful expense statistics.
* Practice writing clean and reusable Python code.

---

## 🚀 Features

### 1. Add Expense

Users can add a new expense by entering:

* Amount
* Description
* Category

The program validates the amount and ensures that:

* The amount is a valid number.
* The amount is greater than `0`.
* The description is not empty.

Example:

```text
Enter amount: 750
Enter description: Dinner
Enter category: Food

Expense added successfully!
```

---

### 2. List All Expenses

Displays all recorded expenses in a numbered format.

Example:

```text
--- All Expenses ---

1. Amount: KSh 500.00 | Description: Lunch | Category: Food
2. Amount: KSh 1500.00 | Description: Transport | Category: Transport
3. Amount: KSh 800.00 | Description: Internet bundle | Category: Communication
4. Amount: KSh 1200.00 | Description: Groceries | Category: Food
```

---

### 3. Filter by Category

Users can search for expenses belonging to a particular category.

The program uses a **list comprehension** to perform the filtering.

Example:

```text
Enter category: Food

Expenses in category: Food

1. KSh 500.00 | Lunch | Food
2. KSh 1200.00 | Groceries | Food
```

If no expenses match the category:

```text
No expenses found in category 'Entertainment'.
```

---

### 4. Expense Summary

The summary provides useful information about all recorded expenses.

It displays:

* Total expenses
* Number of expenses
* Average expense
* Largest expense
* Total spending per category

Example:

```text
--- Expense Summary ---

Total expenses: KSh 4000.00
Number of expenses: 4
Average expense: KSh 1000.00
Largest expense: KSh 1500.00 (Transport)

--- Per-Category Totals ---

Food: KSh 1700.00
Transport: KSh 1500.00
Communication: KSh 800.00
```

---

## 🛠️ Technologies Used

* **Python 3**
* Command Line Interface (CLI)
* Python Lists
* Python Dictionaries
* Functions
* `while` loops
* `for` loops
* `if/elif/else`
* List comprehensions
* Exception handling
* f-strings

No external libraries are required.

---

## 📂 Project Structure

```text
expense-manager/
│
├── expense_manager.py
└── README.md
```

### `expense_manager.py`

Contains the complete Python application.

### `README.md`

Contains project documentation, setup instructions, features, and usage information.

---

## 💻 Installation and Setup

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Enter the project directory

```bash
cd expense-manager
```

### Step 3: Run the application

```bash
python expense_manager.py
```

On some systems, use:

```bash
python3 expense_manager.py
```

---

## 📋 Main Menu

When the program starts, the following menu is displayed:

```text
================================
       EXPENSE MANAGER
================================
1. Add Expense
2. List All
3. Filter by Category
4. Summary
5. Quit
================================
Choose an option (1-5):
```

The program continues displaying the menu until the user selects **5. Quit**.

---

## 🧪 Example Usage

```text
Choose an option (1-5): 1

--- Add Expense ---

Enter amount: 1000
Enter description: Electricity
Enter category: Bills

Expense added successfully!
```

The new expense is stored in the list:

```python
{
    "amount": 1000,
    "desc": "Electricity",
    "category": "Bills"
}
```

---

## 🔐 Input Validation

The application prevents invalid expense amounts.

For example:

```text
Enter amount: abc
Invalid amount. Please enter a number.
```

It also prevents zero or negative expenses:

```text
Enter amount: -500
Amount must be greater than 0.
```

Empty descriptions are rejected:

```text
Enter description:
Description cannot be empty.
```

---

## 📊 Data Structure

Expenses are stored using a list of dictionaries:

```python
expenses = [
    {
        "amount": 500.00,
        "desc": "Lunch",
        "category": "Food"
    },
    {
        "amount": 1500.00,
        "desc": "Transport",
        "category": "Transport"
    }
]
```

This structure makes it easy to add, search, filter, and calculate information about expenses.

---

## 🧠 Python Concepts Demonstrated

### Lists

Used to store multiple expenses:

```python
expenses = []
```

### Dictionaries

Used to represent individual expenses:

```python
expense = {
    "amount": amount,
    "desc": desc,
    "category": category
}
```

### Functions

The program is divided into reusable functions:

```python
add_expense()
list_expenses()
filter_by_category()
show_summary()
```

### Exception Handling

Used to safely handle invalid numbers:

```python
try:
    amount = float(input("Enter amount: "))
except ValueError:
    print("Invalid amount.")
```

### List Comprehension

Used to filter expenses:

```python
filtered = [
    expense for expense in expenses
    if expense["category"].lower() == category.lower()
]
```

### Loops

The `while True` loop keeps the application running until the user chooses to quit.

---

## 🔮 Future Improvements

The project can later be expanded to include:

* Edit expenses
* Delete expenses
* Search by description
* Date tracking
* Monthly expense reports
* Budget limits
* Saving data to a file
* SQLite database
* PostgreSQL database
* Django web interface
* User authentication
* Expense charts and dashboards

---

## 🎓 Learning Milestone

This project represents a transition from basic Python programming to building a structured application.

The current application stores data in memory using:

```text
Python List
     ↓
Dictionaries
     ↓
Functions
     ↓
Menu System
```

The same logic can later be extended into a Django application:

```text
CLI Expense Manager
        ↓
Django Models
        ↓
Database
        ↓
Django Views
        ↓
Web Interface
```

---

👨‍💻 Author

Maxwell Liaram

Python / Software Development Student

---
<img width="678" height="413" alt="image" src="https://github.com/user-attachments/assets/7cadbcc0-6289-4edc-8329-92fb6d5411d0" />
<img width="695" height="467" alt="image" src="https://github.com/user-attachments/assets/f4baa7f1-cca2-4c7f-bb31-226bbcf48569" />



