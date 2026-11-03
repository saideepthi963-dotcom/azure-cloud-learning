# Cloud Deployment Models — Use Cases

**Certification:** Microsoft Azure Fundamentals (AZ-900)  
**Topic:** Cloud Computing Concepts

---

## 1. Choosing the Right Cloud Deployment Model

Organizations choose between **Public, Private, and Hybrid Cloud** based on their requirements for:

- Security and data protection
- Regulatory compliance
- Infrastructure control
- Cost efficiency
- Scalability and flexibility
- Existing IT infrastructure

Each model is suitable for different business needs.

---

## 2. Public Cloud — When to Use It

Public Cloud is ideal when organizations prioritize **rapid deployment, scalability, cost efficiency, and minimal infrastructure management**.

### Common Use Cases

**1. Startups and Small Businesses**
- Deploy applications quickly.
- Avoid large upfront hardware investments.
- Pay based on resource consumption.

**2. Development and Testing**
- Create temporary environments.
- Easily increase or decrease resources.
- Pay for resources as needed.

**3. Websites and Customer-Facing Applications**
- Handle changing website traffic.
- Scale resources to support increasing demand.
- Support applications without maintaining physical infrastructure.

### Key Benefits
- Rapid deployment
- High scalability and elasticity
- Lower upfront costs
- Reduced infrastructure management

**Best Choice:** When speed, flexibility, and cost efficiency matter most.

---

## 3. Private Cloud — When to Use It

Private Cloud is ideal when organizations prioritize **infrastructure control, compliance, security, and data protection**.

### Common Use Cases

**1. Financial Institutions**
- Maintain greater control over infrastructure.
- Apply organization-specific encryption and data-handling requirements.

**2. Government Agencies**
- Operate highly restricted environments.
- Maintain strict infrastructure and security controls.

**3. Healthcare Organizations**
- Protect sensitive patient information.
- Support regulatory compliance requirements, such as HIPAA.

**4. Organizations with Existing Infrastructure**
- Continue using existing on-premises hardware.
- Introduce cloud capabilities such as automation and self-service.

### Key Benefits
- Dedicated infrastructure
- Greater infrastructure control
- Customizable security configurations
- Support for strict compliance requirements
- Ability to use existing hardware investments

**Best Choice:** When control and compliance requirements outweigh cost efficiency and broad scalability.

**Note:** Public cloud services can also support regulated workloads. Private cloud is a deployment choice, not an automatic compliance requirement.

---

## 4. Hybrid Cloud — When to Use It

Hybrid Cloud is ideal when organizations need to **combine their existing private infrastructure with public cloud services such as Microsoft Azure**.

### Common Use Cases

#### 1. Cloud Bursting

Cloud bursting occurs when an organization's on-premises infrastructure reaches capacity and additional workloads are transferred to public cloud resources.

This allows organizations to handle increased demand without permanently expanding their physical infrastructure.

#### 2. Disaster Recovery and Backup

Organizations can replicate workloads or back up data to Azure.

This provides recovery options without requiring an additional physical datacenter.

#### 3. Gradual Cloud Migration

Organizations can move applications and workloads to Azure gradually.

Some workloads remain on-premises while others move to the cloud.

#### 4. Regulatory and Sensitive Workloads

Organizations can:
- Keep sensitive data in private infrastructure.
- Run less-sensitive applications or operations in Azure.
- Maintain flexibility while addressing data control requirements.

### Key Benefits
- Flexibility in workload placement
- Additional cloud capacity when needed
- Disaster recovery capabilities
- Gradual cloud adoption
- Integration of on-premises infrastructure with Azure

**Best Choice:** When organizations need both private infrastructure control and public cloud flexibility.

---

## 5. Comparison of Cloud Deployment Model Use Cases

| Requirement | Recommended Cloud Model |
|---|---|
| Startup with limited upfront budget | Public Cloud |
| Development and testing environments | Public Cloud |
| Website with changing traffic | Public Cloud |
| Dedicated infrastructure and greater control | Private Cloud |
| Highly restricted infrastructure requirements | Private Cloud |
| Existing on-premises hardware with cloud automation | Private Cloud |
| Additional capacity during peak demand | Hybrid Cloud |
| Backup and disaster recovery using Azure | Hybrid Cloud |
| Gradual migration from on-premises to Azure | Hybrid Cloud |
| Sensitive workloads on-premises with other workloads in Azure | Hybrid Cloud |

---

## 6. Important AZ-900 Exam Points

- **Public Cloud:** Best suited for rapid deployment, elasticity, scalability, and cost efficiency.
- **Private Cloud:** Best suited for dedicated infrastructure and greater organizational control.
- **Hybrid Cloud:** Best suited for combining private infrastructure with public cloud capabilities.
- **Cloud Bursting:** Uses public cloud resources when private infrastructure reaches capacity.
- **Disaster Recovery:** Hybrid environments can use Azure to replicate workloads and support recovery.
- **Gradual Migration:** Hybrid cloud allows organizations to move workloads to Azure over time.
- **Regulatory Requirements:** Organizations may choose private or hybrid environments when workloads must remain on-premises.

---

## 7. Quick Revision

| Question | Answer |
|---|---|
| Which cloud model is suitable for startups? | Public Cloud |
| Which model is ideal for temporary development environments? | Public Cloud |
| Which model provides dedicated infrastructure? | Private Cloud |
| Which model offers greater direct infrastructure control? | Private Cloud |
| What is cloud bursting? | Using public cloud capacity when private infrastructure reaches its limits |
| Which model supports cloud bursting? | Hybrid Cloud |
| Which model supports gradual cloud migration? | Hybrid Cloud |
| Which model combines on-premises resources with Azure? | Hybrid Cloud |
| Which model can support Azure-based disaster recovery for on-premises workloads? | Hybrid Cloud |

---

## 8. Lecture Summary

Cloud deployment models are selected based on an organization's security, compliance, cost, control, and scalability requirements.

- **Public Cloud:** Ideal for rapid deployment, scalability, and cost efficiency.
- **Private Cloud:** Ideal for dedicated infrastructure and greater control.
- **Hybrid Cloud:** Ideal for combining existing infrastructure with public cloud capabilities.

**Main Takeaway:** Choose the cloud deployment model that best matches the organization's business and technical requirements.