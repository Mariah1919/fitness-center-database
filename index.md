# 🏋️‍♀️ Fitness Center Membership Management Database

A comprehensive SQL Server database designed to automate and manage the operations of a modern fitness center.

---

## 📘 Project Overview
This project creates a **Fitness Center Membership Management System (FCMMS)** to streamline:
- Member registration and key-fob access
- Class scheduling and trainer assignment
- Equipment tracking and maintenance
- Personal fitness journals and analytics

![ER Diagram]] https://<Mariah1919>.github.io/fitness-center-database/erd
)
))

---

## 🎯 Objectives
- Collect, maintain, and update member information  
- Track retail transactions and attendance trends  
- Manage staff, classes, and personal training sessions  
- Generate predictive analytics for class popularity and equipment replacement

---

## 🧩 Database Schema
| Table | Description |
|-------|--------------|
| `person` | Tracks all members and employees |
| `fitness_class` | Stores scheduled classes |
| `class_registration` | Links members to class enrollments |
| `equipment` | Tracks gym assets and depreciation |
| `maintenance_log` | Logs inspections and repairs |
| `fitness_journal` | Logs workouts per user |
| `training_registration` | Schedules personal training |
| `equipment_category` | Categorizes gym equipment |

---

## 💡 Sample SQL
```sql
CREATE DATABASE fitness_center;

CREATE TABLE person (
    person_ID INT IDENTITY(1,1) PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    email VARCHAR(100),
    is_employee BIT
);

