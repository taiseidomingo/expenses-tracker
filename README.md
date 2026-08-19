# Personal Expense Tracker

A modular Command-Line Interface (CLI) application written in Python to track, categorize, and analyze daily personal finances. This repository showcases the evolution of the project from a simple procedural script (**v1**) into a structured, feature-rich application (**v2**).

---

## 📌 Project Overview

This Python CLI Personal Expense Tracker evolved from a simple script into a modular app. **v1** provided basic expense tracking, sum totals, and max-cost lookups using list dictionaries. **v2** adds functional architecture, preset categories, auto-timestamps, record deletion, daily filtering, try-except safety, and JSON exports for top purchases.

---

## ✨ Features Comparison

| Feature | Version 1 (`v1.py`) | Version 2 (`v2.py`) |
| :--- | :--- | :--- |
| **Architecture** | Single `while` loop with nested `if-elif` statements | Refactored into clean, reusable functions |
| **Data Structure** | Dynamic list of expense dictionaries | Standardized dictionaries with categories & timestamps |
| **Categories** | Name-only inputs | 8 Preset categories (*Health, Education, Food, Rent, Bills, etc.*) |
| **Timestamps** | None | Automatic date (`DD/MM/YYYY`) and time (`HH:MM:SS`) logging |
| **Deletion** | Not supported | Index-based removal with explicit `(y/n)` safety confirmation |
| **Analytics** | Total spending & single largest expense | Daily spending calculator & total expenditure overview |
| **Data Persistence** | In-memory storage only | JSON file export for Top 3 largest expenses (`top_expenses.json`) |
| **Error Handling** | None (crashes on invalid numeric inputs) | `try-except` blocks for enhanced user input validation |

---

## 📁 Repository Structure

```text
.
├── expenses-tracker-v1.py   # Initial baseline implementation
├── expense-tracker-v2.py   # Upgraded modular application
├── top_expenses.json       # Generated output file for top 3 expenses (v2)
├── LICENSE                 # Proprietary / All Rights Reserved license
└── README.md               # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

* Python 3.x installed on your system.
* Standard Python libraries used (no external third-party package installation required):
  * `datetime`
  * `json`

### Running the Application

1. **Clone or Download the Repository:**
   ```bash
   git clone [https://github.com/your-username/expense-tracker.git](https://github.com/your-username/expense-tracker.git)
   cd expense-tracker
   ```

2. **Run Version 1:**
   ```bash
   python expense-tracker-v1.py
   ```

3. **Run Version 2 (Recommended):**
   ```bash
   python expense-tracker-v2.py
   ```

---

## 📖 How to Use (v2 Menu Overview)

When you run `expense-tracker-v2.py`, you will be presented with the following interactive menu:

1. **Add Expense:** Choose from 8 predefined categories, enter the amount, and auto-attach current date/time.
2. **Delete Expense:** View indexed expenses and delete a record safely after confirmation.
3. **Categorize Expense:** Filter and view recorded expenses matching a chosen category.
4. **Calculate Daily Expense:** Summarize expenditure incurred on today's date.
5. **Calculate Total Spending:** Compute total cumulative spending across all logs.
6. **Save Biggest Expense To JSON:** Automatically sort records and export top 3 expenses to `top_expenses.json`.
7. **Exit:** Terminate the program.

---
