# 🗂️ Event Management SQL Project

## 📌 Overview

This project demonstrates advanced SQL querying techniques on an event management database. It models real-world scenarios where organizations track events, assign managers, and analyze event durations, workloads, and scheduling patterns.

The project involves designing a normalized schema, inserting data, and solving analytical business queries using **MySQL**.

---

## 🛠 Tech Stack

- **Database**: MySQL 8+
- **Tools Used**: MySQL Workbench
- **Concepts**: 
  - CTEs
  - Window Functions
  - Date Functions
  - Aggregations
  - Conditional Logic

---

## 🗃️ Database Schema

- **`events`**: Stores event information (name, start date, end date)
- **`managers`**: Stores manager details
- **`event_manager`**: Bridge table for many-to-many relationship between events and managers

---

## EER Diagram

![image](https://github.com/user-attachments/assets/d12bd0e1-359b-42ad-af7e-06ed473127aa)

---

## 🧪 Sample Data
Includes 20 events across 2024 and 5 managers with a realistic mix of short and long events, single and multiple manager assignments.

---

## 🔍 Business Queries

### 1.  Events with Duration Significantly Above Average
- Lists events that exceed the **average event duration**.
- Shows duration and how many days above average.

### 2.  Managers Overseeing Events on the Same Day
- For each event day, shows:
  - Number of **distinct managers**
  - **List of events** held on that date

### 3.  Managers NOT Managing Events Between May–July 2024
- Lists managers with **no events between 2024-05-01 and 2024-07-31**
- Includes **event count managed outside** this date range

### 4.  Event Duration Categories
- Categorizes events as:
  - **Short** (<3 days)
  - **Medium** (3–5 days)
  - **Long** (>5 days)

### 5.  Total Event Days per Manager
- Calculates how many **total event days** each manager is responsible for.

### 6.  Managers Managing Multiple Events in the Same Month
- Identifies managers overseeing **2+ events in the same month**

### 7.  Events Not Assigned to Any Manager
- Lists events that have **no manager assigned**

---

## 📁 Project Structure

