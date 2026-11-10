# Azure Storage Types

Azure provides different storage services depending on **what kind of data you need to store and how you want to use it**.

## 1. Azure Blob Storage

**Blob Storage** stores unstructured data, such as images, videos, PDFs, backups, and log files.

Imagine your website allows customers to upload photos. You can store those photos in Azure Blob Storage instead of keeping them on your own server.

It's called **object storage**, and applications typically access it through HTTP or HTTPS.

**Remember:** Blob Storage → Images, videos, documents, and other unstructured data.

## 2. Azure Files

**Azure Files** provides shared folders in the cloud.

Imagine your company has 20 employees who need access to the same documents. Azure Files allows them to access a shared file system without maintaining a traditional file server.

It supports file-sharing protocols such as **SMB** and can be mounted by Azure VMs or supported on-premises computers.

**Remember:** Azure Files → Shared folders and network drives.

## 3. Azure Queue Storage

**Queue Storage** holds messages that applications need to process.

Imagine a customer places an order on your website.

Instead of processing everything immediately, the website places an order message into a queue. A background application processes it later.

This is called **asynchronous processing**, meaning tasks don't have to be completed immediately.

It also helps **decouple applications**, allowing different parts to work independently.

**Remember:** Queue Storage → Messages waiting to be processed.

## 4. Azure Table Storage

**Table Storage** stores structured, non-relational data using a NoSQL model.

Unlike a traditional SQL database, it doesn't require every record to have the same set of columns.

For example, an application can store user profiles, application information, or device data.

Azure identifies each record using a **PartitionKey** and **RowKey**.

**Remember:** Table Storage → Flexible NoSQL data without traditional relational tables.

## 5. Azure Managed Disks

**Azure Managed Disks** provide storage for Azure Virtual Machines.

Just like your laptop needs a drive to store its operating system and files, an Azure VM needs a disk.

Azure manages the underlying storage infrastructure.

Managed Disks offer different performance options, including HDD and SSD storage.

Data persists when the VM is stopped or restarted.

**Remember:** Managed Disks → Storage for Azure VMs.

---

## Azure Storage Services — Quick Comparison

| Azure Service | What It Stores |
|---|---|
| **Blob Storage** | Photos, videos, PDFs, backups |
| **Azure Files** | Shared files and folders |
| **Queue Storage** | Messages between applications |
| **Table Storage** | Structured NoSQL data |
| **Managed Disks** | VM operating systems and application data |

### Main Takeaway

**Blob → Objects and files**

**Files → Shared folders**

**Queue → Messages**

**Table → NoSQL records**

**Disks → Virtual Machine storage**

For AZ-900, focus on understanding **which storage service matches a particular requirement**, rather than memorizing configuration details.


## Azure Blob Storage Access Tiers

Azure Blob Storage offers four access tiers based on **how often you need your data and how much you want to spend**.

Imagine your company stores thousands of customer photos. Some are accessed every day, while others haven't been opened in years.

Azure lets you store them in different tiers to save money.

### The Four Access Tiers

| Tier | When to Use | Storage Cost | Access Cost |
|---|---|---|---|
| **Hot** | Frequently accessed data | Highest | Lowest |
| **Cool** | Occasionally accessed data | Lower | Higher |
| **Cold** | Rarely accessed data | Even lower | Even higher |
| **Archive** | Almost never accessed data | Lowest | Highest, with retrieval delays |

### How They Work

**Hot →** Active application files, frequently viewed photos, and documents.

**Cool →** Older files or backups that are accessed occasionally but must remain immediately available.

**Cold →** Rarely accessed data that must still be available immediately.

**Archive →** Long-term historical records or backups that can wait hours for retrieval.

### Important Concepts

**Minimum Retention Period:** Cool, Cold, and Archive tiers have minimum storage durations. Moving or deleting data too early can result in additional charges.

**Rehydration:** Archive data must be moved back to an online tier before it can be read. This process can take hours and may incur additional costs.

**Lifecycle Management:** Azure can automatically move blobs between supported tiers based on rules you configure.

For example:

`Hot → Cool → Cold → Archive`

Different blobs in the same container can use different access tiers.

### ⭐ Easy Way to Remember

**Hot → I use it every day.**

**Cool → I use it sometimes.**

**Cold → I rarely use it.**

**Archive → I almost never use it, and I can wait to retrieve it.**

**Main takeaway:** The less frequently you access data, the cheaper it can be to store, but the more expensive or slower it may be to retrieve.

## Azure Storage Redundancy

**Redundancy means Azure keeps extra copies of your data to protect it from failures.**

The main difference between redundancy options is **where Azure keeps those copies**.

### 1. LRS — Locally Redundant Storage

Azure keeps **3 copies of your data in one datacenter** within a single region.

This protects against hardware failures, such as a failed disk or server, but not an entire datacenter failure.

**Remember:** LRS = One datacenter.

### 2. ZRS — Zone-Redundant Storage

Azure keeps **3 copies across different Availability Zones** within one Azure region.

If one zone fails, your data can remain available from another zone.

**Remember:** ZRS = Multiple zones, one region.

### 3. GRS — Geo-Redundant Storage

Azure keeps **3 copies in the primary region** and asynchronously replicates them to **3 additional copies in a secondary region**.

This helps protect against a regional disaster.

**Remember:** GRS = Two regions.

### 4. RA-GRS — Read-Access Geo-Redundant Storage

Works like GRS, but you can also **read data from the secondary region** without waiting for a failover.

**Remember:** RA-GRS = GRS + Read access to backup region.

### 5. GZRS — Geo-Zone-Redundant Storage

Combines ZRS and GRS.

Azure keeps copies across **3 Availability Zones in the primary region**, then replicates data to a secondary region.

This protects against both zonal and regional failures.

**Remember:** GZRS = Multiple zones + Another region.

### 6. RA-GZRS — Read-Access Geo-Zone-Redundant Storage

Works like GZRS, but allows **read access to the secondary region** without waiting for failover.

**Remember:** RA-GZRS = GZRS + Read access to backup region.

### Quick Comparison

| Type | Where Data Is Replicated |
|---|---|
| **LRS** | One datacenter |
| **ZRS** | Multiple zones in one region |
| **GRS** | Two regions |
| **RA-GRS** | Two regions + Secondary read access |
| **GZRS** | Multiple zones + Secondary region |
| **RA-GZRS** | Multiple zones + Secondary region + Read access |

### Important Concepts

**Synchronous replication:** Azure confirms a successful write after the required copies in the primary region are written.

**Asynchronous replication:** Data is copied to another region after the primary write, so the secondary region may temporarily have older data.

**RA (Read Access):** Allows reading from the secondary region. Writes still go to the primary region.

### Easy Way to Remember

**L = Local** → One datacenter.

**Z = Zone** → Multiple Availability Zones.

**G = Geo** → Multiple regions.

**RA = Read Access** → Read from the secondary region.

**Main takeaway:** Choose redundancy based on the failures you need protection against, not simply the option with the most copies.