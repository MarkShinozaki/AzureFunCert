# Describe Features and tools in Azure for Governance and Compliance 

## Introduction

In this module, you'll be introduced to features and tools for governance in your Azure environment. You'll also learn about tools to help keep resources in compliance with corporate or regulatory requirements.

### Learning Objectives

- Describe the purpose of Microsoft Purview.
- Describe the purpose of Azure Policy.
- Describe the purpose of resource locks.
- Describe the purpose of the Service Trust portal.

---

## Microsoft Purview

Microsoft Purview is a family of data governance, risk, and compliance solutions that provides a unified view into your data across on-premises, multicloud, and SaaS environments. It includes features for automated data discovery, sensitive data classification, and end-to-end data lineage.

### Key Features:
- **Risk and Compliance**: Protect sensitive data across clouds, manage data risks, and meet regulatory compliance.
- **Unified Data Governance**: Manage data across Azure, SQL, Hive, and other cloud services like Amazon S3.

Microsoft Purview helps organizations:
- Create a map of their entire data estate.
- Identify sensitive data.
- Securely manage data access and generate insights.

---

## Azure Policy

Azure Policy helps ensure your resources stay compliant with corporate standards. It enables you to create, assign, and manage policies that control or audit your resources. You can apply policies at different levels, such as resource groups or subscriptions, and they are inherited by lower levels.

### Key Concepts:
- **Policy Definitions**: Rules applied to your resources to enforce compliance.
- **Initiatives**: Groups of related policies. For example, the "Enable Monitoring in Azure Security Center" initiative includes policies for monitoring unencrypted databases and missing endpoint protection.

### Key Features:
- Azure Policy can automatically remediate non-compliant resources.
- Policies integrate with Azure DevOps to enforce policies during the deployment phases of your applications.

---

## Resource Locks

Resource locks prevent critical resources from being accidentally deleted or modified. Resource locks can be applied at the resource, resource group, or subscription level and are inherited by resources within the group.

### Types of Resource Locks:
- **Delete**: Prevents resource deletion while allowing modifications.
- **ReadOnly**: Prevents both deletion and modification.

Locks can be managed using the Azure portal, PowerShell, Azure CLI, or Azure Resource Manager templates. To modify or delete a locked resource, you must first remove the lock.

---

## Exercise - Configure a Resource Lock

In this exercise, you will create a storage account in Azure, apply a read-only lock, and observe the effects of the lock by attempting to modify the storage account.

### Steps:
1. Create a storage account in the Azure portal.
2. Apply a read-only resource lock.
3. Attempt to add a container (which will fail due to the lock).
4. Change the lock to "Delete" and add a container successfully.
5. Remove the lock and delete the storage account.

This exercise demonstrates how resource locks prevent accidental modifications or deletions.

---


## Service Trust Portal

The **Microsoft Service Trust Portal** provides access to content, tools, and resources related to Microsoft’s security, privacy, and compliance practices. It offers documentation on how Microsoft implements controls to protect cloud services and customer data.

### Key Features:
- **My Library**: Save documents and receive notifications when they are updated.
- **All Documents**: Access a full set of reports and resources related to Microsoft’s compliance practices.

You can access the portal at [https://servicetrust.microsoft.com/](https://servicetrust.microsoft.com/).

---


## Knowledge Check

1. **How can you prevent the creation of non-compliant resources?**
   - **Answer**: Azure Policy allows you to create policies and initiatives that prevent the creation of non-compliant resources.
   
2. **What's the best way to prevent the inadvertent deletion of a resource?**
   - **Answer**: Use a resource lock to prevent the resource from being deleted.

---



## Summary

In this module, you learned about features and tools to help with governance of your Azure environment. You explored how to keep resources in compliance with corporate or regulatory requirements.

### Learning Objectives Recap:
- Describe the purpose of Microsoft Purview.
- Describe the purpose of Azure Policy.
- Describe the purpose of resource locks.
- Describe the purpose of the Service Trust Portal.

---

# Additional Resources

- **Intro to Azure Policy**: A Microsoft Learn module that introduces you to Azure Policy.  
  [Learn More](https://learn.microsoft.com/en-us/learn/modules/intro-to-azure-policy/)
