Marks-Adding-Project
=====================

This is a simple Python mini-project to calculate total marks for each student from a CSV file.

How It Works:
-------------

- Reads data from a CSV file named 'marks.csv'
- Adds up marks if a student appears more than once
- Prints the total marks using a Python dictionary

Sample CSV File (marks.csv):
----------------------------

Name,Marks
Alice,50
Bob,40
Alice,30
Bob,45
Charlie,60

Expected Output:
----------------

{'Alice': 80, 'Bob': 85, 'Charlie': 60}

Python Code:
------------

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

How to Run:
-----------

1. Save the sample CSV as marks.csv in the same folder.
2. Save the Python code in a file named script.py.
3. Open terminal or command prompt.
4. Run the file using: python script.py

Author:
-------

Devansh2604
GitHub: https://github.com/devansh2604
