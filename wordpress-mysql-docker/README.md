
# 🐳 WordPress + MySQL using Docker Compose

<img width="1916" height="958" alt="image" src="https://github.com/user-attachments/assets/4ac3082c-0983-4619-b2ff-cd69d4abe3af" />

<img width="1919" height="989" alt="image" src="https://github.com/user-attachments/assets/7bad524c-8f69-4bb4-bb65-2570a6c3122f" />

<img width="1918" height="977" alt="image" src="https://github.com/user-attachments/assets/8f3b4f06-bd0c-44a7-bc40-cb6eb8d9105a" />


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
