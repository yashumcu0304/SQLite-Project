#  Restaurant Food Ordering System (SQLite + Python)

This project implements a complete **Restaurant Food Ordering System** using **SQLite** and **Python**.  
The goal of the system is to simulate a realistic food-delivery workflow similar to platforms like Uber Eats and to create a clean, normalized relational database suitable for SQL queries, analysis, and academic coursework.

All data in the database was generated programmatically using Python, ensuring:
- realistic order behaviour  
- consistent foreign key relationships  
- controlled randomness for reproducibility  
- properly structured table relationships  

The project demonstrates skills in **database design**, **data engineering**, **synthetic data generation**, and **SQL validation**.

---

##  Project Overview

The system models the full lifecycle of a food-ordering platform through multiple interconnected tables.  
The database captures:

- Customer registration and demographic details  
- Restaurant information including cuisine, city, and ratings  
- Delivery partner details with vehicle type and performance rating  
- Restaurant menu catalogues with pricing and categories  
- Complete order-level information with timestamps, fees, discounts  
- Item-level order details using a **compound primary key**  
- Payment transactions including methods and settlement statuses  

All relationships were implemented using **foreign keys**, and the database structure ensures **3NF normalization**, with no redundancy and full analytical usability.

---

##  Technologies Used

- **SQLite** (Database Engine)  
- **Python 3**  
  - `sqlite3` (database operations)  
  - `random` (synthetic data generation)  
  - `datetime` (dates and timestamps)  
- **Jupyter Notebook**  
- **DB Browser for SQLite** (validation and visual inspection)

---

##  Key Features

- Fully normalized, well-structured relational database  
- Seven core tables linked through **primary and foreign keys**  
- **Compound primary key** in `order_items`  
- Realistic synthetic dataset created entirely in Python  
- Includes **nominal, ordinal, interval, and ratio** data types  
- Ensures full referential integrity with `PRAGMA foreign_keys = ON`  
- Clean, well-commented Python notebook divided into logical cells  
- Suitable for academic submission, SQL learning, and analytics practice  

---

##  Final Table Row Counts

After successful execution of the Python notebook, the final generated dataset contains:

| Table Name            | Row Count |
|-----------------------|----------:|
| restaurants           | 12        |
| customers             | 600       |
| delivery_partners     | 80        |
| menu_items            | 267       |
| orders                | 1200      |
| order_items           | 3607      |
| payments              | 1095      |

These row counts confirm that:
- all foreign keys were respected  
- all tables were populated correctly  
- the system generated a large, realistic dataset suitable for analysis  

---

##  Files Included

- **Restaurant_Food_Ordering_System.ipynb**  
  → Complete Python code for schema creation, data generation, and validation  
- **Restaurant_Food_Ordering_System_UberEats.db**  
  → Final SQLite database with fully populated tables  
- **screenshots/** *(optional)*  
  → Screenshots from DB Browser for SQLite (table previews, row counts, queries)  
- **README.md**  
  → Project documentation (this file)

---

##  Appendix (Optional)

A separate screenshots/ folder may contain:
- Database structure view  
- Sample data previews  
- SQL query outputs  
- Row count validation  
- Schema inspection screenshots  

These were used to verify correctness and support academic documentation.

---

##  Author

**Yasaswini Sure**  
*MSc Data Science Student*

This project was developed as part of my academic learning journey in data engineering, Python programming, and relational database design.  
It reflects my ability to build full end-to-end data systems, generate realistic datasets, and validate them using SQL.
