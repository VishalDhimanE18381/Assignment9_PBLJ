# Spring and Hibernate Application – Multi-Level Project

This project demonstrates various levels of Java application development using Spring Framework and Hibernate ORM. It includes three levels:

- **Easy Level**: Simple Spring Dependency Injection using Java-based configuration.
- **Medium Level**: Hibernate-based CRUD operations with MySQL.
- **Hard Level**: Transaction management in a Spring + Hibernate integrated banking application.

---

## 🟢 Easy Level: Spring Dependency Injection using Java Config

### Description:
A simple Spring application that demonstrates **Dependency Injection (DI)** using `@Configuration` and `@Bean`.

### Classes:
- `Course`: Contains `courseName` and `duration`.
- `Student`: Contains `name` and a reference to `Course`.

### Features:
- Uses Java-based configuration instead of XML.
- Spring Context is loaded in the main method to display Student details.

### How to Run:
1. Create `Course` and `Student` classes.
2. Create a config class using `@Configuration`.
3. Run the main class to load the context and display output.

---

## 🟡 Medium Level: Hibernate CRUD Application with MySQL

### Description:
A standalone Hibernate application that performs **CRUD operations** on a `Student` entity.

### Requirements:
- MySQL database setup.
- Hibernate configuration (`hibernate.cfg.xml`).
- Entity class: `Student` with `id`, `name`, and `age`.
- Basic CRUD operations using Hibernate SessionFactory.

### Features:
- Add, Read, Update, Delete student records.
- Fully annotated `Student` class.

### How to Run:
1. Set up MySQL and configure database in `hibernate.cfg.xml`.
2. Run the test class to perform CRUD operations.

---

## 🔴 Hard Level: Spring + Hibernate Transaction Management (Banking System)

### Description:
A banking system demonstrating **transactional integrity** using Spring and Hibernate.

### Entities:
- `Account`: Holds account details and balance.
- `Transaction`: Records fund transfers.

### Features:
- Money transfer between accounts.
- Atomic transaction handling using Hibernate Transactions.
- Demonstrates both successful and failed transfers (with rollback).

### How to Run:
1. Set up Spring and Hibernate configuration.
2. Define DAOs and Services with `@Transactional`.
3. Create a test class to perform successful and failed money transfers.

---

## 💾 Technologies Used
- Java 8+
- Spring Framework
- Spring Core / Context
- Hibernate ORM
- MySQL Database
- Maven / Gradle (Optional)

---

## 📂 Project Structure
- easy-level/
  ├── Course.java
  ├── Student.java
  ├── AppConfig.java
  └── MainApp.java

- medium-level/
  ├── Student.java
  ├── HibernateUtil.java
  ├── StudentDAO.java
  └── MainCRUD.java

- hard-level/
  ├── Account.java
  ├── Transaction.java
  ├── AccountService.java
  ├── BankingAppConfig.java
  └── BankingTest.java
