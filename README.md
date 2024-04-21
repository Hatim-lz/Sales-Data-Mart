# Sales Data Mart

## Overview:
In this project, a Sales Data Mart was developed using SQL Server Integration Services (SSIS) and SQL Server, leveraging the AdventureWorks2022 Dataset for online sales analysis. The project involved utilizing Visual Studio, SQL Server Integration Services (SSIS), and SQL Server Management Studio (SSMS) for project development. 
Slowly Changing Dimensions (SCD) Type 1 and Type 2 techniques were implemented for dimension data management, and a star schema comprising dimension tables (Product, Customer, Territory, and Date) and a central fact table was designed to optimize data analysis. 
Additionally, six SSIS packages were created for building the data mart, and SQL scripts were developed for generating the structure schema of the Sales Data Mart

### ETL_Dim_Product : 

In the First load, all records have been inserted into the destination database without passing through any historization.
After the initial load, we refined our Product dimension with SCD Type 1 and Type 2 techniques. Now, it accurately reflects changes, ensuring our data mart provides valuable insights for decision-making. 
![Example](images/Product_Dim_First_Load.PNG)
![Example](images/Product_Dim_After_Making_Changes.PNG)


### ETL_Dim_Customer : 

### ETL_Dim_Territory : 
As part of the project, a lookup table was developed for ingesting territory data with full country names, enhancing the representation of territory data within the Sales Data Mart 
![Example](images/Territory_Dim.PNG)


### ETL_Dim_Date : 

### Fact_Sales_Full_Load : 

![Example](images/Fact_Table_Full_Load_Control_Flow.PNG)

![Example](images/Fact_Table_Full_Load_Data_Flow.PNG)

### Fact_Sales_Increamental_Load :
![Example](images/Fact_Table_Increamental_Load_Control_flow.PNG)

![Example](images/Fact_Table_Full_Load_Data_Flow.PNG)


