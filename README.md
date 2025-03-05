# 📊 DS2002 - Data Project 1: ETL Data Processor

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0%2B-orange.svg)](https://www.mysql.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🎯 Project Overview
This project demonstrates the implementation of an ETL (Extract, Transform, Load) pipeline for data processing. It showcases the ability to work with various data systems (OLTP/OLAP) and handle different data formats through a comprehensive data mart solution.

## 🔍 Key Features
- Dimensional data mart design
- Multi-source ETL pipeline implementation
- SQL query optimization
- Error handling and data validation
- Cross-platform data integration

## 📊 Project Components

### 1. Data Mart Design
- Dimensional model implementation
- Date dimension for temporal analysis
- Multiple dimension tables (minimum 2)
- Fact table for business process metrics

### 2. ETL Pipeline
- Data extraction from multiple sources:
  - SQL database (MySQL/Oracle/SQL Server)
  - NoSQL database (MongoDB/Redis/Cassandra)
  - File system (local/remote)
  - API data (JSON/CSV format)
- Data transformation and cleaning
- Automated data loading process
- Error handling implementation

### 3. SQL Implementation
- Complex SELECT statements
- Multi-table joins (3+ tables)
- Aggregation functions
- Data grouping operations

## 🛠️ Technologies Used
- **Python**: ETL pipeline implementation
- **SQL**: Data definition and manipulation
- **Databases**: 
  - Relational: MySQL/Oracle/SQL Server
  - NoSQL: MongoDB/Redis/Cassandra
- **Data Formats**: JSON, CSV, API payloads

## 📁 Repository Structure
```bash
project/
├── src/                  # Source code
│   ├── etl/             # ETL pipeline scripts
│   └── sql/             # SQL queries and schemas
├── data/
│   ├── raw/             # Original source data
│   └── processed/       # Transformed data
├── docs/                # Documentation
└── requirements.txt     # Python dependencies
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- MySQL or compatible RDBMS
- NoSQL database system
- Required Python packages:
  ```bash
  pip install -r requirements.txt
  ```

### Setup and Deployment
1. Clone the repository
2. Install dependencies
3. Configure database connections
4. Run ETL pipeline:
   ```bash
   python src/etl/main.py
   ```

## 📝 Project Requirements
- Date dimension implementation
- Minimum 2 additional dimension tables
- 1+ fact table
- Data from 3+ different sources
- Comprehensive error handling
- SQL query demonstrations

## 🎓 Academic Context
This project is developed for DS2002 at the University of Virginia, focusing on data integration and ETL pipeline development.

## 👤 Author
Andre Chuabio
- GitHub: [@AndreChuabio](https://github.com/AndreChuabio)

## 🙏 Acknowledgments
- UVA DS2002 course staff
- Sample data providers
- Open-source community

---
⭐️ Developed at the University of Virginia 
