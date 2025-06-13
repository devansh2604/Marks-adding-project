# 📊 Marks-Adding-Project

*A simple Python mini-project to calculate total marks per student from a CSV file.*

---

## ✅ Features

- Reads student marks from a CSV file (`marks.csv`)
- Automatically adds marks if a student appears multiple times
- Prints total marks using Python dictionary
- Beginner-friendly project — only built-in libraries used

---

## 📁 Sample CSV Input

Name,Marks  
Alice,50  
Bob,40  
Alice,30  
Bob,45  
Charlie,60

---

## 📤 Output

{'Alice': 80, 'Bob': 85, 'Charlie': 60}

---

## ▶️ How to Run

### 1. Create a CSV file named `marks.csv` in the same folder:

Name,Marks
Alice,50
Bob,40
Alice,30
Bob,45
Charlie,60

kotlin
Copy
Edit

### 2. Copy and save this Python code as `script.py`:

import csv

totalmarks = {}

with open("marks.csv", "r") as f:
reader = csv.reader(f)
next(reader) # skip header

sql
Copy
Edit
for row in reader:
    name = row[0]
    marks = int(row[1])
    totalmarks[name] = totalmarks.get(name, 0) + marks
print(totalmarks)

bash
Copy
Edit

### 3. Run the script:

Open terminal or command prompt and type:

python script.py

yaml
Copy
Edit

---

## 🧠 What You Learn

- Reading CSV files with `csv.reader`
- Using dictionaries to sum data
- Basic file handling in Python

---

## 🙌 Author

**Devansh2604**  
[Visit my GitHub →](https://github.com/devansh2604)

---

## ⭐ Like this?

If you liked this mini project, please give it a ⭐ star on GitHub to support!

