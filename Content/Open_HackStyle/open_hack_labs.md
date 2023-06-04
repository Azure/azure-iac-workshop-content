# Advanced Content (Optional)

## Overview

The labs defined in this document are more of an `open hack` style approach to challenge  students after they've learnt the fundamentals of Bicep.

add a points system / bonus points for harder things (E.g. system identity > keyvault access | load secret from KeyVault)

## Challenges

These changes are all based on a build-your own adventure style challenge. Look through all of the options available for each Azure resource and decide what to apply.

> *Note:* All the challenges below should be completed by using Bicep. They can be performed in any order.

<br>

> *Tip:* At the bottom of each documentation section is the quick start guide.

<br>

### 1 - Virtual Network

Create an Azure Virtual Network with:

- At least two subnets
- A network security group
- A Route table

Bonus:

- Network Security Group Flow Logs Enabled (pushing to a storage account)

> *Documentation:* [Virtual Network](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/virtualnetworks?pivots=deployment-language-bicep)

<br>

### 2 - Azure Function

Create an Azure Function App that runs a function. This function app must be connected to application insights, exposes diagnostic logs to a Log Analytics Workspace and uses an Azure KeyVault as a reference for an App Setting variable.

> *Documentation:* [Azure Function](https://learn.microsoft.com/en-us/azure/templates/microsoft.web/sites?pivots=deployment-language-bicep)

<br>

### 3 - Virtual Machine Scale Set

**Prerequisite**: An Azure Virtual Network needs to be created before starting this.

Create an Azure Virtual Machine Scale set that uses:

- Operating System: Linux
- Disk 32GB
- Use an extension (any)
- Reference the password from an Azure KeyVault ([Reference secret example](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/bicep-functions-resource#getsecret))

> *Documentation:* [VMSS](https://learn.microsoft.com/en-us/azure/templates/microsoft.compute/virtualmachinescalesets)

<br>

### 4 - Azure Kubernetes Service cluster

Create an AKS cluster with a single node pool.

- Optional - add a secondary `user` node pool
- Use a Linux Operating system

> *Documentation:* [AKS](https://learn.microsoft.com/en-us/azure/templates/microsoft.containerservice/managedclusters)

<br>

### 5 - Azure SQL Databases

Create an Azure SQL server and multiple databases on this server. Consider using Bicep loops for deploying the databases.

- Consider the SQL audit logs
- Backup retention
  - Could an `environment` parameter be used to set the backup retention?

> *Documentation:* [Azure SQL](https://learn.microsoft.com/en-us/azure/templates/microsoft.sql/servers?pivots=deployment-language-bicep)
