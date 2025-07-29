# 🇮🇳 Indian Crime Data Analysis with SQL

This project explores patterns and trends in crime data reported across major Indian cities using **SQL Server (T-SQL)**. The dataset includes incident-level records from 2020 to 2024, detailing crime types, locations, times, victim profiles, and police response.

---

## 📦 Dataset

- **Source:** [Kaggle - Indian Crimes Dataset](https://www.kaggle.com/datasets/sudhanvahg/indian-crimes-dataset/data)
- **Size:** ~40,000+ records
- **Columns include:**
  - `Report_Number`
  - `Date_Reported`, `Date_of_Occurrence`, `Time_of_Occurrence`
  - `City`, `Crime_Code`, `Crime_Description`
  - `Victim_Age`, `Victim_Gender`
  - `Weapon_Used`, `Crime_Domain`
  - `Police_Deployed`, `Case_Closed`, `Date_Case_Closed`

---

## 🧰 Tools Used

- **SQL Server Management Studio (SSMS)**
- **T-SQL** for querying, aggregation, and analysis

---

## 🔎 Analysis Objectives

This project focuses on exploring:
- Total crime reports by city
- Most common types of crimes
- Crime distribution over time (planned)
- Victim demographics (age, gender) and crime type (planned)
- Closure rates and police deployment patterns (planned)

---

## 📌 Sample Queries

```sql
-- Total crimes reported per city
SELECT City, COUNT(*) AS Total_Crimes
FROM crime_dataset_india
GROUP BY City
ORDER BY Total_Crimes DESC;

-- Most frequent crime types
SELECT Crime_Description, COUNT(*) AS Crimes
FROM crime_dataset_india
GROUP BY Crime_Description
ORDER BY Crimes DESC;
```

---

## 🚧 Work in Progress

✅ Data imported and cleaned  
✅ Initial queries written  
🔜 Trend analysis by time and city  
🔜 Crime rate per 1000 population (with external data)  
🔜 Comparative rural vs urban crime analysis (future enrichment)  

---

## 🧠 What I’m Practicing

- Writing efficient SQL queries  
- Data aggregation and pattern discovery  
- Using GROUP BY, COUNT, DATEPART, CASE, and more  
- Exploring real-world data in a structured way  

---

## 📁 Project Structure

📦 crime-sql-analysis  
├── crime_dataset_india.sql         -- Raw table creation and import  
├── queries/  
│   ├── crime_summary_queries.sql   -- Initial exploratory queries  
│   └── time_analysis_queries.sql   -- (planned)  
└── README.md  

---

## 🙋‍♀️ About Me

This is part of my learning journey to deepen my SQL skills through real-world datasets.  
I’m currently working on more analyses and improvements—stay tuned!
