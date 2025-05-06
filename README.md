# ADF_ETL_Project
This is a sample ETL processing project where it will incrementally load delta data from two raw tables and processed to single insights reporting table. On a high level it has a master pipeline which responsible for getting triggered and execute 3 different pipelines in sequencial order where one will ingest raw data from raw table to blob storage, another will clean and process the data using data flow transformations, other will refine and unite data and then inserts to reporting tables main and history tables.

Features
- Fully Automated
- Incremental delta data loading
- Bulk table dynamic copy
- Dynamically handling datasets (only two used for all pipeline activities and dataflows, dynamically works for all)
- Dynamic handling of folderpaths/filenames using parameters and variables
- Loading pipeline run details into log table
- Inserting data to SCD type reporting tables.
