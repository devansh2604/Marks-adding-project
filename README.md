# 📊 Marks-Adding-Project

*A simple Python mini-project to calculate total marks per student from a CSV file.*

---

## ✅ Features

- Reads student marks from a CSV file (`marks.csv`)
- Automatically adds up marks if a student appears more than once
- Works with just built-in Python — no extra libraries needed
- Output is printed as a Python dictionary

---

## 📁 Example Input: `marks.csv`

Name,Marks
Alice,50
Bob,40
Alice,30
Bob,45
Charlie,60

yaml
Copy
Edit

---

## 📤 Output

{'Alice': 80, 'Bob': 85, 'Charlie': 60}

yaml
Copy
Edit

---

## ▶️ How to Run

1. ✅ Make sure you have Python installed (3.x version is fine)

2. ✅ Save this file as `script.py`:

```python
import csv

totalmarks = {}

with open("marks.csv", "r") as f:
    reader = csv.reader(f)
    next(reader)  # skip header

    for row in reader:
        name = row[0]
        marks = int(row[1])
        totalmarks[name] = totalmarks.get(name, 0) + marks

print(totalmarks)
✅ Place your marks.csv in the same folder.

✅ Run the script using:

bash
Copy
Edit
python script.py
💡 Use Cases
📚 School or college student data processing

📈 Simple data aggregation from spreadsheets

💻 Beginner Python project for practice

🧠 What You Learn
Reading CSV files in Python

Using dictionaries to accumulate values

File handling and looping over rows

🙌 Author
Devansh2604
📌 GitHub Profile

⭐ Show Some Love
If you liked this project, give it a ⭐ star on GitHub!

yaml
Copy
Edit

---

📌 **Now just copy this entire block**, paste it into your `README.md` file, and you're done!  
No screenshots, no issues tab, no uploading images — clean and simple. Let me know if you want to add anything else later!







