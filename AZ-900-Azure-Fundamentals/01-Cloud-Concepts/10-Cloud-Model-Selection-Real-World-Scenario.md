# Cloud Model Selection — Real-World Scenario

## 1. Scenario: Healthcare Organization

A healthcare organization wants to modernize its IT infrastructure.

**Current situation:**
- Operates two on-premises datacenters.
- Uses older applications (legacy applications).
- Must follow HIPAA healthcare data protection rules.
- Has limited disaster recovery capabilities.
- Physical infrastructure is aging.
- Hardware maintenance costs are increasing.

**Main challenge:** Modernize IT infrastructure without risking downtime, data security, or compliance violations.

The organization must evaluate Public, Private, and Hybrid Cloud.

## 2. Evaluating Cloud Deployment Models

### Public Cloud (Microsoft Azure)

**Advantages:**
- Resources can scale based on demand.
- Reduces physical hardware maintenance.
- Provides access to Azure regions and availability zones.
- Offers published Service Level Agreements (SLAs).

**Challenges:**
- Older applications may require changes before migration.
- Moving everything at once increases migration risk.
- Requires testing and updated security and governance processes.
- Compliance responsibilities still exist.

**Conclusion:** Public Cloud offers scalability and reduced infrastructure management, but moving everything immediately may introduce operational risks.

### Private Cloud

**Advantages:**
- Greater infrastructure control.
- Familiar security and management processes.
- Clear control over where data is stored.
- Less disruption to existing operations.

**Challenges:**
- Requires continued hardware investment.
- Hardware maintenance and replacement remain necessary.
- Scalability is limited by available infrastructure.
- Geographic redundancy may require additional datacenters.

**Conclusion:** Private Cloud maintains control but does not fully solve the organization's cost and disaster recovery challenges.

### Hybrid Cloud

**Advantages:**
- Allows gradual migration to Azure.
- Sensitive workloads can remain on-premises.
- Other applications can move to Azure.
- Supports improved disaster recovery.
- Allows workload placement based on security, performance, and cost.

**Challenges:**
- Requires managing both on-premises and Azure environments.
- Needs secure connectivity between environments.
- Identity, security monitoring, and governance must work across both.

**Conclusion:** Hybrid Cloud provides a balanced approach by allowing gradual modernization while reducing migration risks.

## 3. Azure Services Supporting Disaster Recovery

| Azure Service | Purpose |
|---|---|
| **Azure Backup** | Backs up data and workloads so they can be restored. |
| **Azure Site Recovery** | Replicates workloads and helps recover applications during outages. |

These services can improve disaster recovery without requiring organizations to build another physical datacenter.

## 4. Reliability and Predictability

### Reliability

**Reliability means keeping applications working and recovering from failures.**

Traditional on-premises environments may depend on manual recovery and local infrastructure.

Azure can improve reliability through:
- Availability Zones
- Geographic redundancy
- Data replication
- Designed failover processes
- Service Level Agreements (SLAs)

**Key Point:** Azure allows organizations to design recovery solutions instead of relying only on manual fixes.

### Predictability

**Predictability means being able to estimate performance and costs.**

Traditional infrastructure requires:
- Large upfront hardware purchases.
- Planning capacity years in advance.
- Paying for unused infrastructure.

Azure provides:
- Consumption-based pricing.
- Cost forecasting and monitoring tools.
- Autoscaling to adjust resources based on demand.

**Key Point:** Azure makes it easier to plan resource usage and costs, although actual spending can still change.

## 5. How to Choose the Right Cloud Model

| Business Requirement | Cloud Model to Consider |
|---|---|
| Rapid deployment and scalability | Public Cloud |
| Unpredictable resource demand | Public Cloud |
| Dedicated infrastructure and strict control | Private Cloud |
| Gradual migration of existing applications | Hybrid Cloud |
| Some workloads must remain on-premises | Hybrid Cloud |
| Existing infrastructure combined with Azure | Hybrid Cloud |
| Azure-based disaster recovery for on-premises systems | Hybrid Cloud |

**Important:** Compliance requirements do not automatically require Private Cloud. Public Cloud can also support regulated workloads when the necessary requirements are met.

## ⭐ Important AZ-900 Exam Points

- **Public Cloud:** Suitable for rapid scaling and reduced hardware management.
- **Private Cloud:** Suitable when dedicated infrastructure and greater control are priorities.
- **Hybrid Cloud:** Suitable for gradual migration and combining existing infrastructure with Azure.
- **Legacy Applications:** Older applications that may require changes before moving to the cloud.
- **Disaster Recovery:** Restoring applications and services after failures.
- **Azure Backup:** Protects data through backups.
- **Azure Site Recovery:** Supports workload replication and disaster recovery.
- **SLA (Service Level Agreement):** Defines Microsoft's service availability commitments.
- **Cloud Model Selection:** Depends on security, compliance, reliability, scalability, and cost requirements.

### Remember for the Exam

**Rapid Scaling → Public Cloud**

**Dedicated Infrastructure → Private Cloud**

**Gradual Migration → Hybrid Cloud**

**Disaster Recovery → Azure Backup / Azure Site Recovery**

**Main Takeaway:** Choosing the right cloud model is about understanding business requirements, not just memorizing definitions.