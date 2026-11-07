# Infrastructure as a Service (IaaS)

## 1. What Is IaaS?

**Infrastructure as a Service (IaaS)** is a cloud service model that provides computing resources over the internet on demand.

These resources include:
- **Compute:** Virtual machines and processing power.
- **Storage:** Space to store files and data.
- **Networking:** Resources that connect systems and applications.

IaaS typically follows a **pay-as-you-go pricing model**, meaning you pay based on the resources you use.

**Example:** Azure Virtual Machines.

## 2. Who Manages What in IaaS?

In IaaS, Microsoft provides and manages the underlying physical infrastructure.

| Microsoft Manages | Customer Manages |
|---|---|
| Physical datacenters | Guest operating systems (Windows/Linux) |
| Physical servers | OS updates |
| Physical networking | Middleware |
| Underlying virtualization | Applications |
| Physical hardware maintenance | Data and security configurations |

**Middleware:** Software that helps applications communicate or operate.

**Remember:** Microsoft manages the physical infrastructure, while you manage the operating systems, middleware, applications, and data running on it.

## 3. Benefits of IaaS

- **Lower upfront costs:** No need to purchase physical servers.
- **Scalability:** Increase or decrease resources based on demand.
- **Faster Deployment:** Quickly create virtual machines and other resources.
- **Reduced Maintenance:** Microsoft maintains the physical infrastructure.
- **Reliability:** Azure infrastructure supports reliable workloads when appropriately configured.
- **Flexible Pricing:** Pay for resources according to their usage and pricing rules.

## 4. Common Business Use Cases

### 1. Lift-and-Shift Migration
Move existing applications from on-premises infrastructure to Azure **without major changes to their architecture**.

- Faster migration.
- Avoids completely rebuilding applications.
- Reduces physical infrastructure management.

### 2. Development and Testing
- Quickly create test environments.
- Remove environments when no longer needed.
- Scale resources based on testing requirements.

### 3. Storage, Backup, and Recovery
- Store data without purchasing physical storage hardware.
- Support backup and recovery requirements.
- Reduce physical storage management.

### 4. Web Applications
- Host websites and applications using cloud infrastructure.
- Deploy applications quickly.
- Scale servers and networking resources when needed.

### 5. High-Performance Computing (HPC)
Use powerful computing resources to solve complex problems involving large amounts of calculations.

**Examples:**
- Weather forecasting
- Earthquake simulations
- Protein folding
- Financial modeling

## ⭐ Important AZ-900 Exam Points

- **IaaS = Compute + Storage + Networking.**
- Provides resources on demand.
- Usually follows consumption-based pricing.
- Microsoft manages the underlying physical infrastructure.
- Customers manage guest operating systems, middleware, applications, and data.
- **Lift-and-Shift:** Move applications to the cloud without major architectural changes.
- IaaS is useful for development, testing, web hosting, backups, and high-performance computing.
- IaaS provides greater infrastructure control than PaaS and SaaS, but also requires more customer management.

**Easy Way to Remember:**

**IaaS → Microsoft provides the infrastructure. You manage what runs on it.**