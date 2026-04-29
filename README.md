# 🐳 INT332 Docker Practicals

This repository contains Docker-based practicals covering containerization, database setup, and multi-container applications using Docker Compose.

---

## 📁 Practicals Included

### 1️⃣ Dockerized MySQL Setup

Demonstrates how to run and manage a MySQL database using Docker.

📂 Location: `mysql-docker/` *(or root if kept there)*

---

### 2️⃣ WordPress + MySQL (Docker Compose)

Demonstrates a real-world multi-container application using WordPress and MySQL.

📂 Location: `wordpress-mysql-docker/`

---

# 🧩 Practical 1: Dockerized MySQL Setup

## 📌 Overview

This practical demonstrates how to provision and run a MySQL database using Docker and interact with it via the MySQL command-line client.

---

## ⚙️ Prerequisites

* Docker installed and running
* Basic knowledge of command line

---

## 🚀 Setup Instructions

### 1. Pull MySQL Image

```
docker pull mysql:latest
```

### 2. Run MySQL Container

```
docker run -it \
  --name my-db \
  -e MYSQL_ROOT_PASSWORD=<your_password> \
  mysql:latest
```

### 3. Access Running Container

```
docker exec -it my-db bash
```

### 4. Connect to MySQL Server

```
mysql -u root -p
```

---

## 🗄️ Database Operations

* Created database
* Created table
* Inserted records
* Queried data

---

## ⚠️ Common Issues & Fixes

### ❌ Invalid Flag

* Error: `unknown flag: --it`
* Fix: Use `-it`

### ❌ Wrong Image Name

* Error: `pull access denied for myaql`
* Fix: Use `mysql`

### ❌ SQL Errors

* Always terminate queries with `;`
* Execute queries one by one

---

## 📊 Sample Output

```
SELECT * FROM lect_1;

+------+
| name |
+------+
| 101  |
+------+
```

---

## 📚 Key Learnings

* Docker container lifecycle
* `docker run` vs `docker exec`
* Running databases in containers
* SQL basics

---




# 🧩 Practical 2: WordPress + MySQL (Docker Compose)

<img width="1919" height="995" alt="image" src="https://github.com/user-attachments/assets/ea3a82f0-47a0-4c9c-a318-cfab2577701e" />

<img width="1919" height="978" alt="image" src="https://github.com/user-attachments/assets/eb6c6684-0e7c-44a4-b4af-421a184ba1c6" />

<img width="1919" height="986" alt="image" src="https://github.com/user-attachments/assets/58efe91f-df7b-4cea-a2fa-d7261eaa98ae" />




## 📌 Overview

This practical demonstrates a multi-container application using Docker Compose with WordPress and MySQL.

---

## 🏗️ Architecture

* WordPress (Frontend + PHP + Apache)
* MySQL (Database)
* Docker Bridge Network
* Named Volumes for persistence

---

## 🚀 Run Project

```
docker compose up -d
```

---

## 🌐 Access

```
http://localhost:8080
```

---

## 🔑 Key Concepts

* Multi-container deployment
* Service-to-service communication
* Docker networking
* Volume-based persistence
* Health checks

---

## 🧠 Summary

WordPress runs in one container and connects to MySQL in another using Docker's internal network. Data is persisted using volumes.

---

# 🔮 Future Enhancements

* Add more Docker-based practicals
* Integrate with MERN stack
* Deploy using Docker Swarm / Kubernetes

---

# 👨‍💻 Author
**Tek Narayan**






