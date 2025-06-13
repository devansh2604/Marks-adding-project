# Mini-Project - Marks Adding

This mini-project adds marks for students based on their roll numbers from a CSV file.

> 📂 Explore Mini Project – Marks Adding.pdf for the full assignment details.

---

## 📌 Problem Statement

Given a list of student roll numbers and their corresponding marks (which may have multiple entries per student), calculate the *total marks* obtained by each unique roll number.

---

## 📥 Input Format (CSV)

| Roll Num    | Marks |
|-------------|-------|
| 102003542   | 1     |
| 102003640   | 1     |
| 102003757   | 1     |
| ...         | ...   |

> Input file: Mini Project - Marks Adding.csv

---

## ✅ Expected Output

| Roll Num    | Marks |
|-------------|-------|
| 102003542   | 1     |
| 102003640   | 3     |
| 102003757   | 2     |
| ...         | ...   |

---

## 🧠 Logic Used

1. Read CSV using csv.reader()
2. Use a Python dictionary to store totals per roll number
3. Add marks if roll number is repeated
4. Print or export final results

---

## 🐍 Python Modules Used

- csv for file reading and parsing
- dict for aggregating marks

---

> Here's a visual representation of how input is processed into output:
![image](https://github.com/user-attachments/assets/d893755f-655d-46d8-b104-a012aea79a5f)

---

## 🚀 How to Run

1. Clone/download this repository
2. Make sure Mini Project - Marks Adding.csv is in the same folder
3. Run the Python script:

```bash
python marks_adder.py
