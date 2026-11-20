# Natural Language Database Manager

## 📌 Project Overview

The **Natural Language Database Manager** is a Python-based application that allows users to perform database operations using simple English commands instead of writing SQL queries manually.

It uses Natural Language Processing techniques with Python regular expressions to identify user commands, convert them into SQL queries, and execute them using SQLite.

This project makes database management easier for beginners by providing a simple and user-friendly command-line interface.

## 🎯 Objectives

- To simplify database operations using English commands.
- To convert natural language instructions into SQL queries.
- To reduce the need for manual SQL coding.
- To provide an easy way to manage database records.
- To understand Python, SQLite, and regular expressions.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Database:** SQLite
- **Libraries:** 
  - `sqlite3` – Database connectivity and SQL execution.
  - `re` – Regular expression-based command processing.

## ✨ Features

The application supports the following database operations:

| Operation | Description |
|---|---|
| CREATE | Create a new database table |
| INSERT | Add new records |
| SELECT | Display all records or filtered records |
| UPDATE | Modify existing records |
| DELETE | Delete specific records |
| DROP | Permanently delete a table |
| TRUNCATE | Delete all records from a table |
| ALTER | Add a new column to an existing table |

## 📂 Project Structure

```text
Natural-Language-Database-Manager/
│
├── database_manager.py
├── database_manager.db
└── README.md
```

*Note: The database file is automatically created when the application runs for the first time.*

## ⚙️ Installation and Execution

### Step 1: Install Python

Download and install Python from:

https://www.python.org/downloads/

### Step 2: Download the Project

Clone the repository:

```bash
git clone YOUR_REPOSITORY_URL
```

### Step 3: Open the Project Folder

```bash
cd Natural-Language-Database-Manager
```

### Step 4: Run the Program

```bash
python database_manager.py
```

## 💻 Sample Commands

### 1. CREATE TABLE

```text
create table students with columns id integer, name text, age integer, mark real
```

### 2. INSERT RECORD

```text
insert student into students with id=1, name='Akshaya', age=20, mark=90.5
```

### 3. SELECT RECORDS

Display all records:

```text
show students
```

Display a specific record:

```text
show students where name is 'Akshaya'
```

### 4. UPDATE RECORD

```text
update students set mark to 95 where name is 'Akshaya'
```

### 5. DELETE RECORD

```text
delete student from students where name is 'Akshaya'
```

### 6. ALTER TABLE

```text
add column city text to students
```

### 7. TRUNCATE TABLE

```text
truncate students
```

### 8. DROP TABLE

```text
drop table students
```

**Note:** DROP and TRUNCATE operations require user confirmation before execution.

## 🔄 Working Process

1. User enters a command in simple English.
2. The application identifies the command using regular expressions.
3. The command is processed and converted into an SQL query.
4. SQLite executes the generated SQL query.
5. The application displays the database results or execution status.

## 🔐 Safety Features

- Validates table and column names.
- Uses parameterized queries for data values.
- Checks supported SQLite data types.
- Requests confirmation before destructive operations.
- Handles SQLite errors and rolls back failed transactions.

## 🚀 Future Enhancements

- Support more natural English sentence patterns.
- Add GUI-based database management.
- Implement advanced search and filtering.
- Support additional SQL operations.
- Integrate advanced Natural Language Processing techniques.

## 🎓 Project Outcome

This project demonstrates how Python can be integrated with SQLite to simplify database management through English-based commands. It provides practical experience in Python programming, database connectivity, SQL query generation, regular expressions, and exception handling.

---

**Developed as a Python and Database Management project.**
