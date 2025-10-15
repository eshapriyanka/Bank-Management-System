# 🏦 Bank Management System

The **Bank Management System** is a Java Swing-based desktop application designed to simulate basic banking operations such as account creation, deposit, withdrawal, and balance inquiry. This system provides a user-friendly interface and integrates with a MySQL database to store and manage customer data securely.

## 🎯 Objective

To provide a simple, intuitive application for managing bank account operations in an educational or prototype environment, demonstrating Java Swing GUI development and MySQL integration.

## 🚀 Features

- 🔐 **User Authentication**: Admin login with credentials.
- 👤 **Customer Management**:
  - Create new bank accounts
  - View customer details
  - Update and delete accounts
- 💰 **Banking Operations**:
  - Deposit and withdraw funds
  - View account balance
  - Generate transaction receipts
- 📊 **Database Integration**:
  - Stores all customer and transaction details in MySQL
- 🖼️ **GUI Interface**:
  - Built using Java Swing for a clean and responsive interface

## 🛠️ Technologies Used

- **Language**: Java
- **GUI**: Java Swing
- **Database**: MySQL
- **IDE**: Eclipse / IntelliJ / NetBeans (compatible)

## ⚙️ Installation & Setup

### 🗂️ Clone the repository:

```bash
git clone https://github.com/Sahitha-chunduri/Bank-Management-System.git
cd Bank-Management-System
```
## 🔧 Prerequisites
- **Java JDK 8 or above**

- **MySQL server installed and running**

- **MySQL Connector/J (JDBC driver)**

## 🛠️ Setup Steps
1. Create the database in MySQL:

```bash
CREATE DATABASE bankdb;
USE bankdb;
```
2. Configure the DB connection in the Java project:

Inside the Java file that handles the database connection (likely DBConnection.java), ensure the following:

```bash
String url = "jdbc:mysql://localhost:3306/bankdb";
String username = "your_mysql_username";
String password = "your_mysql_password";
```
3. Compile and Run the Application

Using your IDE, open the project folder and run the main Java file.

## 🧩 Future Enhancements
- **Add user role-based access (Admin/User)**

- **Implement interest calculation logic**

- **Export customer reports to PDF or Excel**

- **Improve UI with more modern JavaFX interface**

- **Add email notifications for transactions**

## 🤝 Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any improvements, features, or bug fixes.

## 📄 License
This project is licensed under the MIT License. See the LICENSE file for more information.




