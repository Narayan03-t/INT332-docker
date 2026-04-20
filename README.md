# 🐳 Dockerized MySQL Setup

## 📌 Overview

This repository demonstrates how to provision and run a MySQL database using Docker, and interact with it via the MySQL command-line client. It covers container creation, database initialization, and basic SQL operations.

---

## ⚙️ Prerequisites

* Docker installed and running
* Basic understanding of command-line interface

---

## 🚀 Setup Instructions

### 1. Pull MySQL Image

```bash
docker pull mysql:latest
```

### 2. Run MySQL Container

```bash
docker run -it \
  --name my-db \
  -e MYSQL_ROOT_PASSWORD=<your_password> \
  mysql:latest
```

### 3. Access Running Container

```bash
docker exec -it my-db bash
```

### 4. Connect to MySQL Server

```bash
mysql -u root -p
```

---

## 🗄️ Database Operations

The following operations were performed inside the MySQL shell:

* Created a new database
* Switched to the database
* Created a table
* Inserted records
* Queried data

---

## ⚠️ Common Issues & Resolutions

### 1. Invalid Flag Usage

**Issue:**

```
unknown flag: --it
```

**Resolution:**
Use `-it` instead of `--it`.

---

### 2. Incorrect Image Name

**Issue:**

```
pull access denied for myaql
```

**Resolution:**
Ensure the correct image name is used: `mysql`.

---

### 3. SQL Syntax Errors

**Issue:** Multiple SQL statements executed without proper termination.

**Resolution:**

* Terminate each SQL statement with `;`
* Execute statements individually
* Ensure proper syntax for INSERT and CREATE queries

---

## 📊 Sample Query Output

```sql
SELECT * FROM lect_1;

+------+
| name |
+------+
| 101  |
+------+
```

---

## 📚 Key Learnings

* Container lifecycle management using Docker
* Difference between `docker run` and `docker exec`
* Running database services inside containers
* Importance of SQL syntax and execution order

---

## 🔮 Future Enhancements

* Configure Docker volumes for persistent storage
* Expose MySQL port for external connections
* Integrate with backend applications (Node.js / MERN)
* Use Docker Compose for multi-container orchestration

---

## 👨‍💻 Author

Tek Narayan
