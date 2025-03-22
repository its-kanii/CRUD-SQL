# CRUD Operations in SQL for Various Management Systems 🚀

## Introduction 📌
This document provides an overview of **CRUD (Create, Read, Update, Delete) operations** in SQL for different management systems, including:
- **🛒 Sales Management System**
- **🏥 Healthcare Management System**
- **👨‍💼 HR Management System**
- **🎓 Student Admission System**
- **🚌 Transport Management System**
- **📦 Inventory Management System**

Each section includes table creation, inserting data, retrieving records, updating records, and deleting records.

---

## 1. 🛒 Sales Management System
**Table Structure:**
```sql
CREATE TABLE Sales (
    SaleID INT PRIMARY KEY AUTO_INCREMENT,
    ProductName VARCHAR(100),
    CustomerName VARCHAR(100),
    Quantity INT,
    Price DECIMAL(10,2),
    SaleDate DATE
);
```

**Insert Data:**
```sql
INSERT INTO Sales (ProductName, CustomerName, Quantity, Price, SaleDate) 
VALUES ('Laptop', 'John Doe', 1, 1000.00, '2025-03-21');
```

**Read Data:**
```sql
SELECT * FROM Sales;
```

**Update Data:**
```sql
UPDATE Sales SET Quantity = 2, Price = 2000.00 WHERE SaleID = 1;
```

**Delete Data:**
```sql
DELETE FROM Sales WHERE CustomerName = 'John Doe';
```

---

## 2. 🏥 Healthcare Management System
**Table Structure:**
```sql
CREATE TABLE Patients (
    PatientID INT PRIMARY KEY AUTO_INCREMENT,
    Name VARCHAR(100),
    Age INT,
    Gender VARCHAR(10),
    Diagnosis VARCHAR(255),
    AdmissionDate DATE
);
```

**Insert Data:**
```sql
INSERT INTO Patients (Name, Age, Gender, Diagnosis, AdmissionDate) 
VALUES ('Alice Smith', 30, 'Female', 'Diabetes', '2025-03-18');
```

**Read Data:**
```sql
SELECT * FROM Patients;
```

**Update Data:**
```sql
UPDATE Patients SET Diagnosis = 'Bronchitis' WHERE PatientID = 1;
```

**Delete Data:**
```sql
DELETE FROM Patients WHERE Name = 'Alice Smith';
```

---

## 3. 👨‍💼 HR Management System
**Table Structure:**
```sql
CREATE TABLE Employees (
    EmployeeID INT PRIMARY KEY AUTO_INCREMENT,
    Name VARCHAR(100),
    Age INT,
    Gender VARCHAR(10),
    Department VARCHAR(50),
    Salary DECIMAL(10,2),
    HireDate DATE
);
```

**Insert Data:**
```sql
INSERT INTO Employees (Name, Age, Gender, Department, Salary, HireDate) 
VALUES ('Bob Johnson', 40, 'Male', 'Finance', 80000.00, '2021-09-25');
```

**Read Data:**
```sql
SELECT * FROM Employees;
```

**Update Data:**
```sql
UPDATE Employees SET Salary = 90000.00 WHERE EmployeeID = 1;
```

**Delete Data:**
```sql
DELETE FROM Employees WHERE Name = 'Bob Johnson';
```

---

## 4. 🎓 Student Admission System
**Table Structure:**
```sql
CREATE TABLE Students (
    StudentID INT PRIMARY KEY AUTO_INCREMENT,
    Name VARCHAR(100),
    Age INT,
    Gender VARCHAR(10),
    Course VARCHAR(50),
    AdmissionDate DATE,
    FeesPaid DECIMAL(10,2)
);
```

**Insert Data:**
```sql
INSERT INTO Students (Name, Age, Gender, Course, AdmissionDate, FeesPaid) 
VALUES ('John Doe', 18, 'Male', 'Computer Science', '2025-03-10', 5000.00);
```

**Read Data:**
```sql
SELECT * FROM Students;
```

**Update Data:**
```sql
UPDATE Students SET Course = 'Data Science' WHERE StudentID = 1;
```

**Delete Data:**
```sql
DELETE FROM Students WHERE Name = 'John Doe';
```

---

## 5. 🚌 Transport Management System
**Table Structure:**
```sql
CREATE TABLE Vehicles (
    VehicleID INT PRIMARY KEY AUTO_INCREMENT,
    VehicleNumber VARCHAR(20) UNIQUE,
    DriverName VARCHAR(100),
    Route VARCHAR(100),
    Capacity INT,
    Status VARCHAR(20),
    LastServiceDate DATE
);
```

**Insert Data:**
```sql
INSERT INTO Vehicles (VehicleNumber, DriverName, Route, Capacity, Status, LastServiceDate) 
VALUES ('KA-01-AB-1234', 'John Doe', 'City Center to Airport', 40, 'Active', '2025-02-15');
```

**Read Data:**
```sql
SELECT * FROM Vehicles;
```

**Update Data:**
```sql
UPDATE Vehicles SET Status = 'Under Maintenance' WHERE VehicleNumber = 'KA-01-AB-1234';
```

**Delete Data:**
```sql
DELETE FROM Vehicles WHERE VehicleNumber = 'KA-01-AB-1234';
```

---

## 6. 📦 Inventory Management System
**Table Structure:**
```sql
CREATE TABLE Products (
    ProductID INT PRIMARY KEY AUTO_INCREMENT,
    ProductName VARCHAR(100),
    Category VARCHAR(50),
    Quantity INT,
    Price DECIMAL(10,2),
    Supplier VARCHAR(100),
    LastRestocked DATE
);
```

**Insert Data:**
```sql
INSERT INTO Products (ProductName, Category, Quantity, Price, Supplier, LastRestocked) 
VALUES ('Laptop', 'Electronics', 50, 800.00, 'Tech Supplies Ltd.', '2025-03-15');
```

**Read Data:**
```sql
SELECT * FROM Products;
```

**Update Data:**
```sql
UPDATE Products SET Quantity = Quantity + 20 WHERE ProductName = 'Laptop';
```

**Delete Data:**
```sql
DELETE FROM Products WHERE ProductName = 'Laptop';
```

---

## Conclusion 🎯
This document provides structured SQL queries for CRUD operations across different management systems. Each system can be further expanded with additional features like **constraints, triggers, and stored procedures** to enhance functionality.

Feel free to modify these examples based on your database requirements! 💡

