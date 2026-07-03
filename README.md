# Housing-Data-Cleaning-ETL


## Project Overview 

This project demonstrates data transformation techniques to clean and 
standardise messy, real-world system exports typical of those from UK housing 
associations (e.g., Reapit or Capita). By simulating a production environment, I integrated 
three disparate data sources- MS SQL Server logs, flat CSVs, and manual Excel files, into a 
unified, analysis-ready dataset. The goal was to eliminate human errors and structural 
glitches, ensuring absolute data integrity for downstream reporting. 


<img width="771" height="471" alt="2 Enterprise Data Ingestion from MS SQL Server" src="https://github.com/user-attachments/assets/a965f40b-da5f-4487-9f44-9fe3b211c7f5" />


<img width="1193" height="531" alt="3 Power Query Navigator Initialising the Repairs_Log Dataset" src="https://github.com/user-attachments/assets/424f1a97-51fb-49b0-9272-2c233868a36f" />



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



<img width="1333" height="661" alt="8 Column From Examples for Postcode Parsing" src="https://github.com/user-attachments/assets/25e0f5e6-9334-456b-bc6d-ff4b583a02b5" />


<img width="1345" height="629" alt="11 Data Profiling   Quality Validation via Applied Steps Panel" src="https://github.com/user-attachments/assets/9001c955-0c18-479c-ae0d-3916b41eb8e6" />


<img width="1339" height="661" alt="14 Handling Missing Values   Normalising Vulnerability Register Anomalies" src="https://github.com/user-attachments/assets/629ba463-c98f-4576-a330-7b1cdba9361c" />


<img width="1347" height="637" alt="15 Categorical Standardisation   Text Mapping for Repairs Category" src="https://github.com/user-attachments/assets/b5e68b09-fcc8-4ee1-b2e1-7c03713470a8" />


## Tools Used 

Power BI Desktop, Power Query, MS SQL Server, Excel, CRM (Reapit/Capita) data exports. 
