# Vegan Store Management — Python CLI Application

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white)
![OOP](https://img.shields.io/badge/Design-OOP-green)
![JSON](https://img.shields.io/badge/Persistence-JSON-lightgrey)

## Overview

Command-line application for managing a vegan product store: product catalogue, sales registration, stock control, and profit reporting.
Built with a focus on **clean code organisation**, **data persistence**, and **robust input validation** — demonstrating solid Python fundamentals and OOP design in a real-world CRUD context.

---

## Features

| Feature | Description |
|---------|-------------|
| Product registration | Add products with name, quantity, purchase price, sell price |
| Product listing | Full catalogue view with current stock levels |
| Sales recording | Log transactions, auto-update stock quantities |
| Stock validation | Alert if requested quantity exceeds available stock |
| Stock replenishment | Add stock to existing product without re-entering prices |
| Gross profit | Total sales revenue calculation |
| Net profit | Revenue minus purchase cost of sold goods |
| Data persistence | State saved to `db.json` between sessions |
| Input validation | Numeric checks with error recovery on all inputs |

---

## Usage

```bash
git clone https://github.com/sylver86/18-vegan-store-management-python.git
cd 18-vegan-store-management-python
python main.py
```

**Interactive menu:**
```
=== VEGAN STORE MANAGEMENT ===
1. Add product
2. List products
3. Register sale
4. Show gross profit
5. Show net profit
0. Exit
```

Data is automatically persisted to `db.json` after each operation.

---

## Code Structure

```
18-vegan-store-management-python/
├── main.py        # Entry point — CLI menu and main loop
├── db.json        # JSON persistence file (auto-created)
└── README.md
```

**Design highlights:**
- Functions separated by single responsibility (product management, sales, reporting)
- Dictionary + list data structures for in-memory catalogue
- JSON serialisation for cross-session persistence
- Try/except blocks on all numeric inputs with user-friendly error messages

---

## Technologies

`Python 3.8+` · `JSON` · `OOP` · `CLI`
