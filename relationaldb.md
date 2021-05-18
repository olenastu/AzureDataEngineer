**BigData & AI Landscape 2020 https://mattturck.com/data2020/**

**Understand your relational databases, understand your data**
- Learn how to model data
- Data is your fuel, Azure is your rocket ship
- Always remember about data consumption (a well-designed db is a prerequisite for fast data retriewval and updates)
- Most data is stored in structured in relational db systems
- One of the foundation programming languages data engineers speak is *SQL*
- Normalization, ACID (atomicity, consistency, isolation, durability), Transactions, Constraints, Consistency.

**Azure Relational DB offering**
- Azure SQL https://azure.microsoft.com/en-us/products/azure-sql/database/ 
- Azure Synapse Analytics - mainly for DWH
- Azure DB for MySQL
- Azure DB for PostgreSQL
- Azure DB for MariaDB
- Azure DB for PostgreSQL - Hyperscale (Citus)

**AzureSQL**
- based ont he latest stable version of MS SQL DB - SQL Server 2019
- Fully managed
- Automatically replicated
- Compatible with existing TDS-capable software (i.e. SSMS, VS, Entity Framework)
- Managed using existing tools (CLI, Powershell etc)

*Offering: Managed Instance, Single and Elastic Pool*

**Azure SQL Reference Architectures**
 Basic Web Application https://docs.microsoft.com/en-us/azure/architecture/reference-architectures/app-service-web-app/basic-web-app?tabs=cli 
 ![image](https://user-images.githubusercontent.com/63510256/118671808-11014380-b7f8-11eb-9cd3-4df87bf39d30.png)

**What is SQL DB managed instance?**
- easy lift and shift
- fully managed PaaS
- full isolation and security
- new business model

**When to choose what?**
- *Scenario 1:* in case you are building a new application, cloud native application and just need a base functionality. The best solution will be Azure SQL DB (PaaS)
- *Scenario 2:* If you move application from on -prem and you need SQL agent or CLR, the best option will be Azure SQL MI (PaaS)
- *Scenario 3:* You need SSAS/SSIS, and SQL agent/CLR and you are dependent on specific SQL Server version - you should use SQL Server on VM (IaaS)
