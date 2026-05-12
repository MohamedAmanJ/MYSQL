# SQL Patient Records Analysis Project

## 📌 Project Overview
This project contains SQL queries performed on a hospital patient management database.  
The queries are used for data analysis, filtering, aggregation, joins, grouping, and reporting using SQL.

The database includes tables such as:
- patients
- admission
- doctors
- province_names

---

## 🛠️ Skills Used
- SQL
- Data Filtering
- Joins
- Aggregate Functions
- Group By & Having
- Sorting & Ordering
- CASE Statements
- Data Cleaning
- String Functions

---

## 📊 Key SQL Operations Performed

### ✅ Basic Queries
- Fetch male patients
- Find patients without allergies
- Filter names using LIKE
- Find patients within weight range

### ✅ Data Cleaning
- Replace NULL allergies with `NKA`

### ✅ String Functions
- Concatenate full names
- Convert names to uppercase/lowercase

### ✅ Joins
- Joined patients with province names
- Joined admissions with doctors and patients

### ✅ Aggregate Functions
- Count admissions
- Count male & female patients
- Find max/min values
- Calculate grouped totals

### ✅ Advanced SQL
- GROUP BY & HAVING
- CASE statements for obesity classification
- DISTINCT filtering
- Date filtering and extraction
- Weight grouping analysis

---

## 📁 Sample Queries Included

### Example 1: Male Patients
```sql
SELECT first_name, last_name, gender
FROM patients
WHERE gender = 'M';
```

Example 2: Full Name Concatenation
```sql
SELECT CONCAT(first_name, ' ', last_name) AS full_name
FROM patients;
```

Example 3: Obesity Classification
```sql
SELECT 
    patient_id,
    weight,
    height,
    CASE 
        WHEN weight / POWER(height / 100.0, 2) >= 30 THEN 1
        ELSE 0
    END AS isObese
FROM patients;
```

📈 Concepts Practiced
SELECT
WHERE
BETWEEN
LIKE
IN
ORDER BY
GROUP BY
HAVING
INNER JOIN
UNION
CASE
Aggregate Functions
🚀 Purpose of This Project

This project was created to strengthen practical SQL skills for Data Analyst roles by solving real-world healthcare database problems.

👨‍💻 Author

Mohamed Amaan
Aspiring Data Analyst skilled in Python, SQL, Excel, and Power BI.
