# Cloud Deployment Models

**Certification:** Microsoft Azure Fundamentals (AZ-900)  
**Topic:** Cloud Computing Concepts

---

## 1. What Are Cloud Deployment Models?

Cloud deployment models define **where cloud resources are hosted, who manages them, and how they are accessed**.

There are three main cloud deployment models:

1. **Public Cloud**
2. **Private Cloud**
3. **Hybrid Cloud**

---

## 2. Public Cloud

A **Public Cloud** is a cloud environment where the infrastructure is owned and managed by a third-party cloud provider, such as Microsoft Azure.

Multiple customers share the underlying infrastructure, but their resources and environments remain logically isolated.

### Key Characteristics

- Infrastructure is owned and managed by the cloud provider.
- Multiple organizations share the underlying physical infrastructure.
- Customer environments are logically isolated through virtualization and identity controls.
- Cloud services are accessible over the internet.
- Resources are available on demand.
- Typically uses consumption-based pricing.
- Provides high scalability and cost efficiency.

### Example

A company uses **Microsoft Azure Virtual Machines** to host applications instead of purchasing physical servers.

The company pays for the Azure resources it consumes.

**Key Point:** Public Cloud = Shared infrastructure managed by a cloud provider.

---

## 3. Private Cloud

A **Private Cloud** is a cloud environment dedicated exclusively to a single organization.

Unlike a public cloud, its infrastructure is not shared with other organizations.

A private cloud can be:

- **On-premises:** Hosted in the organization's own datacenter.
- **Off-premises:** Hosted by an external service provider.

### Key Characteristics

- Dedicated infrastructure for one organization.
- Greater control over infrastructure and data.
- Supports strict security and compliance requirements.
- Provides cloud capabilities such as scalability and automation.
- Typically requires more infrastructure management.
- The organization generally has greater responsibility for hardware maintenance and security.

### Example

A bank operates a private cloud to maintain greater control over sensitive financial data and infrastructure.

**Key Point:** Private Cloud = Dedicated infrastructure for a single organization.

---

## 4. Hybrid Cloud

A **Hybrid Cloud** combines public and private cloud environments, allowing organizations to use both.

Organizations can decide where applications and data should be hosted based on their requirements.

### Key Characteristics

- Combines public and private cloud environments.
- Allows workloads to run in different environments.
- Provides flexibility in resource placement.
- Supports compliance and data control requirements.
- Allows organizations to use additional public cloud capacity when needed.
- Requires connectivity and coordination between environments.

### Example

A company:

- Stores sensitive databases in its private cloud.
- Uses Microsoft Azure Public Cloud to handle increased application traffic.

This allows the organization to maintain control over sensitive data while benefiting from public cloud scalability.

### Azure Technologies Supporting Hybrid Environments

| Technology | Purpose |
|---|---|
| VPN Gateway | Provides encrypted connectivity between networks |
| Azure ExpressRoute | Provides private connectivity between on-premises infrastructure and Microsoft cloud services |
| Azure Arc | Extends Azure management and governance capabilities to hybrid and multicloud environments |

**Key Point:** Hybrid Cloud = Combination of public and private cloud environments.

---

## 5. Public vs. Private vs. Hybrid Cloud

| Feature | Public Cloud | Private Cloud | Hybrid Cloud |
|---|---|---|---|
| Infrastructure | Shared | Dedicated | Combination |
| Ownership | Cloud provider | Organization or hosting provider | Depends on environment |
| Management | Primarily cloud provider | Primarily organization or hosting provider | Shared across environments |
| Scalability | High | Depends on available infrastructure | Flexible |
| Upfront Cost | Generally low | Generally higher | Depends on architecture |
| Infrastructure Control | Less direct control | Greater control | Varies by environment |
| Best Suited For | Flexible, cost-effective cloud services | Strict control and compliance requirements | Combining private infrastructure with public cloud capabilities |

---

## 6. Important AZ-900 Exam Points

- **Public Cloud:** Infrastructure is owned and managed by a cloud provider and shared among customers.
- **Private Cloud:** Infrastructure is dedicated to one organization.
- **Hybrid Cloud:** Combines public and private cloud environments.
- Public cloud environments use logical isolation to separate customers.
- Private clouds can be hosted on-premises or by an external provider.
- Private clouds generally require more infrastructure management.
- Hybrid cloud allows organizations to choose where workloads and data reside.
- VPN Gateway, ExpressRoute, and Azure Arc support different aspects of hybrid cloud environments.

---

## 7. Quick Revision

| Question | Answer |
|---|---|
| What are the three cloud deployment models? | Public, Private, and Hybrid |
| Who owns public cloud infrastructure? | Cloud provider |
| Is public cloud infrastructure shared? | Yes, with logical isolation between customers |
| Which cloud model provides dedicated infrastructure? | Private Cloud |
| Can private cloud be hosted off-premises? | Yes |
| Which model combines public and private cloud? | Hybrid Cloud |
| Which model is commonly preferred for low upfront costs and rapid scalability? | Public Cloud |
| Which model offers greater direct infrastructure control? | Private Cloud |
| Which model allows sensitive workloads to remain private while using public cloud resources? | Hybrid Cloud |

---

## 8. Lecture Summary

Cloud deployment models describe how cloud infrastructure is hosted and managed.

- **Public Cloud:** Shared infrastructure owned and managed by a cloud provider.
- **Private Cloud:** Dedicated infrastructure used by a single organization.
- **Hybrid Cloud:** Combines public and private cloud environments for greater flexibility.

**Main Takeaway:** The appropriate cloud model depends on an organization's cost, control, security, compliance, and scalability requirements.