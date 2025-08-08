---
description: 
page_type: sample
products:
- azure
- azure-resource-manager
urlFragment: azure_servicenow_mid_server_single
languages:
- json
- bicep
---
# azure_servicenow_mid_server_single

[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#view/Microsoft_Azure_CreateUIDef/CustomDeploymentBlade/uri/https%3a%2f%2fsnowmiddeploy.blob.core.windows.net%2fsnowmid-azure-templates%2fazure_servicenow_mid_server_single%2fmainTemplate.json/uiFormDefinitionUri/https%3a%2f%2fsnowmiddeploy.blob.core.windows.net%2fsnowmid-azure-templates%2fazure_servicenow_mid_server_single%2fcreateUiDefinition.json)
[![Deploy To Azure Gov](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazuregov.svg?sanitize=true)](https://portal.azure.us/#view/Microsoft_Azure_CreateUIDef/CustomDeploymentBlade/uri/https%3a%2f%2fsnowmiddeploy.blob.core.windows.net%2fsnowmid-azure-templates%2fazure_servicenow_mid_server_single%2fmainTemplate.json/uiFormDefinitionUri/https%3a%2f%2fsnowmiddeploy.blob.core.windows.net%2fsnowmid-azure-templates%2fazure_servicenow_mid_server_single%2fcreateUiDefinition.json)
[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3a%2f%2fsnowmiddeploy.blob.core.windows.net%2fsnowmid-azure-templates%2fazure_servicenow_mid_server_single%2fmainTemplate.json)

Single ServiceNow MID Server deployment

This template uses Azure Resource Manager (ARM) templates compiled from Bicep source files to deploy ServiceNow MID Server infrastructure components.

## Template Details

- **Template Type**: Microsoft_Azure_CreateUIDef
- **Base Template**: azure_servicenow_mid_server_single
- **UI Definition**: uiFormDefinition.mid_server_single.json

## Prerequisites

Before deploying this template, ensure you have:

- An active Azure subscription
- Appropriate permissions to create resources in the target resource group
- ServiceNow instance credentials (if required by the template)

## Deployment

### Azure Portal

Click the "Deploy to Azure" button above to deploy this template through the Azure Portal with a guided UI experience.

### Azure CLI

```bash
az deployment group create \
  --resource-group myResourceGroup \
  --template-uri https://snowmiddeploy.blob.core.windows.net/snowmid-azure-templates/azure_servicenow_mid_server_single/mainTemplate.json \
  --parameters @parameters.json
```

### Azure PowerShell

```powershell
New-AzResourceGroupDeployment \
  -ResourceGroupName "myResourceGroup" \
  -TemplateUri "https://snowmiddeploy.blob.core.windows.net/snowmid-azure-templates/azure_servicenow_mid_server_single/mainTemplate.json" \
  -TemplateParameterFile "parameters.json"
```

## Parameters

Refer to the template's parameter file and UI definition for required and optional parameters.

## Resources Created

This template creates Azure resources as defined in the Bicep source file. Review the compiled ARM template for specific resource details.

`Tags: servicenow, mid-server, azure, infrastructure, bicep, arm-template`
