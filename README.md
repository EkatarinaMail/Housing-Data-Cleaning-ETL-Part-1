# Housing-Data-Cleaning-ETL

![ETL Pipeline Overview](https://github.com/user-attachments/assets/933e85fc-5f1c-4635-a52e-21cad36838bf)
*From raw multi-source files (Excel/SQL Server) to the final cleansed dataset in Power Query*



## Project Overview 

This project focuses on cleaning and preparing raw housing data for analysis in Power BI. The dataset combines information from SQL Server, CSV files, and Excel spreadsheets, each containing common data quality issues such as duplicates, inconsistent formatting, and missing values.

Using Power Query, I built a repeatable ETL process that transformed these sources into a clean and reliable dataset ready for data modelling and reporting. 


![Data Ingestion from MS SQL Server](https://github.com/user-attachments/assets/758edda9-d4f6-41d9-afaf-6fb21d7cf75f)

*Data Ingestion from MS SQL Server*

![Loading raw SQL Server data into Power Query](https://github.com/user-attachments/assets/f76a8925-08c4-4575-b5b8-fa1621402636)
*Loading raw SQL Server data into Power Query*


## Key Skills Demonstrated

* Data Integration: Combined data from SQL Server, CSV files, and Excel into a single Power Query workflow, creating one consistent dataset for analysis. 

* Data Cleaning: Standardised text values by fixing inconsistent capitalisation, removing extra spaces, and correcting formatting issues to improve data quality. 

* Removing Duplicates: Identified and removed duplicate records created during system exports, ensuring each property appeared only once in the final dataset.

* Data Transformation: Used Power Query's Column From Examples feature to extract and format UK postcodes into a consistent structure, making the data suitable for future reporting and mapping.

* Data Quality: Replaced invalid text values such as "MISSING" and "None" with proper null values and assigned appropriate data types, including fixed decimal numbers for financial data, to ensure accurate calculations



![Column From Examples for Postcode Parsing](https://github.com/user-attachments/assets/5763856f-3315-4291-926d-420ac52c6564)
*Column From Examples for Postcode Parsing*

![Clean data result and profiling validation for the Tenancies table](https://github.com/user-attachments/assets/06b9d37b-c41b-44c7-b192-e820392a685f)
*Clean data result and profiling validation for the Tenancies table*

![Clean data result and profiling validation for the Vulnerability table](https://github.com/user-attachments/assets/d28d7f44-077c-4ca0-819c-f75b64efe401)
*Clean data result and profiling validation for the Vulnerability table*

![Clean data result and profiling validation for the Repair_Log table](https://github.com/user-attachments/assets/7b397743-1673-424b-b706-75c168c08872)
*Clean data result and profiling validation for the Repair_Log table*

## Tools Used 

Power BI Desktop, Power Query, MS SQL Server, Excel, CRM (Reapit/Capita) data exports. 


👉 **Check out the next phase here:** [Housing-Data-Modelling-Metrics-PowerBI](https://github.com/EkatarinaMail/Housing-Data-Modelling-Metrics-PowerBI/blob/main/README.md)
