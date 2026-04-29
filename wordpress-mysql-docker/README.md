
# 🐳 WordPress + MySQL using Docker Compose

## 📌 Overview
This project demonstrates a multi-container Docker setup using WordPress and MySQL.

---

## 🏗️ Architecture
- WordPress (Frontend + PHP + Apache)
- MySQL (Database)
- Docker Bridge Network for communication
- Named Volumes for data persistence

---

## ⚙️ Setup Instructions

### 1. Start Services
docker compose up -d

### 2. Check Running Containers
docker compose ps

### 3. View Logs
docker compose logs -f

---

## 🌐 Access Application
http://localhost:8080

---

## 🔑 Configuration

- Database Host: db
- Database Name: wordpress_db
- Username: wp_user
- Password: wp_pass123

---

## 📦 Volumes

- mysql_data → stores database files
- wp_content → stores WordPress content

---

## 🔍 Key Concepts Learned

- Multi-container deployment
- Service-to-service communication
- Docker networking
- Data persistence using volumes
- Health checks & dependencies

---

## 🧠 Viva Summary

WordPress runs in one container and connects to MySQL in another container using the service name as hostname via Docker network. Data is persisted using named volumes.

---

## 👨‍💻 Author
Tek Narayan
