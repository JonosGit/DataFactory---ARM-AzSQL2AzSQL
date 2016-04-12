# Data-Factory---ARM AzSQL2AzSQL Templates for Azure SQL to Azure SQL Data Factory Pipelines


DF-AzSql2AzSql.json - ARM Template to deploy Azure SQL to Azure SQL Pipeline
DF-AzSql2AzSql_Answer.json - ARM Answer File to automate DF-AzSql2AzSql.json deployment

To Execute the template run the following commands in Azure Powershell 1.x or greater after downloading the ARM template to C:\Temp. Note you will need to update the Template Parameter File if you decide to use it.

Login-AzureRMAccount
New-AzureRmResourceGroup -Location "WESTUS" -Name "DataFactory"

New-AzureRmResourceGroupDeployment -ResourceGroupName "DataFactory" -TemplateFile C:\Temp\DF-AzSql2AzSql.json -TemplateParameterFile C:\Temp\DF-AzSql2AzSql_Answer.json