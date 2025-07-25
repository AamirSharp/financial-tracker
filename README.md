# Anask’s Financial and Inventory Management System

A full-stack desktop application built using Java and MySQL to help a small clothing business manage its inventory and finances. Developed as part of the IB Computer Science Internal Assessment (IA), the app includes secure login, inventory tracking, expense/revenue logging, and PDF report export.

---

## 🧩 Features

- 🔐 Secure Login / Registration System  
- 📦 Inventory Management (Add/Edit/Delete Items)  
- 💰 Finance Tracker (Income, Expenses, Profit Calculation)  
- 📄 Export Reports to PDF (via iText)  
- 🌙 Dark Mode UI  
- ✅ Input validation, error handling, and confirmations  
- 💾 Persistent data storage via MySQL  

---

## 🛠️ Tech Stack

- **Java** – GUI built with Swing & AWT  
- **MySQL** – Database for storing users, inventory, and financial data  
- **JDBC** – Java Database Connector  
- **iTextPDF** – For generating PDF reports  
- **NetBeans IDE** – Used for development  

---

## 🚀 How to Run

### 🧰 Prerequisites:

- Java JDK 8 or higher  
- MySQL installed and running  
- NetBeans (or compatible IDE)

### ▶️ Steps:

1. Clone this repository  
2. Import the project into NetBeans  
3. Create a MySQL database named `anaskdatabase`  
4. Create the necessary tables (`registration`, `inventory`, `finance`) as described below  
5. Update DB credentials in `DatabaseConnector.java` or wherever your connection is defined  
6. Run the project via `Main.java`

---

## 🧪 Test Credentials

Use the following credentials to test the app:

```txt
Username: Adamp
Password: Asdfghjkl!1
```

## 🗃️ Database Schema

📌 **Database Name**: `anaskdatabase`


```sql
CREATE TABLE registration (
  fname VARCHAR(33),
  lname VARCHAR(33),
  username VARCHAR(33) PRIMARY KEY,
  password VARCHAR(33)
);

CREATE TABLE inventory (
  item_id INT PRIMARY KEY AUTO_INCREMENT,
  item_name VARCHAR(100),
  quantity INT,
  price DOUBLE,
  description TEXT
);
CREATE TABLE finance (
  id INT PRIMARY KEY AUTO_INCREMENT,
  type VARCHAR(10),  -- 'income' or 'expense'
  category VARCHAR(50),
  amount DOUBLE,
  date DATE,
  notes TEXT
);
```
