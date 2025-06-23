# 📊Netflix Titles Dataset Cleaning Project

## 🎯 Overview
This project is a data cleaning and preprocessing task performed as part of a **Data Analyst Internship**. The dataset contains Netflix TV Shows and Movies metadata, and required cleaning to handle null values, duplicates, and inconsistent formats.

---

## 🛠️ Tools Used
- **Python 3**
- **Pandas**
- **Jupyter Notebook / Any IDE**
- No paid tools were used.

---

## 📁 Files Included
| File Name | Description |
|-----------|-------------|
| `netflix_titles.csv` | Original dataset |
| `netflix_titles_cleaned.csv` | Cleaned dataset after processing |
| `netflix_cleaning_script.py` | Python script used to clean the data |
| `README.md` | Documentation of the entire process |

---

## 🔧 Data Cleaning Steps

| Step | Category             | Action Taken |
|------|----------------------|--------------|
| 1️⃣   | Column Names         | Renamed all columns to lowercase with underscores (e.g., `date_added`) |
| 2️⃣   | Missing Values       | - Filled `director`, `cast`, `country`, `duration` with `'Unknown'`<br>- Filled `rating` with most frequent value<br>- Dropped rows with missing `date_added` |
| 3️⃣   | Duplicates           | Removed all exact duplicate rows |
| 4️⃣   | Date Format          | Converted `date_added` to `dd-mm-yyyy` format |
| 5️⃣   | Text Standardization | Standardized text fields (`type`, `country`, `rating`) with proper casing and trimmed spaces |
| 6️⃣   | Data Type Fixes      | Ensured `release_year` is of type `int` |
| 7️⃣   | Output Files         | Exported cleaned dataset and script for reproducibility |

---

## 🧾 Sample of Cleaned Data

| show_id | type    | title                 | country        | date_added | release_year | rating |
|---------|---------|-----------------------|----------------|------------|--------------|--------|
| s1      | Movie   | Dick Johnson Is Dead  | United States  | 25-09-2021 | 2020         | PG-13  |
| s2      | Tv Show | Blood & Water         | South Africa   | 24-09-2021 | 2021         | TV-MA  |
| s3      | Tv Show | Ganglands             | Unknown        | 24-09-2021 | 2021         | TV-MA  |

---

## ✅ Learning Outcomes
- Understood practical issues in real-world data (nulls, formats, duplicates)
- Gained hands-on experience with `Pandas` for cleaning and preprocessing
- Prepared dataset for downstream analysis and visualization

---

## 🗃️ How to Reproduce
1. Download `netflix_titles.csv`
2. Run `netflix_cleaning_script.py`
3. Output will be saved as `netflix_titles_cleaned.csv`

---

## 📌 Author
This task was completed as part of a **Data Analyst Internship Assignment** by [Your Name].
