## SQL & Database Workflow (AWS RDS – MySQL)

This project uses **AWS RDS (MySQL)** as the relational data source for analytics and visualization in Power BI.

---

### RDS Instance Setup
- An AWS RDS MySQL instance was created using the AWS Management Console.
- During instance creation, a database name was not specified.
- The database was later created manually after connecting to the RDS instance.

---

### Database & Table Creation
- Connection to the RDS instance was established using **MySQL Workbench** with:
  - Endpoint
  - Port
  - Username and password
- A database was created manually inside the RDS instance.
- A table was created with column definitions matching the cleaned immigration dataset.

---

### Data Loading
- Cleaned immigration data (prepared earlier in the AWS S3 pipeline project) was imported into the MySQL table.
- Data import was performed using **MySQL Workbench’s Table Data Import Wizard**.
- This approach reflects a common analyst workflow for loading structured datasets into relational databases.

---

### SQL Usage
- SQL was used to:
  - Validate data after import
  - Verify row counts and column mappings
  - Support analytical queries consumed by Power BI
- Power BI connects directly to the AWS RDS MySQL database to retrieve data for dashboard creation.

---

### Notes
- SQL scripts are not included in this repository because database creation and data loading were performed interactively using MySQL Workbench.
- This project focuses on **cloud database connectivity and analytics consumption**, rather than automated database provisioning.
