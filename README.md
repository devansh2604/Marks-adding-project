# 📘 Marks-Adding-Project

A simple Python mini-project that calculates total marks for each student from a CSV file.

---

## ⚙️ How It Works

- 📂 Reads data from a CSV file named `marks.csv`
- ➕ Adds up marks if a student appears more than once
- 📊 Prints total marks using a Python dictionary

---

## 📝 Sample CSV Input (`marks.csv`)

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

## 💻 Python Code

'''python 
import csv

totalmarks = {}

with open("marks.csv", "r") as f:
    reader = csv.reader(f)
    next(reader)  # Skip header
    for row in reader:
        name = row[0]
        marks = int(row[1])
        totalmarks[name] = totalmarks.get(name, 0) + marks

print(totalmarks)
▶️ How to Run
✍️ Save the CSV data into a file named marks.csv

💾 Save the code above into a file called script.py

🖥️ Run the script:

nginx
Copy
Edit
python script.py
🧠 What You'll Learn
📑 Reading CSV files using Python

🧮 Summing values using dictionaries

📁 File handling basics

👤 Author
Devansh2604
🔗 GitHub: https://github.com/devansh2604

⭐ Support
If you like this project, please give it a ⭐ on GitHub!
