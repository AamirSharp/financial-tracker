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

## 🧪 Test Credentials

To test the system, use the following login:

```txt
Username: Adamp
Password: Asdfghjkl!1
📁 Project Structure
graphql
Copy
Edit
financial-tracker/
├── src/                       # Java source code
├── Documentation/            # IB IA PDFs: Criteria A–E, Appendices
├── Product/                  # Executables (if included)
├── build.xml                 # NetBeans Ant build config
├── README.md                 # This file
🗃️ Database Schema
📌 Database Name: anaskdatabase
Table: registration
Column	Type
fname	VARCHAR(33)
lname	VARCHAR(33)
username	VARCHAR(33) PRIMARY KEY
password	VARCHAR(33)

Table: inventory
Stores product details: item name, price, quantity, etc.

Table: finance
Tracks income and expense records with timestamps and categories.

⚠️ Full details are available in Criterion C and Appendix II in the Documentation/ folder.

🚀 How to Run
🧰 Prerequisites:
Java JDK 8 or higher

MySQL installed and running

NetBeans (or compatible IDE)

▶️ Steps:
Clone this repository

Import the project into NetBeans

Create a MySQL database named anaskdatabase

Create the necessary tables (registration, inventory, finance) as described above or in the documentation

Update DB credentials in DatabaseConnector.java or wherever the connection is defined

Run the project via Main.java

