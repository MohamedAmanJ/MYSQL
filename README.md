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
