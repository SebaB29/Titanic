# 🛳️ Titanic Data Engineering: ETL Pipeline

A comprehensive Data Engineering project focused on the **ETL (Extract, Transform, Load)** process. This repository demonstrates how to take raw, inconsistent data from the classic Titanic dataset and transform it into a clean, normalized SQLite database ready for professional analysis and SQL querying.



# 📸 Overview
Data is rarely clean. This project tackles real-world data issues—such as missing values, redundant features, and duplicate records—by implementing a robust pipeline that ensures data integrity and consistency before storage.

# 📍 Table of Contents
- [📝 Description](#-description)
  - [🎯 Project Objectives](#-project-objectives)
  - [🛠️ ETL Workflow](#️-etl-workflow)
- [🔍 Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [🏗️ Transformation Logic](#️-transformation-logic)
- [🛠️ Technologies](#️-technologies)
- [👥 Team Members](#-team-members)
- [📄 License](#-license)

---

# 📝 Description
Developed for the **Database (TA044)** course, this project implements a full ETL lifecycle. We utilized the Titanic dataset (Kaggle) to practice data cleaning techniques and schema design, culminating in the loading of refined data into an **SQLite** relational database.

## 🎯 Project Objectives
- Build a functional ETL pipeline from scratch.
- Resolve data quality issues (nulls, duplicates, inconsistent types).
- Design and populate a relational database schema optimized for SQL queries.

## 🛠️ ETL Workflow
1. **Extract:** Pulling raw CSV data from Kaggle sources.
2. **Transform:** Applying cleaning logic using Python and Pandas.
3. **Load:** Exporting the final structured data into an SQLite engine.



---

# 🔍 Exploratory Data Analysis (EDA)
Before transformation, an exhaustive EDA was performed to understand the data's health:
- **Null Analysis:** Identified critical gaps in columns like `age` and `deck`.
- **Distribution Check:** Visualized age ranges per gender using boxplots.
- **Redundancy Audit:** Spotted overlapping columns that provided no additional information.

---

# 🏗️ Transformation Logic
Key engineering decisions made during the process:
- **Feature Selection:** Dropped redundant columns (`male`, `class`) and high-null columns (`deck`).
- **Smart Imputation:** Filled missing `age` values using the mean average calculated by gender groups.
- **De-duplication:** Removed duplicate records while preserving an occurrence count to maintain data history.
- **Normalization:** Standardized formats to ensure the SQLite schema constraints were met.

---

# 🛠️ Technologies
- **Language:** Python 3.x
- **Data Manipulation:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Database:** SQLite
- **Environment:** Jupyter Notebook / Python Scripts

---

# 👥 Team Members
| Name |
| :--- |
| **Sebastián Brizuela** |
| **Victoria Avalos** |
| **Gonzalo Manuel Calderón** |
| **Mateo Liberini** |
| **Franco Agustín Rodriguez** |
| **Urbano Sol Guadalupe** |

---

# 📄 License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
