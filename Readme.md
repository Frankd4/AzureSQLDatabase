## Template Description

The ARM template defines the following resources:

- Azure SQL Server: Deploys an Azure SQL Server using the specified name, administrator login, and password.
- Elastic Pool: Creates an Elastic Pool within the Azure SQL Server. The pool has the "Standard" edition and allows for a minimum capacity of 0.5 and a maximum capacity of 2.
- Azure SQL Database: Deploys an Azure SQL Database within the Elastic Pool.
- The database has the "Standard" edition and uses the specified collation.
- It is associated with the Elastic Pool based on the provided `elasticPoolId`.


## Deployment Steps

Follow the steps below to deploy the Azure SQL Database into a Azure SQL Database Elastic Pool using the provided ARM template:

1. Navigate to the directory where the `ARM_Template_Add_AzureSQLDatabase_To_ElasticPool.json` file is located.
2. Customize the parameters in the `ARM_Template_Parameters_Add_AzureSQLDatabase_To_ElasticPool.json` file according to your requirements. The available parameters are as follows:

   - `databaseName`: Name of the new Azure SQL database.
   - `elasticPoolName`: Name of the existing or new Elastic Pool.
   - `serverName`: Name of the Azure SQL server.
   - `administratorLogin`: Administrator username for the Azure SQL server.
   - `administratorLoginPassword`: Administrator password for the Azure SQL server.

6. Deploy the ARM template by executing the following command, replacing `<resourceGroupName>` with the name of the resource group where you want to deploy the resources:
7. Wait for the deployment to complete. You can monitor the progress through the command-line interface or the Azure portal.

