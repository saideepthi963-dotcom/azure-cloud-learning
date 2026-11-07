# Azure Regions and Region Pairs

## 1. What Is an Azure Region?

An **Azure Region** is a geographical area containing one or more Microsoft datacenters connected through a low-latency network.

Microsoft operates physical datacenters worldwide to provide Azure services.

When creating resources such as Virtual Machines, you usually select the Azure region where they will run.

**Examples:**
- East US
- Canada Central
- North Europe

### Why Are Azure Regions Important?

- **Low Latency:** Deploy applications closer to users to reduce communication delays.
- **Scalability:** Access computing resources across different geographical locations.
- **Redundancy:** Support backup and recovery architectures.
- **Data Residency:** Help organizations keep data within required geographical locations.

**Data Residency:** Keeping data in a specific geographical location to meet business or legal requirements.

### Important Points

- Some Azure services and VM sizes are available only in certain regions.
- Storage options and other features can also vary by region.
- Some global services don't require selecting a specific region.

**Examples of global services:**
- Microsoft Entra ID (formerly Azure Active Directory)
- Azure Traffic Manager
- Azure DNS

## 2. Special Azure Regions

Special regions are designed for organizations with specific legal, government, or compliance requirements.

| Special Region | Purpose |
|---|---|
| US Gov Virginia | Azure Government services |
| US Gov Iowa | Azure Government region referenced in the lecture |
| US DoD Central | Government and defense workloads |
| China East | Azure services in China |
| China North | Azure services in China |

**Azure Government:**
- Provides isolated cloud environments for eligible government organizations and partners.
- Uses screened US personnel for applicable operations.
- Supports additional compliance requirements.

**Azure China:**
- Operated by **21Vianet** through a partnership with Microsoft.
- Uses infrastructure separate from the global Azure cloud.

## 3. What Are Azure Region Pairs?

A **Region Pair** is an arrangement in which Microsoft associates two Azure regions to support certain reliability and disaster recovery capabilities.

Traditionally, paired regions are:
- Located within the same geography, with some exceptions.
- Often separated by hundreds of miles.
- Used by certain Azure services for geographical redundancy.

**Example:** East US ↔ West US

### Why Are Region Pairs Useful?

**1. Disaster Recovery**
- Some services can replicate data to another region.
- Helps protect against major regional disasters.

**2. Planned Updates**
- Microsoft aims to update paired regions at different times.
- Helps reduce the risk of both regions being affected by the same update problem.

**3. Recovery Priority**
- During a major outage, Microsoft may prioritize recovering one region in a pair.

**4. Data Residency**
- Most region pairs are within the same geography.
- This can help organizations meet data location requirements.

### Important Clarification

Not all Azure regions have a region pair.

Also, **region pairing does not automatically provide failover**. Applications must use supported replication and recovery configurations.

For example, Azure Geo-Redundant Storage (GRS) can automatically replicate data to a paired region.

## 4. Azure Region vs. Region Pair

| Azure Region | Azure Region Pair |
|---|---|
| A geographical area containing datacenters | Two associated Azure regions |
| Used to deploy cloud resources | Supports certain cross-region reliability features |
| Helps reduce latency | Helps support disaster recovery |
| Helps meet data residency requirements | Can support geographical redundancy |

## ⭐ Important AZ-900 Exam Points

- **Azure Region:** Geographical area containing one or more datacenters.
- **Low Latency:** Reduced delay in communication.
- **Data Residency:** Keeping data in a required geographical location.
- **Special Regions:** Support specific government or legal requirements.
- **Region Pair:** Two associated regions used for certain redundancy and recovery capabilities.
- **Geo-Redundancy:** Maintaining data copies across geographically separated locations.
- **Availability Zones:** Separate datacenter groups within a region; regions supporting zones have at least three.

### Easy Way to Remember

**Azure Region → Where your resources are deployed.**

**Region Pair → Helps support cross-region redundancy and disaster recovery.**

**Availability Zone → Helps protect against datacenter failures within a region.**