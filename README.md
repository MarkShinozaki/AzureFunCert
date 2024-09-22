# Describe Azure Storage Services 

This module introduces the Azure storage services, focusing on storage accounts, blob storage tiers, redundancy options, and tools for data migration.

## Learning Objectives
- Compare Azure storage services.
- Describe storage tiers.
- Describe redundancy options.
- Describe storage account types.
- Identify file movement options like AzCopy, Azure Storage Explorer, and Azure File Sync.
- Describe migration options including Azure Migrate and Azure Data Box.

---

## 1. Azure Storage Accounts

A storage account provides a unique namespace for your Azure storage data, accessible over HTTP/HTTPS. It is secure, highly available, durable, and scalable.

### **Key Azure Storage Account Types**
| Type                      | Support Services                                      | Redundancy Options                                  | Usage                                                                                                                                                     |
|---------------------------|------------------------------------------------------|----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard General-purpose v2| Blob Storage, Queue Storage, Table Storage, Azure Files| LRS, GRS, RA-GRS, ZRS, GZRS, RA-GZRS               | Standard storage account type for blobs, file shares, queues, and tables. Supports both NFS and SMB in premium file shares.                                |
| Premium Block Blobs        | Blob Storage                                         | LRS, ZRS                                           | Recommended for scenarios with high transaction rates or smaller objects, or requiring low storage latency.                                                |
| Premium File Shares        | Azure Files                                          | LRS, ZRS                                           | Recommended for enterprise applications. Supports SMB and NFS.                                                                                            |
| Premium Page Blobs         | Page Blobs only                                      | LRS                                                | Premium storage for page blobs.                                                                                                                           |

### **Storage Account Endpoints**
Each storage account has a unique namespace in Azure. The endpoint format for Azure services is as follows:

| Storage Service         | Endpoint Format                                          |
|-------------------------|----------------------------------------------------------|
| Blob Storage            | https://\<storage-account-name>.blob.core.windows.net     |
| Data Lake Storage Gen 2  | https://\<storage-account-name>.dfs.core.windows.net     |
| Azure Files             | https://\<storage-account-name>.file.core.windows.net     |
| Queue Storage           | https://\<storage-account-name>.queue.core.windows.net    |
| Table Storage           | https://\<storage-account-name>.table.core.windows.net    |

---

## 2. Azure Storage Redundancy

Azure Storage replicates your data to ensure availability and durability. The available redundancy options include:

### **Redundancy Options**
- **Locally Redundant Storage (LRS)**: Replicates data three times within a single data center. Offers 99.999999999% durability.
- **Zone-Redundant Storage (ZRS)**: Replicates data across three availability zones. Offers 99.9999999999% durability.
- **Geo-Redundant Storage (GRS)**: Synchronously replicates data within one region and asynchronously to another.
- **Geo-Zone-Redundant Storage (GZRS)**: Combines ZRS in the primary region with LRS in a secondary region. Ensures maximum availability and protection.

### **Read-Access Options**
- **Read-Access Geo-Redundant Storage (RA-GRS)**: Provides read access to data in a secondary region if the primary is unavailable.
- **Read-Access Geo-Zone-Redundant Storage (RA-GZRS)**: Offers read access to the secondary region when using GZRS.

---

## 3. Azure Storage Services

The Azure Storage platform includes the following services:

- **Azure Blobs**: Massively scalable object storage for unstructured data, ideal for storing text or binary data.
- **Azure Files**: Managed file shares accessible through SMB or NFS protocols, can be mounted in cloud and on-premise environments.
- **Azure Queues**: Provides reliable message queuing for asynchronous workflows.
- **Azure Disks**: Block-level storage for Azure VMs.
- **Azure Tables**: NoSQL table storage for structured, non-relational data.

---

## 4. Azure Blob Storage Tiers

Azure Blob storage offers different access tiers to help balance storage costs based on usage patterns:

- **Hot**: For frequently accessed data.
- **Cool**: For data infrequently accessed and stored for at least 30 days.
- **Cold**: For data infrequently accessed and stored for at least 90 days.
- **Archive**: For rarely accessed data stored for at least 180 days, with longer retrieval times.

---

## 5. Azure Data Migration Options

Azure provides tools to migrate data into and within Azure:

### **Azure Migrate**
- Provides a unified platform to assess and migrate on-premises infrastructure to Azure.
- Integrated tools:
  - **Azure Migrate: Discovery and Assessment**
  - **Azure Migrate: Server Migration**
  - **Data Migration Assistant**
  - **Azure Database Migration Service**
  - **Azure App Service Migration Assistant**

### **Azure Data Box**
- Physical data migration service for moving large amounts of data to Azure.
- Transfers data using a proprietary storage device that supports up to 80 TB.
- Suitable for scenarios with limited network connectivity or large one-time data transfers.

---

## 6. Azure File Movement Options

Azure offers tools to move or interact with individual files or small groups of files:

- **AzCopy**: Command-line utility to copy files to and from Azure Storage.
- **Azure Storage Explorer**: GUI tool to manage Azure Storage resources (blobs, files, and queues).
- **Azure File Sync**: Synchronizes on-premises Windows file shares with Azure Files, offering centralized storage with local access.

---

## 7. Knowledge Check

1. Which tool automatically keeps files between an on-premises Windows server and an Azure cloud environment updated?
   - **Answer**: Azure File Sync

2. Which storage redundancy option provides the highest durability (16 nines)?
   - **Answer**: Geo-Zone-Redundant Storage (GZRS) or Geo-Redundant Storage (GRS)

3. Which Azure storage service supports big data analytics, as well as handling text and binary data?
   - **Answer**: Azure Blobs

---

## Summary

In this module, you learned about Azure Storage services, including the following:
- **Azure Storage Account types** and **endpoints**.
- **Storage redundancy options** such as LRS, ZRS, GRS, and GZRS.
- **Blob storage tiers** and their use cases (Hot, Cool, Cold, Archive).
- **Migration tools** such as Azure Migrate and Azure Data Box.
- **File movement tools** like AzCopy, Azure Storage Explorer, and Azure File Sync.

---

## Additional Resources
- **[Store data in Azure](https://learn.microsoft.com/en-us/learn/paths/store-data-in-azure/)**: Microsoft Learn course that covers more information about storing data in Azure.
- **[Microsoft Certified: Azure Data Fundamentals](https://learn.microsoft.com/en-us/learn/certifications/azure-data-fundamentals/)**: Certification course.

