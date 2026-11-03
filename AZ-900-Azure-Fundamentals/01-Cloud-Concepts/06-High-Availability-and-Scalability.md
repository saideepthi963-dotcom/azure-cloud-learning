# High Availability and Scalability in Azure

High Availability and Scalability are two important benefits of Azure. They help applications stay reliable, handle changing demand, and reduce costs.

## 1. High Availability (HA)

**High Availability means keeping applications running even when hardware fails or maintenance occurs.**

Azure uses **redundancy** (multiple resources working as backups) to reduce downtime.

Azure can distribute workloads across different servers, racks, and datacenters.

### How Azure Provides High Availability

**1. Availability Sets**
- Distribute Virtual Machines (VMs) across:
  - **Fault Domains:** Protect against hardware failures.
  - **Update Domains:** Reduce downtime during planned maintenance.
- Help prevent all VM instances from being affected by the same failure or maintenance event.

**2. Availability Zones**
- Physically separate datacenter groups within the same Azure region.
- Each zone has independent power, cooling, and networking.
- Help applications remain available if one zone fails, when appropriate redundancy and failover are configured.

### Benefits
- Less downtime
- Better reliability
- Faster recovery from failures
- Reduced impact of maintenance

## 2. Scalability

**Scalability means increasing or decreasing computing resources based on demand.**

For example, when website traffic increases, more computing resources can be added. When traffic decreases, unnecessary resources can be removed.

### Types of Scaling

| Type | Meaning |
|---|---|
| **Vertical Scaling** | Increase or decrease CPU/RAM of a resource |
| **Horizontal Scaling** | Add or remove resource instances |

### Azure Services Supporting Scalability

**1. Azure Virtual Machine Scale Sets**
- Manage multiple VM instances.
- Can automatically add VMs when CPU usage increases.
- Can remove extra VMs when demand decreases.

**2. Azure App Service**
- Hosts web applications.
- Supports automatic scaling based on demand.
- Helps applications handle changing traffic.

*Note: Automatic scaling must be supported and configured; it doesn't happen for every resource by default.*

## 3. Cost Benefits of Scalability

In traditional datacenters, companies purchase enough hardware to handle their highest expected demand, even when it is rarely needed.

With Azure:
- Increase resources during busy periods.
- Reduce resources during low-demand periods.
- Avoid purchasing unnecessary physical hardware.
- Reduce costs by removing unused capacity.

Actual savings depend on resource configuration and pricing.

## 4. High Availability vs. Scalability

| High Availability | Scalability |
|---|---|
| Handles infrastructure failures | Handles changing demand |
| Focuses on reliability | Focuses on resource capacity |
| Reduces downtime | Helps maintain performance |
| Availability Sets and Zones | VM Scale Sets and App Service |

## ⭐ Important AZ-900 Exam Points

- **High Availability:** Keeps applications accessible during failures.
- **Redundancy:** Uses multiple resources to reduce the impact of failures.
- **Fault Domain:** Protects against certain hardware failures.
- **Update Domain:** Reduces the impact of planned maintenance.
- **Availability Zone:** Physically separate datacenter infrastructure within an Azure region.
- **Scalability:** Increases or decreases resources based on demand.
- **Vertical Scaling:** Scale up/down (CPU, RAM).
- **Horizontal Scaling:** Scale out/in (number of instances).
- **Autoscaling:** Automatically adjusts resources based on configured rules or demand.
- **Elasticity:** The ability to dynamically adjust resources as demand changes.

**Remember:**

**High Availability → Handles failures.**  
**Scalability → Handles demand.**  
**Elasticity → Adjusts resources dynamically.**