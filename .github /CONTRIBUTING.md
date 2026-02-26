# Contributing to Titanic ETL 🛳️

Thank you for your interest in improving our data pipeline! This project is a space to practice and refine **Data Engineering** techniques. Whether you want to improve the cleaning logic or optimize the database schema, we welcome your help.

## How to Contribute

1. **Fork** the repository.
2. Create your branch: `git checkout -b feature/new-transformation`.
3. Make your changes (e.g., adding a new imputation method or a SQL view).
4. Commit your changes: `git commit -m "Add median imputation for Age column"`.
5. Push your branch: `git push origin feature/new-transformation`.
6. Open a **Pull Request**.

## 💡 Ideas for Contribution

- **Automated Extraction:** Implement a script to download the dataset automatically using the **Kaggle API**.
- **Advanced Cleaning:** Add more complex imputation techniques, such as using **IterativeImputer** or K-Nearest Neighbors for missing values.
- **Database Optimization:** Design a more normalized schema (3NF) or add **SQL Indexes** to improve query performance on the SQLite file.
- **Data Validation:** Implement a validation step using a library like **Great Expectations** to ensure the data meets quality standards before loading.
- **New Visualizations:** Expand the EDA section with interactive plots using **Plotly** or **Altair**.
- **Logging:** Add a logging system to track how many rows were extracted, transformed, and loaded in each run.



[Image of Extract Transform Load ETL process diagram]


## 🧪 Development Guidelines

- **Reproducibility First:** Any script added must be able to run from start to finish without manual data manipulation.
- **Code Style:** Follow PEP 8 for Python code and ensure your SQL queries are well-formatted.
- **Data Integrity:** If you change the transformation logic, you must verify that you are not introducing new null values or invalid data types.
- **Environment:** Use a `requirements.txt` or `environment.yml` if you add new dependencies (like `scikit-learn` or `SQLAlchemy`).
- **Minimalism:** Keep the final SQLite database as clean as possible. Only load columns that provide actual analytical value.

## 🏗️ ETL Pipeline Structure

1. **Extract:** Logic to read the CSV file.
2. **Transform:** Data cleaning, normalization, and feature selection.
3. **Load:** Schema creation and data insertion into SQLite.

Thank you for helping us build a more robust data pipeline! ⚙️📊
