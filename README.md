# 📊 Movie Rental Data Warehouse Platform

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0%2B-orange.svg)](https://www.mysql.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4.0%2B-green.svg)](https://www.mongodb.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🎯 Project Overview
A comprehensive data warehouse solution for movie rental business analytics, integrating data from multiple sources including traditional RDBMS, NoSQL databases, and REST APIs. The platform provides a unified view of rental transactions, movie performance metrics, customer behavior, and staff performance.

## 🔍 Key Features
- Multi-source data integration (SQL, NoSQL, API)
- Dimensional data warehouse model
- Automated ETL pipeline
- Movie performance analytics
- Customer behavior tracking
- Revenue analysis system

## 📊 Architecture Components

### 1. Data Warehouse Schema
- **Fact Table**: 
  - `fact_payments`: Rental transactions with temporal and financial metrics
- **Dimension Tables**:
  - `customer`: Customer demographics and activity
  - `staff`: Employee information
  - `inventory`: Comprehensive movie data including:
    - Basic film information
    - Award statistics
    - Ratings data
    - Revenue metrics
  - `date_dimension`: Temporal analysis support

### 2. Data Sources
- **Sakila Database**: Core rental business data
  - Customer records
  - Staff information
  - Basic movie details
  - Transaction history
- **MongoDB (sample_mflix)**:
  - Movie ratings
  - Award information
- **TMDB API**:
  - Movie revenue data
  - Additional film metrics

### 3. ETL Pipeline
- **Extract**:
  - SQL queries for transactional data
  - MongoDB connection for movie metrics
  - REST API integration for revenue data
- **Transform**:
  - Data cleaning and standardization
  - ID matching across sources
  - Null handling
  - Format consistency enforcement
- **Load**:
  - Staged loading process
  - Dimension table population
  - Fact table integration
  - Data validation

## 🛠️ Technology Stack
- **Core Processing**: Python 3.8+
- **Data Storage**: 
  - MySQL 8.0+ (Primary warehouse)
  - MongoDB 4.0+ (Source system)
- **Python Libraries**:
  - `pandas`: Data manipulation
  - `pymongo`: MongoDB integration
  - `requests`: API handling
- **APIs**: TMDB API for movie data

## 📁 Project Structure
```bash
project/
├── Lab 1/
│   ├── SQL/
│   │   ├── 1_schema_creation.sql     # Database schema
│   │   ├── 2_table_population.sql    # Data loading
│   │   ├── 3_date_dimension_creation.sql
│   │   ├── 4_date_key_creation.sql
│   │   └── 5_query.sql              # Analysis queries
│   ├── Python/
│   │   ├── lab_api_call.ipynb       # TMDB API integration
│   │   └── lab_mongo_call.ipynb     # MongoDB extraction
│   ├── Data/
│   │   ├── apidat.csv              # API extracted data
│   │   └── mongodat.csv            # MongoDB extracted data
│   └── Documentation/
        └── Data Sources.docx        # Source documentation
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- MySQL 8.0+
- MongoDB 4.0+
- TMDB API key
- Required Python packages:
  ```bash
  pip install pandas pymongo requests
  ```

### Setup Process
1. Clone the repository
2. Configure database connections:
   - MySQL credentials
   - MongoDB connection string
   - TMDB API key
3. Run schema creation scripts
4. Execute ETL pipeline:
   - Run MongoDB extraction
   - Process API data
   - Load dimension tables
   - Populate fact table

## 📊 Data Model
- **Star Schema Design**
  - Centralized fact table (payments/rentals)
  - Connected dimension tables
  - Temporal dimension support
  - Movie metrics integration

## 🔍 Analysis Capabilities
- Rental pattern analysis
- Revenue tracking
- Movie performance metrics
- Customer behavior insights
- Staff performance evaluation
- Temporal trend analysis

## 👤 Developer
Andre Chuabio
- GitHub: [@AndreChuabio](https://github.com/AndreChuabio)

## 🙏 Acknowledgments
- TMDB API for movie data
- MongoDB Atlas for sample datasets
- MySQL Sakila database

---
⭐️ Built with modern data engineering practices
