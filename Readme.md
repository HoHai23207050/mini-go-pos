# 🛒 Supermarket Management System (Mini Go POS)

[![C++](https://img.shields.io/badge/Language-C++-00599C.svg?style=flat-square&logo=c%2B%2B)](https://isocpp.org/)
[![GUI](https://img.shields.io/badge/GUI-Win32_API_%7C_GDI+-lightgrey.svg?style=flat-square)](#)

This is a class project for the Object-Oriented Programming (OOP) course by students of the Electronics and Telecommunications Faculty, University of Science, VNU-HCM. 

The program is a small-scale Point of Sale (POS) software written in C++ combined with a Win32 API interface, designed to assist with basic transaction recording and inventory management tasks.

---

## 🎥 Demo Video

> **Click the image below to watch a demo video of the software's features:**

[![Demo Video](https://img.youtube.com/vi/BgR5ysIELhw/maxresdefault.jpg)](https://youtu.be/BgR5ysIELhw)



---

## ✨ Features

The application provides basic data management tools for a working shift:

- **System Management**: A Power button to turn the software on/off, including an auto-save feature for incomplete data.
- **Shift Management**: 
  - **Open Shift**: Verify the employee and record the initial cash.
  - **Close Shift**: Record revenue, register cash, and calculate any discrepancies.
- **Sales**: Input product codes and quantities, automatically calculate the total amount, and export invoices (supports `.csv` and `.txt` files).
- **Inventory Management**:
  - **Import**: Record goods received from suppliers.
  - **Export**: Record goods removed from the inventory with specific reasons (e.g., disposal, charity, borrowing).
- **Notebook**: Record events during the shift (medical issues, paperwork, taxes, etc.).
- **Data Upload/Export**: Support reading input data (employee and product lists) from `.txt`/`.csv` files and manually exporting reports to a specified folder.

## 🛠️ Structure and Applied Technologies

The software is built with the goal of applying core Object-Oriented Programming (OOP) concepts:

- **Language & Libraries**: Standard C++ and the STL library (`std::vector` for dynamic array management).
- **Interface**: Built using the **Win32 API** event system and the **GDI+** library for drawing graphic logos.
- **Storage**: Direct reading and writing to text files (`.csv`, `.txt`) using the `<fstream>` library.
- **MVC-lite Architecture**: Separates the user interface code (View) from data processing (Controller/Model). The interface only receives user interactions and calls functions, without performing direct calculations.
- **OOP Principles**:
  - **Encapsulation**: Data is strictly validated before being added to the storage array.
  - **Inheritance & Polymorphism**: A base `Transaction` class is built to contain a common list structure. The *Sales* (`Invoice`), *Import*, and *Export* modules inherit from this class and override the `save()` function to determine their specific file writing methods, keeping the source code clean and organized.

## 👥 Team Members (Group 8)

This project was carried out by Group 8, class 23DTV_CLC1:

| No. | Full Name | Student ID |
| :---: | :--- | :--- |
| 1 | Hồ Trọng Hải | 23207050 |
| 2 | Bùi Anh Phúc | 23207094 |
| 3 | Lý Anh Thư | 23207114 |
| 4 | Đỗ Trường Tín | 23207135 
| 5 | Mai Lý Khải Triều | 23207136 

**Instructor:** MSc. Cao Trần Bảo Thương

## 🚀 How to Install and Run

1. Clone the repository to your computer:
   ```bash
   git clone [https://github.com/HoHai23207050/mini-go-pos.git](https://github.com/HoHai23207050/mini-go-pos.git)
