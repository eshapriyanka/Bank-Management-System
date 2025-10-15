# Bank Management System

A desktop banking application built with Java Swing that simulates the core functions of an ATM. It provides a graphical user interface for users to manage their accounts, perform transactions, and view their statements, with all data stored in a MySQL database.



---

## Features

* **Secure User Onboarding:** Multi-step signup process for new customers.
* **User Authentication:** Secure login using a card number and PIN.
* **Transaction Menu:** A central hub for all banking operations.
* **Core Banking Operations:**
    * **Deposit:** Add funds to an account.
    * **Withdrawal:** Withdraw funds with balance validation.
    * **Fast Cash:** Quick withdrawal of pre-set amounts.
    * **PIN Change:** Securely update the account PIN.
    * **Balance Enquiry:** Check the current account balance.
    * **Mini Statement:** View a list of recent transactions.

---

## Technology Stack

* **Language:** Java
* **GUI Framework:** Java Swing
* **Database:** MySQL
* **External Libraries:**
    * JCalendar (for the date picker in the signup form)
    * MySQL Connector/J (JDBC Driver)

---

## Setup and Installation

To run this project on your local machine, follow these steps.

### 1. Prerequisites

Make sure you have the following software installed:
* Java Development Kit (JDK) 8 or newer
* MySQL Server
* An IDE like IntelliJ IDEA or Eclipse

### 2. Clone the Repository

```bash
git clone https://github.com/eshapriyanka/Bank-Management-System.git
```

### 3.Database Setup
You need to create the database and all the required tables. Open MySQL Workbench and run the following SQL script:

```
CREATE DATABASE bankmanagementsystem;

USE bankmanagementsystem;

CREATE TABLE signup (formno VARCHAR(20), name VARCHAR(50), fname VARCHAR(50), dob VARCHAR(20), gender VARCHAR(20), email VARCHAR(50), marital VARCHAR(20), address VARCHAR(100), city VARCHAR(50), pincode VARCHAR(20), state VARCHAR(50));

CREATE TABLE signup2 (formno VARCHAR(20), religion VARCHAR(20), category VARCHAR(20), income VARCHAR(20), education VARCHAR(20), occupation VARCHAR(20), pan VARCHAR(20), aadhar VARCHAR(20), scitizen VARCHAR(20), eaccount VARCHAR(20));

CREATE TABLE signup3 (formno VARCHAR(20), atype VARCHAR(40), cardno VARCHAR(25), pin VARCHAR(10), facility VARCHAR(100));

CREATE TABLE login (formno VARCHAR(20), cardno VARCHAR(25), pin VARCHAR(10));

CREATE TABLE bank (pin VARCHAR(10), date VARCHAR(50), type VARCHAR(20), amount VARCHAR(20));
```

### 4. IDE Configuration
Open the project folder in your IDE (e.g., IntelliJ IDEA).

Set the src folder as the Sources Root.

Add the required JAR files (jcalendar-1.4.jar and the MySQL connector .jar) to the project's libraries/dependencies.

Important: Open the conn.java file and update the database password to match your own MySQL root password.

```
// in src/Bank/Management/System/conn.java
c = DriverManager.getConnection("jdbc:mysql:///bankmanagementsystem", "root", "YOUR_PASSWORD_HERE");
```

### 5. Running the Application
Rebuild the project in your IDE.

Find the login.java file.

Right-click and select "Run".
