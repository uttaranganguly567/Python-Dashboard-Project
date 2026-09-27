# 📱 Mobile Shop Management System

A beginner-friendly Python CRUD application for managing a mobile shop inventory — built using only core Python (lists, loops, functions) with no external libraries or databases.

---

## ✨ Features

| # | Feature | Description |
|---|---------|-------------|
| 1 | **Add Mobile** | Add a new mobile record with ID, brand, model, price, and quantity |
| 2 | **Display All Mobiles** | View all records in a formatted table |
| 3 | **Search Mobile** | Look up a mobile by its ID |
| 4 | **Update Mobile** | Edit details of an existing mobile |
| 5 | **Delete Mobile** | Remove a mobile record with confirmation prompt |
| 6 | **Exit** | Quit the application |

---

## 🗂️ Data Structure

Each mobile is stored as a plain Python list inside a global `mobiles` list:

```python
[id, brand, model, price, quantity]
```

**Example:**
```python
mobiles = [
    [101, "Samsung", "Galaxy A55", 35000, 5],
    [102, "Apple",   "iPhone 15",  65000, 3],
    [103, "OnePlus", "Nord 4",     30000, 7]
]
```

| Field | Type | Description |
|-------|------|-------------|
| `id` | `int` | Unique mobile identifier |
| `brand` | `str` | Manufacturer name |
| `model` | `str` | Model name |
| `price` | `float` | Price in ₹ |
| `quantity` | `int` | Stock count |

---

## ⚙️ CRUD Mapping

| Operation | Function | List Method Used |
|-----------|----------|-----------------|
| **C**reate | `add_mobile()` | `append()` |
| **R**ead | `display_mobiles()` | `for` loop |
| **R**ead / Search | `search_mobile()` | `for` + condition |
| **U**pdate | `update_mobile()` | Direct index assignment |
| **D**elete | `delete_mobile()` | `remove()` |

---

## 🚀 Getting Started

**Requirements:** Python 3.10+ (uses `match-case` statement)

**Run the app:**
```bash
python mobile_shop.py
```

**Sample menu:**
```
=============================================
         MOBILE SHOP MANAGEMENT
=============================================
1. Add Mobile
2. Display All Mobiles
3. Search Mobile
4. Update Mobile
5. Delete Mobile
6. Exit
=============================================
```

---

## 📂 Project Structure

```
mobile-shop-crud/
└── mobile_shop.py      # Single-file application
```

---

## ⚠️ Limitations

- Data is stored **in-memory only** — all records are lost when the program exits
- No file or database persistence
- Designed for learning purposes; not production-ready

---

## 📄 License

For educational purposes.
