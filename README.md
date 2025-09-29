# 🗄️ Database Design Project - Invoice Management System  

This repository contains our **Database Technology Final Project** at **Binus University**, focusing on designing and implementing a relational database for an **Invoice Management System**.  
The project applies **data normalization (UNF → 1NF → 2NF → 3NF)**, ERD modeling, SQL implementation, and visualization.  

---

## 👥 Team Members (Group 1)
- Aaron Lawrence (2702239763)  
- Brandon Lim Santosa (2702239391)  
- Dimas Bramantyo Putra Santoso (2702237386)  
- Ignatius Abraham Aristio Kusnadi (2702243590)  
- Kalvin (2702238804)  

**Department:** School of Computer Science  
**University:** Binus University  
**Academic Year:** 2024  

---

## 📌 Project Background
Invoices are essential in sales transactions, but poorly structured data often causes duplication, inconsistencies, and inefficiency.  
In this project, we normalized unstructured invoice data (UNF) into **3NF** to ensure:  
- ✅ Reduced data duplication  
- ✅ Improved data integrity  
- ✅ Easier data management  
- ✅ Better support for reporting & decision-making  

---

## 🎯 Objectives
- Apply **normalization** from UNF → 1NF → 2NF → 3NF.  
- Design **ERD, logical, and physical diagrams**.  
- Implement database using **MySQL**.  
- Demonstrate **SQL queries, views, and constraints**.  
- Visualize insights from the database.  

---

## 🧩 Methodology
1. **Data Collection** → 115 invoices simulated (INV001–INV115).  
2. **Unnormalized Form (UNF)** → Raw invoices stored in one table.  
3. **Normalization** → Step-by-step normalization up to 3NF.  
4. **Database Design** → ERD, logical schema, physical schema.  
5. **Implementation** → SQL scripts in MySQL.  
6. **Testing & Validation** → Queries for integrity and performance.  

---

## 🏗 Database Design

### Conceptual Diagram
![Conceptual Diagram](screenshots/Conceptual.png)  

### Logical Diagram
![Logical Diagram](screenshots/Logical.png)   

### Physical Diagram
![Physical Diagram](screenshots/Physical.png)  

**Entities:**  
- Invoice  
- Invoice_Date  
- Sales  
- Customers  
- Products  

---

## 🔎 Implementation
- Built in **MySQL**.  
- Includes **Primary Keys, Foreign Keys, Constraints**.  
- Populated with 115 simulated invoices.  
- Tested with multiple **JOIN queries** and aggregation.  

📂 Repository Structure:
