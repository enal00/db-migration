# db-migration
Migrating enterprise data from SQL Server to PostgreSQL

We'll be using
- SQL
- Python
- Jupyter notebook

# Pseudocode

## High-level

1. Audit the data in SQL server
2. Extract data from SQL server (SSMS)
3. Transform the data
4. Load the data in PostgreSQL
5. Validate the data (after migration)
6. Generate a validation report

## Low-level

1. Cretae a .env file
2. Load env variable
3. Connect to SQL Server (pyodbc)
4. Connect to Postgres (psycopg2)
5. Audit the data
6. For each table
7. Get row count
8. Extract all rows
9. Transform the column names to lowercase
10. Convert the data types
11. Create tables in Postgres
12. Load tables into Postgres
13. Run post-data migration checks
14. Generate validation report 
