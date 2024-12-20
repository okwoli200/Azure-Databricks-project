# Azure-Databricks-project

## Project Overview  
This project demonstrates how to extract data from the **an OnPrem** database, load it into Azure Storage, and use **Azure Databricks** to perform data transformations. The pipeline is designed to enable efficient data management and processing in the cloud.

## Objectives  
1. **Data Loading**: Extract data from the **AdventureWorksLT2017** database and load it into Azure Storage.  
2. **Data Transformation**: Utilize Azure Databricks to clean, transform, and prepare the data for analysis or downstream consumption.

---

## Prerequisites  
To successfully run this project, you need the following:  
- **AdventureWorksLT2017** database available locally or on a SQL Server.  
- An **Azure Storage Account** configured with access credentials.  
- An **Azure Databricks Workspace**.  
- Required libraries for database connection and transformation, such as:  
  - `pymssql` or `pyodbc` for SQL Server connections.  
  - `pyspark` for transformations.  

---

## Steps  

### 1. Load Data from AdventureWorksLT2017 to Azure Storage  
1. **Connect to the AdventureWorksLT2017 Database**  
   - Establish a connection using  Azure Data Factory.  

2. **Extract Data**  
   - Query the database to extract the necessary tables or datasets.  

3. **Upload Data to Azure Storage**  
   - Save the extracted data as files (e.g., CSV, Parquet) and upload them to your Azure Blob Storage or Data Lake.  

### 2. Transform Data Using Azure Databricks  
1. **Set Up Databricks Cluster**  
   - Create and configure a cluster in Azure Databricks.  
   - Ensure access to Azure Storage (use a Key Vault or SAS token for secure access).  

2. **Load Data into Databricks**  
   - Use PySpark to load data from Azure Storage into Databricks.  
   

3. **Perform Data Transformations**  
   - Apply transformations such as filtering, aggregations, or data enrichment.  
  

4. **Save Transformed Data**  
   - Write the transformed data back to Azure Storage in your preferred format.  
  

---

## Deliverables  
- **Raw Data**: Stored in Azure Storage.  
- **Transformed Data**: Available in Azure Storage for analysis or further processing.  

---

## Notes  
- Ensure that the database connection credentials and Azure Storage access are secured.  
- Review transformation logic to align with the specific requirements of your use case.  
- Leverage Azure Key Vault to manage sensitive information like connection strings and access keys.  

---

## Author  
**Emmanuel Okwoli**    
