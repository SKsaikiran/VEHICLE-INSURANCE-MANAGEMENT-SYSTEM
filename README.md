# Vehicle Insurance Management System

[**SYNOPSIS**](https://github.com/SKsaikiran/VEHICLE-INSURANCE-MANAGEMENT-SYSTEM/blob/2aad7133cb5a7b3220e1ad215296059b6997b7b7/Documents/SYNOPSIS.md)

## Contents
1. [Introduction](#introduction)
   - [Problem Statement](#problem-statement)
   - [Objectives](#objectives)
   - [Dataset Description](#dataset-description)
2. [System Design](#system-design)
   - [ER Diagram](#er-diagram)
   - [ER to Relation Mapping](#er-to-relation-mapping)
   - [Schema Diagram](#schema-diagram)
3. [Project Setup](#project-setup)
4. [Database Setup](#database-setup)
5. [Running the Application](#running-the-application)
---

## Introduction

The **Vehicle Insurance Management System** is designed to overcome issues faced by traditional manual systems. This software aims to eliminate or reduce the common challenges of maintaining records manually, improving operational efficiency for insurance management companies.

With this application, data entry errors are minimized, and error messages are provided for invalid entries, making it user-friendly. By automating record-keeping and management tasks, the system enables users to focus on other essential business activities.

This system is tailored to meet the specific needs of organizations to effectively manage data related to insurance, customers, and vehicles, offering secure and efficient record handling, remote access, and resource management.

### Problem Statement

The purpose of this system is to automate the existing manual process using computerized equipment and software, allowing valuable data to be stored longer and accessed or modified with ease. This system is intended to meet the practical requirements of the insurance management industry.

### Objectives

The main objectives of this project are to:
- Manage details of customers, insurance policies, vehicles, and administrative information.
- Ensure data integrity and security while simplifying administrative tasks.
- Minimize manual errors in customer, insurance, and vehicle records.
- Provide centralized access, allowing only administrators to make changes, thereby ensuring control over information.

### Dataset Description

- **Customer Module**: Manages customer details (name, cust_id, address, email).
- **Insurance Module**: Manages insurance policy details (policy_id, price, description, validity).
- **Vehicle Module**: Manages vehicle information (reg_no, description, type, vehicle_no).
- **Login Module**: Manages user login details (login_id, username, email, password).
- **Admin Module**: Manages customer details for administrators (id, name, phone, email).
- **Accident Module**: Manages accident details (location, date).

---

## System Design

### ER Diagram

The ER (Entity-Relationship) Diagram represents the entities, attributes, and relationships within the system.

![ER Diagram](https://user-images.githubusercontent.com/89591339/205450286-969500dd-c84b-4a56-98b8-7a1dd6496da9.png)

### ER to Relation Mapping

- **Admin** and **Insurance**: 1:n relationship (`Manages`)
- **Admin** and **Login**: 1:1 relationship (`Has`)
- **Insurance** and **Customer**: n:1 relationship (`Insurance holder`)
- **Customer** and **Accident**: 1:n relationship (`Involved`)
- **Customer** and **Vehicle**: 1:n relationship (`Occurs`)
- **Accident** and **Vehicle**: 1:1 relationship (`Happened`)

### Schema Diagram

The **Schema Diagram** represents the database structure, defining how the tables and relationships are constructed.

![Schema Diagram](https://user-images.githubusercontent.com/89591339/205450353-f279516e-093a-4132-b016-f37dd8a11704.png)

---

## Project Setup

### Clone the Repository
```bash
git clone https://github.com/SKsaikiran/VEHICLE-INSURANCE-MANAGEMENT-SYSTEM.git
cd VEHICLE-INSURANCE-MANAGEMENT-SYSTEM
```

### Configure Environment Variables
1. Create a `.env` file in the project root directory.
2. Add the following configurations:
    ```plaintext
    DB_URL=jdbc:mysql://localhost:3306/vehicle_insurance_db
    DB_USERNAME=your_mysql_username
    DB_PASSWORD=your_mysql_password
    ```

---

## Database Setup

1. Open MySQL Workbench or command-line MySQL.
2. Create a new database:
   ```sql
   CREATE DATABASE vehicle_insurance_db;
   ```
3. Import the SQL file located in `src/main/resources` to create tables and initial data.

---

## Running the Application

1. Open a terminal in the project root directory.
2. Compile the project:
   ```bash
   mvn clean install
   ```
3. Run the application:
   ```bash
   mvn spring-boot:run
   ```
4. Access the application at `http://localhost:8080`.

---

## Contributing

Contributions are welcome! Fork this repository and submit a pull request to add or improve features.
