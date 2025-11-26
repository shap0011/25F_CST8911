# Lab #5: SQL Databases

**Student: Olga Durham**

**Student#: 040687883**

---

# Prerequisites:

Download SQL Server Management Studio (SSMS) or Azure Data Studio in order to complete this lab

https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16

https://learn.microsoft.com/en-us/azure-data-studio/download-azure-data-studio?tabs=win-install%2Cwin-user-install%2Credhat-install%2Cwindows-uninstall%2Credhat-uninstall#download-azure-data-studio

---

# Complete the Tasks

1. Create a sql database with the ability to use both SQL and Microsoft Entra authentication to login. Create for development workload environment, select locally redundant backup storage /5

Subscription: `Azure for Students`

Resource group: `8911lab5rg`

Location: `Canada central`

Database name: `SQLAuthLab5DB`

Server name: `sqllab5server`

Authentication method: `Use both SQL and Microsoft Entra authentication`

Server admin login: `sqladminolga`

Password: `olga%durham25`

Microsoft Entra Admin: `shap0011@algonquinlive.com`

Compute + storage: `General Purpose - Serverless Standard series (Gen5), 1 vCore, 32 GB storage, zone redundant disabled`

Workload environment: `Development`

Backup storage redundancy: `Locally redundant backup storage`

2. Login to the database using SQL Server Management Studio (SSMS) or Azure Data Studio using both Microsoft authentication to install and sql login to the database created in step 1 /10

Login failed with error: `Cannot connect to sqllab5server.database.windows.net. Reason: An instance-specific error occurred while establishing a connection to SQL Server. Connection was denied because Deny Public Network Access is set to Yes.(Microsoft SQL Server, Error: 47073)`

The public network access needs to be turned `on`

_NOTE: The screenshot available in the "Screenshot. Step 2. Section"_

3. Delete sql database and any other resources created /5

---

# Screenshots:

## Step 1:

- Screenshots must include each step of the creation of the azure SQL database and server specifically focused on the of workload environment, and if the right checkboxes were selected to allow both SQL and Microsoft Entra authentication. Any additional settings that are relevant that would allow you to sign in and any permissions that might need to be given to allow you to login for step 2, should also be included.

**Start creating new SQL database**

<img src="./screenshots/1_open_azure_sql_databases_create.png" alt="" title="Start creating new SQL database" width="500"/>

**Create SQL Database Server Setting**

<img src="./screenshots/2_create_server_setup.png" alt="" title="Create SQL Database Server Setting" width="700"/>

**Create SQL Database Setting**

<img src="./screenshots/3_create_database_setting.png" alt="" title="Create SQL Database Setting" width="700"/>

**New database and server deployed to resource group**

<img src="./screenshots/4_database_created.png" alt="" title="New database and server deployed to resource group" width="500"/>

**Resource group overview**

<img src="./screenshots/5_resource_group_server_database_created.png" alt="" title="Resource group overview" width="1100"/>

**SQL server overview**

<img src="./screenshots/6_sql_server_created.png" alt="" title="SQL server overview" width="1100"/>

**SQL database overview**

<img src="./screenshots/7_sql_database.png" alt="" title="SQL database overview" width="1100"/>

## Step 2:

- Screenshot of the credentials being inputted to sign in via SQL login(username and password) and following result that you were able to sign in being shown as well

**Edit the Server Networking setting**

<img src="./screenshots/10_edit_network_setting.png" alt="" title="Edit the server networking setting" width="1100"/>

**Network access and firewall rules updated**

<img src="./screenshots/11_updated_server_firewall_rules_server_public_network_access.png" alt="" title="Network access and firewall rules updated" width="400"/>

**Connection Properties setting**

<img src="./screenshots/9_connect_to_server.png" alt="" title="Connection Properties setting" width="700"/>

**Login setting**

<img src="./screenshots/8_connect_to_server.png" alt="" title="Login setting" width="700"/>

**SQL connection works**

<img src="./screenshots/12_sql_connect_work.png" alt="" title="SQL connection works" width="600"/>

**The database listed under databases**

<img src="./screenshots/13_database_listed_under_Databases.png" alt="" title="The database listed under databases" width="600"/>

- Screenshot of the credentials being inputted to sign in via Microsoft Entra ie authentication and following result that you were able to sing in being shown as well

**Entra Connection Properties setting**

<img src="./screenshots/14_set_network_protocol_to_tcp_ip.png" alt="" title="Entra Connection Properties setting" width="700"/>

**Entra Login setting**

<img src="./screenshots/15_login_setting.png" alt="" title="Entra Login setting" width="700"/>

**Entra login completed**

<img src="./screenshots/16_entra_login_completed.png" alt="" title="Entra login completed" width="600"/>

## Step 3:

- Screenshot of all resources being deleted

<img src="./screenshots" alt="" title="" width="500"/>

<img src="./screenshots" alt="" title="" width="500"/>
