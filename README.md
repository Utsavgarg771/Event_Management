README.md

# 🎉 **College Event Management System**

### *DBMS Project — Semester 3, IIIT Naya Raipur*

### **Developed By**

* **Utsav Garg**
* **Vipul Netam**
* **Eishita Mishra**

**Special thanks to *Abhishek Shrivastava Sir* for his guidance and support throughout this project.**

---

## 📘 Overview

This project is a **Java Swing + MySQL–based Event Management System** developed as part of the **DBMS course** at **IIIT Naya Raipur (Semester 3)**.

It provides an intuitive interface for:

* Managing college events
* Handling student registrations
* Performing admin-level operations

It showcases practical DBMS concepts including:

* Relational schema design
* CRUD operations using JDBC
* GUI development with Java Swing
* Integration between UI, service, and database layers

---

## ✨ Features

### 🔐 **User Authentication**

* Separate login for **Admin** and **Students**

### 🛠 **Event Management (Admin)**

* Create, update, delete events
* View events and participant lists

### 🎓 **Student Module**

* Register for events
* Update personal details
* View registered events

### 📊 **Admin Dashboard**

* Overview of all events
* Real-time participant data

---

## 🛠 Technologies Used

* **Java Swing / AWT**
* **MySQL**
* **JDBC**
* **Maven**

---

## 🚀 Getting Started

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/Utsavgarg771/Event_Management.git
cd Event_Management
```

### **2️⃣ Database Setup**

```sql
CREATE DATABASE event_management;

CREATE USER 'superadmin'@'localhost' IDENTIFIED BY 'Super@1999';
GRANT ALL PRIVILEGES ON event_management.* TO 'superadmin'@'localhost';
FLUSH PRIVILEGES;
```

Create tables:

* `events`
* `participants`

### **3️⃣ Configure Database Connection**

Edit:

```
src/main/resources/config.properties
```

Set:

```
db.url=jdbc:mysql://localhost:3306/event_management
db.username=superadmin
db.password=Super@1999
```

### **4️⃣ Build & Run**

```bash
mvn clean install
java -jar target/event-management-1.0-SNAPSHOT-jar-with-dependencies.jar
```

---

## 📂 Project Structure

```
src/main/java/com/eventmanagement/
  ├── models/
  ├── controllers/
  ├── services/
  ├── repositories/
  └── ui/
```

---

## 📸 Screenshots

### 🏠 Home Page

![Home](screenshots/version-1.0.0/home.png)

### 🔐 Admin Login

![Admin Login](screenshots/version-1.0.0/admin_login.png)

### 📝 Student Registration

![Student Registration](screenshots/version-1.0.0/student_registration.png)

### ✔ Registration Confirmation

![Confirmation](screenshots/version-1.0.0/confirm.png)

### 🎉 Success Message

![Success](screenshots/version-1.0.0/success.png)

---

## 🙏 Acknowledgment

This project was completed under the guidance of **Abhishek Shrivastava Sir**, whose insights greatly enhanced our understanding of DBMS concepts.

---

<div align="center">
  <b>Made with ❤️ by IIITNR Students</b>
</div>