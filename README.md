# 🏨 Hotel Data Analysis using Snowflake & Power BI

## 📌 Project Overview
This project focuses on analyzing hotel booking data using **Snowflake (SQL)** and visualizing insights through **Power BI dashboards**.  
A **Medallion Architecture (Bronze, Silver, Gold layers)** approach is implemented to ensure efficient data ingestion, cleaning, and transformation for analytics.

---

## 🚀 Tech Stack
- **Data Warehouse:** Snowflake  
- **Query Language:** SQL  
- **Architecture:** Medallion Architecture  
- **Visualization Tool:** Power BI  

---

## 🏗️ Medallion Architecture Implementation

### 🔹 Data Ingestion (Staging)
- Created a Snowflake database for the project  
- Defined a CSV file format for structured data ingestion  
- Created a staging area to upload and manage raw data files  
- Loaded hotel booking data from stage into Snowflake  

---

## 🥉 Bronze Layer (Raw Data)
- Created a table to store raw hotel booking data  
- Loaded data directly from staging without transformations  
- Preserved original data structure for traceability  
- Performed initial data preview and validation  

---

## 🥈 Silver Layer (Cleaned & Transformed Data)
- Created structured table with appropriate data types  
- Cleaned and standardized the dataset:
  - Fixed inconsistent city and customer name formats  
  - Validated and cleaned email addresses  
  - Converted date fields into proper date format  
  - Handled missing and null values  
  - Removed invalid records (e.g., incorrect dates)  
  - Corrected inconsistent booking status values  
  - Ensured numeric fields like revenue are valid and positive  
- Applied filtering to keep only valid and usable records  

---

## 🥇 Gold Layer (Business-Ready Data)
- Created final curated tables for analytics  
- Built aggregated datasets including:
  - Daily booking trends and revenue  
  - City-wise revenue analysis  
- Created a clean, analytics-ready dataset for reporting  
- Optimized tables for Power BI consumption  

---

## 🔄 Data Pipeline Flow
1. Raw CSV data uploaded to Snowflake Stage  
2. Loaded into **Bronze Layer** (raw data)  
3. Cleaned and transformed in **Silver Layer**  
4. Aggregated and prepared in **Gold Layer**  
5. Connected Gold layer data to **Power BI**  

---

## 📊 Power BI Dashboard
- Connected Power BI to Snowflake Gold tables  
- Created interactive dashboards with:
  - Revenue analysis  
  - Booking trends  
  - Occupancy insights  
  - City-wise performance  
  - Customer behavior insights
<img width="1385" height="782" alt="image" src="https://github.com/user-attachments/assets/fac759b7-db49-4dc3-96c8-638b39377c20" />

---

## 📁 Project Structure

Hotel-Data-Analysis/
│
├── data/
│ ├── bronze/
│ ├── silver/
│ └── gold/
│
├── sql/
│ └── medallion_architecture.sql
│
├── powerbi/
│ └── dashboard.pbix
│
└── README.md


---

## 📈 Key Insights
- Identified peak booking periods  
- Analyzed revenue contribution by cities  
- Improved data quality through cleaning and validation  
- Enabled efficient reporting using structured datasets  

---

## ⭐ Acknowledgements
- Snowflake Documentation  
- Power BI Community  

