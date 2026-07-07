# 🏢 SuperStore Data Warehouse with SSIS

An end-to-end ETL project built using **SQL Server Integration Services (SSIS)** to design and populate a **Data Warehouse** from the SuperStore operational database.

## 📌 Project Overview

This project demonstrates the complete ETL process, including:

- Extracting data from the SuperStore source database
- Transforming and cleansing data
- Loading data into a Star Schema Data Warehouse
- Building Dimension and Fact tables using SSIS packages

---

## 🛠️ Technologies

- SQL Server
- SQL Server Integration Services (SSIS)
- SQL Server Management Studio (SSMS)
- Visual Studio 2022

---

## 📂 Project Structure

```
SSIS/
│
├── Database/
│   ├── SuperStore.sql
│   └── SuperStoreDW.sql
│
├── Packages/
│   ├── DimCustomer.dtsx
│   ├── DimGeo.dtsx
│   ├── DimProduct.dtsx
│   ├── DimShipMode.dtsx
│   └── FactOrder.dtsx
│
├── Images/
│
└── README.md
```

---

## ⭐ Data Warehouse Schema

The Data Warehouse is designed using a **Star Schema**.

### Dimension Tables

- DimCustomer
- DimProduct
- DimGeo
- DimShipMode

### Fact Table

- FactOrder

---

## 🔄 ETL Workflow

1. Read data from the SuperStore source database.
2. Perform data cleansing and transformation.
3. Lookup existing dimension records.
4. Load Dimension tables.
5. Populate the FactOrder table.
6. Store the final data in the SuperStore Data Warehouse.

---

## 📦 SSIS Packages

| Package | Description |
|----------|-------------|
| DimCustomer.dtsx | Loads customer dimension |
| DimProduct.dtsx | Loads product dimension |
| DimGeo.dtsx | Loads geographical dimension |
| DimShipMode.dtsx | Loads shipping mode dimension |
| FactOrder.dtsx | Loads fact table with foreign keys |

---

## 🚀 Getting Started

### 1. Create the Source Database

Run:

```
Database/SuperStore.sql
```

### 2. Create the Data Warehouse

Run:

```
Database/SuperStoreDW.sql
```

### 3. Open the Project

Open the SSIS solution in Visual Studio.

### 4. Configure Connection Managers

Update the SQL Server instance name if necessary.

### 5. Execute Packages

Run the Dimension packages first, then execute the FactOrder package.

---

## 📸 Project Screenshots

- Architecture Diagram
- Star Schema
- Control Flow
- Data Flow
- SQL Results

*(See the Images folder.)*

---

## 📈 Learning Outcomes

- ETL Development using SSIS
- Data Warehouse Design
- Star Schema Modeling
- Dimension & Fact Table Loading
- SQL Server Integration Services
- Lookup Transformations
- Data Flow Design

---

## 👨‍💻 Author

**Arshia Norouzi**

GitHub: https://github.com/YourUsername
LinkedIn: https://linkedin.com/in/YourProfile
