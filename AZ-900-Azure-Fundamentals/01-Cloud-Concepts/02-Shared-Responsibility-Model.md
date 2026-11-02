# Shared Responsibility Model in Azure

**Certification:** Microsoft Azure Fundamentals (AZ-900)  
**Topic:** Cloud Computing Concepts

---

## 1. What Is the Shared Responsibility Model?

The **Shared Responsibility Model** defines how security and management responsibilities are divided between the cloud provider (Microsoft Azure) and the customer.

Moving to the cloud does not mean Microsoft manages everything.

Instead, both Microsoft and the customer are responsible for different aspects of the cloud environment.

**Key Concept:** Microsoft manages the underlying cloud infrastructure, while customers remain responsible for securing and managing their data, identities, and applicable configurations.

---

## 2. Responsibilities in On-Premises Infrastructure

In a traditional **on-premises environment**, organizations are responsible for managing and securing their entire IT infrastructure.

This includes:

- Physical datacenters and servers
- Networking equipment
- Firewalls
- Operating systems and updates
- Applications
- Data protection
- Access controls and security configurations

**Key Point:** In an on-premises environment, the organization is responsible for every layer of infrastructure and security.

---

## 3. Shared Responsibility in Cloud Service Models

When organizations move to Azure, some responsibilities shift to Microsoft.

The division depends on the cloud service model:

- **IaaS:** Infrastructure as a Service
- **PaaS:** Platform as a Service
- **SaaS:** Software as a Service

As you move from **IaaS → PaaS → SaaS**, Microsoft manages more components, reducing the customer's infrastructure management responsibilities.

### Infrastructure as a Service (IaaS)

**Example:** Azure Virtual Machines

Microsoft manages:
- Physical datacenters
- Physical servers
- Physical networking equipment
- Underlying virtualization infrastructure

The customer manages:
- Guest operating systems and updates
- Installed applications
- Application data
- Access controls
- Operating system and application security configurations

**Key Point:** In IaaS, Microsoft manages the physical infrastructure, but customers manage the operating systems, applications, and data deployed on it.

### Platform as a Service (PaaS)

**Examples:**
- Azure App Service
- Azure SQL Database

Microsoft manages:
- Physical infrastructure
- Operating systems
- Middleware
- Runtime environments
- Platform maintenance and updates

The customer manages:
- Applications and application code
- Data
- Access controls
- Application security configurations

**Key Point:** In PaaS, Microsoft manages the infrastructure and platform, allowing customers to focus on applications and data.

### Software as a Service (SaaS)

**Example:** Microsoft 365

Microsoft manages:
- Physical infrastructure
- Operating systems
- Application platform
- Application maintenance
- Software updates

The customer manages:
- User identities and access
- User data
- Permissions
- Applicable security settings
- Multifactor Authentication (MFA)
- Conditional Access configurations

**Key Point:** In SaaS, Microsoft manages nearly the entire application environment, while customers remain responsible for their users, data, and access configurations.

---

## 4. Comparison of Responsibilities

| Responsibility | On-Premises | IaaS | PaaS | SaaS |
|---|---|---|---|---|
| Physical datacenters | Customer | Microsoft | Microsoft | Microsoft |
| Physical servers | Customer | Microsoft | Microsoft | Microsoft |
| Physical networking | Customer | Microsoft | Microsoft | Microsoft |
| Operating systems | Customer | Customer | Microsoft | Microsoft |
| Middleware and runtime | Customer | Customer | Microsoft | Microsoft |
| Application management | Customer | Customer | Customer | Microsoft |
| Data protection | Customer | Customer | Shared* | Shared* |
| Identity and access management | Customer | Customer | Shared* | Shared* |

*Shared responsibilities vary by service and configuration. Customers remain responsible for their data and user access, while Microsoft provides and secures the underlying managed services.*

### Responsibility Progression

**On-Premises → IaaS → PaaS → SaaS**

- On-Premises: Customer manages everything.
- IaaS: Microsoft manages the underlying infrastructure.
- PaaS: Microsoft manages infrastructure and the application platform.
- SaaS: Microsoft manages infrastructure, platform, and software.

**Remember:** Customer infrastructure management responsibilities generally decrease from IaaS to SaaS.

---

## 5. Why Is the Shared Responsibility Model Important?

Understanding this model helps organizations:

1. **Prevent security gaps:** Know which security responsibilities belong to the customer.
2. **Avoid unnecessary management:** Do not spend time maintaining components already managed by Microsoft.
3. **Improve security:** Ensure applications, identities, and data are properly protected.
4. **Choose appropriate cloud services:** Understand the management requirements of IaaS, PaaS, and SaaS.

---

## 6. Important AZ-900 Exam Points

- The Shared Responsibility Model defines responsibilities between Microsoft and the customer.
- **On-Premises:** The customer manages the entire infrastructure.
- **IaaS:** Customers manage guest operating systems, applications, and data.
- **PaaS:** Microsoft manages operating systems and runtime environments; customers focus on applications and data.
- **SaaS:** Microsoft manages the software and underlying infrastructure; customers manage their data, identities, and applicable access settings.
- Microsoft is responsible for the physical security of Azure datacenters.
- Customers remain responsible for their data and access management across cloud service models.
- The customer has the greatest infrastructure management responsibility in **IaaS** compared with PaaS and SaaS.

---

## 7. Quick Revision

| Question | Answer |
|---|---|
| What is the Shared Responsibility Model? | Division of cloud security and management responsibilities between Microsoft and the customer. |
| Who manages physical Azure datacenters? | Microsoft |
| Who updates the guest OS in an Azure VM? | Customer |
| Who manages the OS in Azure App Service? | Microsoft |
| Who manages applications in SaaS? | Microsoft |
| Who manages customer data and user access? | Customer, with certain supporting responsibilities shared with Microsoft |
| Which cloud model gives customers the most infrastructure management responsibility? | IaaS |
| Which cloud model gives Microsoft the most management responsibility? | SaaS |

---

## 8. Lecture Summary

The Shared Responsibility Model explains how cloud management and security tasks are divided between Microsoft and the customer.

In **IaaS**, customers manage operating systems, applications, and data.

In **PaaS**, Microsoft additionally manages operating systems and runtime environments.

In **SaaS**, Microsoft manages the software and underlying infrastructure, while customers remain responsible for their data, users, and applicable security settings.

**Main Takeaway:** The more managed the cloud service model becomes, the fewer infrastructure management responsibilities remain with the customer.