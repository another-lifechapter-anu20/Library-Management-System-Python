# 📚 Library Management System

A command-line library management system built with **Python OOP**. Demonstrates abstract base classes, inheritance, polymorphism, and magic methods.

## 🎯 Project Purpose

This project demonstrates Object-Oriented Programming concepts in Python:

| Concept | Implementation |
|---------|----------------|
| **Abstract Base Classes** | `LibraryItem` ABC enforcing `get_item_type()`, `get_max_borrow_days()`, `get_fine_per_day()` |
| **Inheritance** | `Book`, `Magazine`, `DVD` inheriting from `LibraryItem` |
| **Polymorphism** | Same methods (`borrow()`, `return_item()`) with different behaviors per item type |
| **Magic Methods** | `__str__`, `__len__`, `__getitem__`, `__contains__`, `__iter__` |
| **Encapsulation** | Private attributes with controlled access |

## 🚀 Features

| Feature | Description |
|---------|-------------|
| 📖 **Item Management** | Add Books, Magazines, and DVDs with different borrow periods |
| 👥 **Member Management** | Register, remove, and track borrowed items for members |
| 🔄 **Borrow/Return** | Complete transaction system with overdue calculation |
| 🔍 **Search** | Find items by title, author, or ID |
| 💰 **Fine System** | Automatic fine calculation for overdue returns |
| 📜 **Transaction History** | Complete log of all library activities |
| 📊 **Reports** | View summary statistics and system status |

## 📁 Class Structure

```
LibraryItem (ABC)
    ├── Book
    ├── Magazine
    └── DVD
Member
Transaction
Library (main system)
```

## 💻 Installation

```bash
# No external dependencies - only Python standard library
git clone https://github.com/yourusername/Library-Management-System-Python.git
cd Library-Management-System-Python
python library_system.py
```

## 🚀 Run on Google Colab

1. Open [colab.research.google.com](https://colab.research.google.com)
2. Upload `Library_Management_System.ipynb`
3. Click **Runtime** → **Run all**

## 🛠️ Technologies

| Technology | Usage |
|------------|-------|
| Python 3 | Core language |
| ABC Module | Abstract base classes |
| Datetime | Due date and fine calculation |
| UUID | Unique identifiers for items |
| Magic Methods | `__str__`, `__len__`, `__getitem__`, `__contains__` |

## 📖 Usage Examples

```python
# Create a library
library = Library()

# Add items
book = Book("The Alchemist", "Paulo Coelho", 248)
library.add_item(book)

# Register member
library.add_member("Anupreet", "anupreet@example.com")

# Borrow item
library.borrow_item(member_id, item_id, borrow_days=14)

# Return item (calculates fine if overdue)
library.return_item(member_id, item_id)

# Search items
library.search_items("Alchemist")

# View report
library.get_summary_report()
```

## 🔧 Future Enhancements

- [ ] JSON/CSV data persistence
- [ ] GUI with Tkinter
- [ ] Email notifications for overdue items
- [ ] Web API with Flask
- [ ] Database integration (SQLite)

## 📄 License

MIT License

## 👨‍💻 Author

**Anupreet Kaur**
 [Linkedin Profile](www.linkedin.com/in/anupreet-kaur-26curiousmind)


## 📅 Date Created

June 2026

