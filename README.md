# Housing-Data-Cleaning-ETL



## Project Overview 

This project demonstrates data transformation techniques to clean and 
standardise messy, real-world system exports typical of those from UK housing 
associations (e.g., Reapit or Capita). By simulating a production environment, I integrated 
three disparate data sources- MS SQL Server logs, flat CSVs, and manual Excel files, into a 
unified, analysis-ready dataset. The goal was to eliminate human errors and structural 
glitches, ensuring absolute data integrity for downstream reporting. 


<img width="771" height="471" alt="Data Ingestion from MS SQL Server" src="https://github.com/user-attachments/assets/758edda9-d4f6-41d9-afaf-6fb21d7cf75f" />
*Data Ingestion from MS SQL Server*

<img width="1193" height="531" alt="Loading raw SQL Server data into Power Query" src="https://github.com/user-attachments/assets/f76a8925-08c4-4575-b5b8-fa1621402636" />
*Loading raw SQL Server data into Power Query*


## Key Skills Demonstrated

* Multi-Source Data Integration: I ingested and consolidated three distinct data streams 
(SQL Server Repairs Log, a CRM Tenancy Register CSV, and a manual Excel Vulnerability 
Register) into a centralised Power Query pipeline. 

* Text Standardisation & Hygiene: I resolved case discrepancies (e.g., "EALING" vs "ealing") 
by applying text capitalisation and using the Trim tool to eliminate trailing whitespace, 
preventing categorisation errors. 

* Data De-duplication: I implemented structural de-duplication steps across the unified 
rows to eradicate system export glitches and isolate unique property entries. 

* Pattern Recognition & Parsing: I utilised the "Column From Examples" feature in Power 
Query to automatically parse and standardise unformatted British postcodes (e.g., 
converting "tw33pa" to "TW3 3PA") for future geospatial mapping.

* Data Type Optimisation: I replaced text anomalies (like "MISSING" or "None") with proper 
system null values to preserve calculation integrity. Finally, I enforced strict data types, 
applying Fixed Decimal Numbers to currency fields to eliminate rounding errors. 



<img width="1333" height="661" alt="Column From Examples for Postcode Parsing" src="https://github.com/user-attachments/assets/5763856f-3315-4291-926d-420ac52c6564" />
*Column From Examples for Postcode Parsing*

<img width="1345" height="629" alt="Clean data result and profiling validation for the Tenancies table" src="https://github.com/user-attachments/assets/06b9d37b-c41b-44c7-b192-e820392a685f" />
*Clean data result and profiling validation for the Tenancies table*

<img width="1339" height="661" alt="Clean data result and profiling validation for the Vulnerability table" src="https://github.com/user-attachments/assets/d28d7f44-077c-4ca0-819c-f75b64efe401" />
*Clean data result and profiling validation for the Vulnerability table*

<img width="1347" height="637" alt="Clean data result and profiling validation for the Repair_Log table" src="https://github.com/user-attachments/assets/7b397743-1673-424b-b706-75c168c08872" />
*Clean data result and profiling validation for the Repair_Log table*

## Tools Used 

Power BI Desktop, Power Query, MS SQL Server, Excel, CRM (Reapit/Capita) data exports. 
