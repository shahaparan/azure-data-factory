# Azure Data Factory Environment Setup

## Step-01: creating Azure Data factory

- Crearting Azure Data factory
- **Basics**
  - **Subscription:** Free Trial
  - **Resource Group:** Creat New: covid-rg1
  - **Region:** (US) Central US
  - **Name:** covid-reporting-adf
- **Git configure**
  - **configure Git Later:** yes
- **Networking**
  - Rest all leave to defaults
- **Tags**
  - leave to defaults
- **Review + Create**
  - Click on **Create**

## Step-02: creating Azure storage Account

- Creating Azure storage Account
- **Basics**
  - **Subscription:** pay-as-you-go
  - **Resource Group:** covid-rg1
  - **Region:** (US) Central US
  - **Storage Account Name:** covid-reporting-sa
  - **Redundancy:** LRS
  - leave to defaults
- **Review + Create**
  - Click on **Create**

## Step-03: Installing Azure storage explorer

- Go to https://azure.microsoft.com/en-us/products/storage/storage-explorer
- **Default Directory** - Click on **yes**

## Step-04: creating Azure Data Lake storage Account

- Creating Azure Data Lake storage Account
- **Basics**
  - **Subscription:** pay-as-you-go
  - **Resource Group:** covid-rg1
  - **Region:** (US) Central US
  - **Storage Account Name:** covid-reporting-datalake
  - **Redundancy:** LRS
  - leave to defaults
- **Advanced**
  - **Data Lake Storage Gen2:** Yes
- **Review + Create**
  - Click on **Create**

## Step-05: creating Azure SQL Database

- creating Azure SQL Database
- **Basics**

  - **Subscription:** pay-as-you-go
  - **Resource Group:** covid-rg1
  - **Region:** (US) Central US
  - **DB Name:** covid-db
  - **Server:** Create new
    - **Server Name:** covid-server
    - **Location:** (US) Central US
    - **Auth:** use SQL AUTH
    - **admin:** admin
    - **pasword:** admin
    - **password:** admin
  - **SQL EL POOL:** NO
  - **Workload Env:** Dev
  - **Compute + storage:** Configure database
    - **Service tier:** basic(for less demanding workloads)
  - **Backup storage redundancy** Locally

- **networking**
  - **Connectivity Method** Public access
  - **Firewall rules** allow Azure sericess & Current IP (YES)
  - leave to defaults
- **Review + Create**
  - Click on **Create**

## Step-06: Installing Azure studio

- https://learn.microsoft.com/en-us/sql/azure-data-studio/download-azure-data-studio?view=sql-server-ver16&viewFallbackFrom=sql-server-ver16%5C&tabs=redhat-install%2Credhat-uninstall
- **Connection**
  - **Server :** URL
  - **User name:** admin
  - **Database:** covid_db
  - **pasword:** admin
  - Click on **Create**
