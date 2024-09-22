# Describe Features and tools for managing and deploying Azure resources 


## Introduction

This module introduces you to features and tools for managing and deploying Azure resources. You will learn about the Azure portal (a graphic interface for managing Azure resources), the command line, and scripting tools that help deploy or configure resources. Additionally, you'll explore Azure services that help manage your on-premises and multicloud environments.

### Learning Objectives:
- Describe the Azure portal.
- Describe Azure Cloud Shell, including Azure CLI and Azure PowerShell.
- Describe the purpose of Azure Arc.
- Describe Azure Resource Manager (ARM), ARM templates, and Bicep.

---

## Tools for Interacting with Azure

To manage your Azure environment, including resources and subscriptions, you have multiple tools at your disposal:

### Azure Portal:
- A web-based unified console for managing your Azure subscription using a graphical user interface.
- **Features:**
  - Build, manage, and monitor resources from simple apps to complex deployments.
  - Customizable dashboards for resource views.
  - Continuous availability, resilient to datacenter failures, with no downtime for maintenance.

### Azure Cloud Shell:
- A browser-based shell tool available via the Azure portal. It supports both Azure PowerShell and Azure CLI (Bash).
- **Features:**
  - No installation required; accessed via browser.
  - Authenticated with your Azure credentials for immediate access to resources.
  - Supports both PowerShell and CLI, allowing you to use the shell you're familiar with.

### Azure PowerShell:
- A shell for developers, DevOps, and IT pros to run commands (cmdlets) that call the Azure REST API for managing resources.
- **Use Cases:**
  - Managing infrastructure via scripts for repeatable tasks.
  - Available via Azure Cloud Shell or installed locally on Windows, Linux, or Mac.

### Azure CLI:
- Equivalent in functionality to Azure PowerShell but uses Bash commands.
- **Features:**
  - Perform discrete tasks or orchestrate complex operations.
  - Installable on Windows, Linux, Mac, or available through Azure Cloud Shell.
  - Choice between Azure PowerShell and CLI is based on user preference for syntax.

---


## Azure Arc

Managing hybrid and multi-cloud environments can be complex. Azure Arc helps simplify governance and management across these environments by projecting non-Azure resources into Azure Resource Manager (ARM).

### Key Features:
- **Unified Management**: Manage on-premises, multicloud, and hybrid environments as if they were Azure resources.
- **Supported Resources**: Servers, Kubernetes clusters, Azure data services, SQL Server, and Virtual Machines (preview).

Azure Arc allows you to:
- Manage non-Azure resources alongside Azure resources.
- Use Azure services and management capabilities across environments.
- Introduce DevOps practices alongside traditional IT operations.

---



## Azure Resource Manager (ARM) and ARM Templates

Azure Resource Manager (ARM) is the deployment and management service for Azure. It handles all requests for Azure resources via the Azure portal, CLI, APIs, or SDKs.

### ARM Benefits:
- **Declarative Templates**: Manage your infrastructure via JSON templates instead of scripts.
- **Resource Grouping**: Manage and monitor resources as a group rather than individually.
- **Repeatable Deployments**: Deploy infrastructure consistently throughout the development lifecycle.
- **Tagging and Billing**: Apply tags to resources to organize and track costs.

### Infrastructure as Code:
- **ARM Templates**: Describes resources in a declarative JSON format. Templates ensure consistent deployment and automate resource creation.
- **Bicep**: A language similar to ARM templates but more concise and easier to read. Bicep provides modularity and orchestration features.

#### Key Benefits of ARM Templates and Bicep:
- **Declarative Syntax**: No need to write commands—just declare what you want.
- **Orchestration**: ARM deploys interdependent resources in the correct order.
- **Modularity**: Break templates into smaller components for reusability.
- **Extensibility**: Include PowerShell or Bash scripts for additional setup during deployments.

---



## Knowledge Check

1. **What service helps you manage your Azure, on-premises, and multicloud environments?**
   - **Answer**: Azure Arc, working with Azure Resource Manager (ARM), helps manage hybrid and multicloud configurations.
   
2. **What two components could you use to implement infrastructure as code deployments?**
   - **Answer**: Bicep and ARM Templates.

---



## Summary

In this module, you learned about the features and tools for managing and deploying Azure resources, including:
- The **Azure portal** for graphical management.
- **Azure Cloud Shell** for CLI-based management using PowerShell or Bash.
- **Azure Resource Manager (ARM)** for deployment and management of resources.
- **Bicep** and **ARM templates** for implementing infrastructure as code.

### Learning Objectives Recap:
- Describe the Azure portal.
- Describe Azure Cloud Shell, including Azure CLI and Azure PowerShell.
- Describe Azure Resource Manager (ARM), ARM templates, and Bicep.

---

## Additional Resources

- **Implement Resource Management Security in Azure**:  
  A Microsoft Learn path for more information on managing Azure resources.  
  [Learn More](https://learn.microsoft.com/en-us/learn/paths/implement-resource-mgmt-security/)

