# Azure Storage Accounts

## 1. What Is an Azure Storage Account?

An **Azure Storage Account** is a container that holds and organizes different types of data in Microsoft Azure.

Imagine your company needs to store customer photos, documents, application data, and shared files. Instead of maintaining physical storage servers, you can use Azure Storage.

A storage account provides a unique name and endpoints to access your data, including through HTTP or HTTPS.

### What Can You Store?

| Storage Service | Purpose |
|---|---|
| **Blob Storage** | Stores images, videos, documents, and other unstructured data |
| **Azure Files** | Provides shared file storage |
| **Queue Storage** | Stores messages exchanged between applications |
| **Table Storage** | Stores structured NoSQL data |

Azure also provides managed disks for virtual machines.

## 2. Types of Azure Storage Accounts

Azure offers **Standard and Premium storage accounts** depending on your performance requirements.

### Standard General-Purpose v2 (GPv2)

This is the most commonly recommended storage account for general use.

It supports Blob Storage (including Data Lake Storage), Azure Files, Queue Storage, and Table Storage.

**Best for:** Most everyday storage requirements.

### Premium Block Blob Storage

Designed for applications that require high transaction rates and consistently low storage latency.

**Best for:** Frequently accessed blobs, small objects, and high-performance applications.

### Premium File Shares

Provides high-performance file shares that support SMB and NFS protocols.

**Best for:** Enterprise applications requiring fast shared file storage.

### Premium Page Blobs

Designed specifically for workloads requiring high-performance page blob storage.

**Best for:** Specialized workloads that require page blobs.

## 3. Storage Redundancy

**Redundancy means keeping extra copies of data to protect against failures.**

Azure offers different redundancy options depending on the storage account type.

| Redundancy | Simple Meaning |
|---|---|
| **LRS** | Keeps copies within one physical location in a region |
| **ZRS** | Keeps copies across availability zones in one region |
| **GRS** | Replicates data to a secondary Azure region |
| **RA-GRS** | GRS with read access to the secondary region |
| **GZRS** | Combines zone redundancy with replication to another region |
| **RA-GZRS** | GZRS with read access to the secondary region |

The Standard GPv2 account supports the broadest range of these options.

Premium account types support fewer redundancy choices, depending on the service.

## 4. Storage Account Comparison

| Account Type | Supports | Best For |
|---|---|---|
| **Standard GPv2** | Blobs, Files, Queues, Tables | General-purpose storage |
| **Premium Block Blobs** | Block and append blobs | High transaction rates and low latency |
| **Premium File Shares** | Azure Files | High-performance file sharing |
| **Premium Page Blobs** | Page blobs | Specialized page blob workloads |

## 5. Storage SLAs

An **SLA (Service Level Agreement)** defines Microsoft's commitment to a service's availability.

Azure Storage has SLAs that vary depending on the service and configuration.

## Important AZ-900 Concepts

**Storage Account →** Holds and organizes Azure storage data.

**Standard GPv2 →** Suitable for most storage requirements.

**Premium Storage →** Designed for workloads needing higher performance.

**Redundancy →** Protects data by storing additional copies.

**SLA →** Microsoft's commitment to service availability.

**Main takeaway:** Choose an Azure storage account based on the type of data, required performance, and redundancy needs.