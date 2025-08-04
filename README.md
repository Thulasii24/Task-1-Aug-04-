# TASKONE Database Project

This project involves the creation of a relational database named **TASKONE**, designed to manage data for departments, students, and manuals. It demonstrates core SQL concepts such as table creation, primary and foreign keys, normalization, and entity-relationship modeling using **MySQL Workbench**.

---

## Database: TASKONE

### Tables & Structure

#### Department
- `Department_id` (Primary Key)
- `Dept_Name` (Name of the department)

#### Student
- `Student_id` (Primary Key)
- `Student_Name`
- `Gender` (`ENUM('M', 'F')`)
- `Email_id` (Unique)
- `Mobile_No` (Unique)
- `Department_id` (Foreign Key → `Department.Department_id`)

#### Manuals
- `Manual_id` (Primary Key)
- `Manual_name`
- `Published_year`
- `Manual_price`
- `Department_id` (Foreign Key → `Department.Department_id`)

---

## Relationships

- Each **student** belongs to **one department**
- Each **manual** is associated with **one department**
- `Department_id` acts as a **foreign key** in both `Student` and `Manuals` tables, establishing **one-to-many** relationships from `Department`.

---

## ER Diagram

The ER diagram is designed using **MySQL Workbench** and visually represents the structure and relationships between the tables.

![ER Diagram URL](./your-er-diagram-file-name.png)

---

## Technologies Used
- SQL (MySQL)
- MySQL Workbench

---

## Author

Created by **K Thulaseeswar** as part of a database design task.

---

