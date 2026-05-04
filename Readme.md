# 🛒 Supermarket Management System (Mini Go POS)

[![C++](https://img.shields.io/badge/Language-C++-00599C.svg?style=flat-square&logo=c%2B%2B)](https://isocpp.org/)
[![GUI](https://img.shields.io/badge/GUI-Win32_API_%7C_GDI+-lightgrey.svg?style=flat-square)](#)

This is a class project for the Object-Oriented Programming (OOP) course by students of the Electronics and Telecommunications Faculty, University of Science, VNU-HCM. 

The program is a small-scale Point of Sale (POS) software written in C++ combined with a Win32 API interface, designed to assist with basic transaction recording and inventory management tasks.

---

## 🎥 Demo Video

> **Click the image below to watch a demo video of the software's features:**

<!-- REPLACE THE LINK BELOW WITH YOUR TEAM'S YOUTUBE VIDEO LINK -->
<!-- REPLACE 'YOUR_VIDEO_ID' WITH THE ACTUAL YOUTUBE VIDEO ID TO DISPLAY THE THUMBNAIL -->
[![Demo Video](https://img.youtube.com/vi/YOUR_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)

*(Note: If you have an `.mp4` file directly in your repository, you can use the HTML tag `<video src="link-to-video.mp4" controls="controls" width="100%"></video>` instead)*

---

## ✨ Features

The application provides basic data management tools for a working shift:

- **System Management**: A Power button to turn the software on/off, including an auto-save feature for incomplete data[cite: 1].
- **Shift Management**[cite: 1]: 
  - **Open Shift**: Verify the employee and record the initial cash[cite: 1].
  - **Close Shift**: Record revenue, register cash, and calculate any discrepancies[cite: 1].
- **Sales**: Input product codes and quantities, automatically calculate the total amount, and export invoices (supports `.csv` and `.txt` files)[cite: 1].
- **Inventory Management**[cite: 1]:
  - **Import**: Record goods received from suppliers[cite: 1].
  - **Export**: Record goods removed from the inventory with specific reasons (e.g., disposal, charity, borrowing)[cite: 1].
- **Notebook**: Record events during the shift (medical issues, paperwork, taxes, etc.)[cite: 1].
- **Data Upload/Export**: Support reading input data (employee and product lists) from `.txt`/`.csv` files and manually exporting reports to a specified folder[cite: 1].

## 🛠️ Structure and Applied Technologies

The software is built with the goal of applying core Object-Oriented Programming (OOP) concepts[cite: 1]:

- **Language & Libraries**: Standard C++ and the STL library (`std::vector` for dynamic array management)[cite: 1].
- **Interface**: Built using the **Win32 API** event system and the **GDI+** library for drawing graphic logos[cite: 1].
- **Storage**: Direct reading and writing to text files (`.csv`, `.txt`) using the `<fstream>` library[cite: 1].
- **MVC-lite Architecture**: Separates the user interface code (View) from data processing (Controller/Model)[cite: 1]. The interface only receives user interactions and calls functions, without performing direct calculations[cite: 1].
- **OOP Principles**[cite: 1]:
  - **Encapsulation**: Data is strictly validated before being added to the storage array[cite: 1].
  - **Inheritance & Polymorphism**: A base `Transaction` class is built to contain a common list structure[cite: 1]. The *Sales* (`Invoice`), *Import*, and *Export* modules inherit from this class and override the `save()` function to determine their specific file writing methods, keeping the source code clean and organized[cite: 1].

## 👥 Team Members (Group 8)

This project was carried out by Group 8, class 23DTV_CLC1[cite: 1]:

| No. | Full Name | Student ID |
| :---: | :--- | :--- |
| 1 | Hồ Trọng Hải | 23207050 |[cite: 1]
| 2 | Bùi Anh Phúc | 23207094 |[cite: 1]
| 3 | Lý Anh Thư | 23207114 |[cite: 1]
| 4 | Đỗ Trường Tín | 23207135 |[cite: 1]
| 5 | Mai Lý Khải Triều | 23207136 |[cite: 1]

**Instructor:** MSc. Cao Trần Bảo Thương[cite: 1]

## 🚀 How to Install and Run

1. Clone the repository to your computer:
   ```bash
   git clone [https://github.com/HoHai23207050/mini-go-pos.git](https://github.com/HoHai23207050/mini-go-pos.git)
