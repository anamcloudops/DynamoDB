# 🎓 AWS DynamoDB Student Management System

> 🚀 A simple and practical **AWS Cloud project** for managing student records using **Amazon DynamoDB**.

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge\&logo=amazonaws)
![DynamoDB](https://img.shields.io/badge/Amazon-DynamoDB-blue?style=for-the-badge\&logo=amazondynamodb)
![Database](https://img.shields.io/badge/Database-NoSQL-green?style=for-the-badge)
![Project](https://img.shields.io/badge/Project-Cloud%20Computing-purple?style=for-the-badge)

---

## 📌 Project Overview

The **AWS DynamoDB Student Management System** is a cloud-based student record management project built using **Amazon DynamoDB**, a fully managed NoSQL database service provided by AWS.

The project demonstrates how student information can be stored and managed efficiently in a scalable cloud database.

It performs the basic **CRUD operations**:

* ➕ **Create** – Insert new student records
* 🔍 **Read** – Retrieve student information
* ✏️ **Update** – Modify existing student details
* 🗑️ **Delete** – Remove student records

This project is designed to demonstrate practical knowledge of **AWS DynamoDB, NoSQL databases, tables, partition keys, and database operations**.

---

## 🏗️ Architecture

```text
             👤 User
                │
                ▼
        ☁️ AWS Management Console
                │
                ▼
      ┌──────────────────────┐
      │   Amazon DynamoDB    │
      │                      │
      │  📋 Students Table   │
      └──────────────────────┘
                │
                ▼
        🎓 Student Records
```

### 🔑 Database Flow

```text
User
  │
  ├── ➕ Insert Student
  │
  ├── 🔍 Retrieve Student
  │
  ├── ✏️ Update Student
  │
  └── 🗑️ Delete Student
          │
          ▼
   Amazon DynamoDB
```

---


## 📋 Database Design

### Table Name

```text
Students
```

### 🔑 Partition Key

```text
StudentID
```

### Data Type

```text
String
```

### 📊 Attributes

| Attribute    | Description               |
| ------------ | ------------------------- |
| 🆔 StudentID | Unique student identifier |
| 👤 Name      | Student name              |
| 🎓 Course    | Student's course          |
| 📍 City      | Student's city            |

---

## 🗂️ Sample Student Records

### 👨‍🎓 Student 1

```text
StudentID : S101
Name      : Anam
Course    : MScIT
City      : Chiplun
```

### 👩‍🎓 Student 2

```text
StudentID : S102
Name      : Ayesha
Course    : BScIT
City      : Mumbai
```

---

# ⚙️ Project Implementation

## 1️⃣ Create DynamoDB Table

Open the **AWS Management Console** and navigate to:

```text
AWS Console
     ↓
DynamoDB
     ↓
Tables
     ↓
Create Table
```

Enter:

```text
Table Name : Students
Partition Key : StudentID
Data Type : String
```

Then click:

```text
Create Table
```

---

# 2️⃣ ➕ Insert Student Record

After creating the table:

```text
Students
   ↓
Explore table items
   ↓
Create item
```

Add the following item:

```text
StudentID : S101
Name      : Anam
Course    : MScIT
City      : Chiplun
```

Create another student:

```text
StudentID : S102
Name      : Ayesha
Course    : BScIT
City      : Mumbai
```

---

# 3️⃣ 🔍 Retrieve Student Record

To retrieve a student:

```text
Students
   ↓
Explore table items
   ↓
Search / Retrieve
```

Use:

```text
StudentID = S101
```

DynamoDB retrieves the corresponding student record.

### Expected Result

```text
StudentID : S101
Name      : Anam
Course    : MScIT
City      : Chiplun
```

---

# 4️⃣ ✏️ Update Student Record

Select:

```text
StudentID = S101
```

Edit the student's city.

### Before

```text
City : Chiplun
```

### After

```text
City : Pune
```

The updated record becomes:

```text
StudentID : S101
Name      : Anam
Course    : MScIT
City      : Pune
```

---

# 5️⃣ 🗑️ Delete Student Record

Select:

```text
StudentID = S102
```

Choose:

```text
Delete
```

Confirm the deletion.

The student record is removed from the DynamoDB table.

---

📸 Screenshots

![](./Screenshot%202026-10-01%20154022.png)

![](./Screenshot%202026-10-01%20155008.png)

![](./Screenshot%202026-10-01%20155322.png)

![](./Screenshot%202026-10-01%20155344.png)