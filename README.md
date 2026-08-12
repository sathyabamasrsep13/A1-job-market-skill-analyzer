# Job Market Skill Analyzer

## Project Description

This project is a Python-based Job Market Skill Analyzer that analyzes skills requested in job postings.

The program can:

- Store job posting information
- Add new job postings interactively
- Clean and normalize skill data
- Extract individual skills
- Calculate skill frequency
- Find jobs based on a specific skill
- Identify jobs containing common skills
- Find unique skills
- Save cleaned job data to a CSV file
- Save top skills and their frequencies to a text file

## Dataset

```python
job_data = {
    "Job_ID": [1, 2, 3, 4, 5],
    "Role": [
        "Data Analyst",
        "Data Scientist",
        "Business Analyst",
        "Data Engineer",
        "ML Engineer"
    ],
    "Company": [
        "ABC Corp",
        "XyZ Ltd",
        "DataWorks",
        "InfraTech",
        "AI Labs"
    ],
    "Skills": [
        "Excel SQL Python",
        "Python ML Statistics",
        "Excel SQL PowerBI",
        "Python SQL Spark",
        "Python ML DeepLearning"
    ]
}

Features
1. Display Job Postings

Prints each job posting in a readable format.

Example:

ID: 1 | Role: Data Analyst | Company: ABC Corp | Skills: Excel SQL Python

2. Add New Job Postings

Users can interactively enter:

Role
Company
Skills

Job IDs are automatically incremented.

3. Clean & Normalize Skills

The clean_skills() function:

Converts skills to lowercase
Replaces commas with spaces
Removes extra spaces
Normalizes whitespace

Example:

Excel, SQL, Python

becomes:

excel sql python

4. Skill Frequency Analysis

The program extracts individual skills and calculates their frequency.

Example:

python: 4
sql: 3
excel: 2
ml: 2

5. Skill Search

The function:

find_jobs_by_skill("sql")

returns jobs containing the requested skill.

6. Unique Skills

The program creates a unique skill set and displays the skills in alphabetical order.

Example:

['deeplearning', 'excel', 'ml', 'powerbi', 'python', 'spark', 'sql', 'statistics']

7. Save Output Files

The program creates:

job_skills.csv
top_skills.txt

job_skills.csv contains cleaned and structured job records.

top_skills.txt contains the most frequently requested skills and their counts.

Technologies Used
Python
Lists
Dictionaries
Sets
Functions
Loops
Conditional Statements
Lambda Functions
filter()
List Comprehension
File Handling
CSV
Pandas
Project Files

Job-Market-Skill-Analyzer/

Job_Market_Skill_Analyzer.ipynb
job_skills.csv
top_skills.txt
README.md
How to Run
Open the Jupyter Notebook or Google Colab.
Run the cells in order.
Enter new job postings when prompted.
Analyze the skills.
The program will generate:
job_skills.csv
top_skills.txt
Sample Output

Top skills by frequency:

python: 4
sql: 3
excel: 2
ml: 2

Author

SATHYABAMA RAJARAM

Project: Job Market Skill Analyzer

Language: Python
