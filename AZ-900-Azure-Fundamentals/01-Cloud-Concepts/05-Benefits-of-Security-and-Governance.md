# Benefits of Security and Governance in Azure

**Certification:** Microsoft Azure Fundamentals (AZ-900)  
**Topic:** Cloud Computing Concepts

---

## 1. What Are Security and Governance in Azure?

**Security** protects cloud resources, applications, and data from unauthorized access and cyber threats.

**Governance** defines and enforces rules for how cloud resources should be created, accessed, and managed.

Together, they help organizations:
- Protect resources and sensitive data.
- Control how Azure resources are used.
- Follow organizational policies and legal requirements.
- Reduce security risks.
- Maintain consistent cloud environments.

**Key Difference:**
- **Security = Protection**
- **Governance = Rules and Control**

---

## 2. Benefits of Security in Azure

In traditional on-premises environments, organizations are responsible for managing much of their security infrastructure.

This includes:
- Purchasing security hardware.
- Configuring firewalls.
- Updating and patching servers.
- Monitoring systems for threats.
- Maintaining physical infrastructure security.

Microsoft Azure reduces some of these responsibilities by providing built-in security capabilities.

Microsoft protects the underlying cloud infrastructure, including:
- Physical datacenters
- Global networking infrastructure
- Hypervisors (software that runs and manages virtual machines)
- Azure platform infrastructure

**Key Point:** Azure provides enterprise-level security capabilities without requiring organizations to build all the underlying infrastructure themselves.

However, customers must still secure their own data, identities, applications, and configurations according to the Shared Responsibility Model.

---

## 3. Important Azure Security Services

### Microsoft Entra ID

Microsoft Entra ID is a cloud-based identity and access management service.

It helps organizations:
- Manage user identities.
- Control access to applications and resources.
- Protect user accounts.
- Detect suspicious sign-in activity through identity protection capabilities.

**Remember:** Microsoft Entra ID helps manage identities and access.

### Microsoft Defender for Cloud

Microsoft Defender for Cloud is a cloud security management service.

It helps organizations:
- Monitor the security of Azure resources.
- Identify potential security risks.
- Detect threats through supported protection capabilities.
- Receive recommendations to improve security.

**Remember:** Defender for Cloud helps organizations identify security risks and improve cloud protection.

### Data Encryption

Encryption converts readable data into a protected form that requires the appropriate key to read.

Azure supports encryption in two important situations:

| Encryption Type | Meaning |
|---|---|
| Encryption at Rest | Protects data while it is stored. |
| Encryption in Transit | Protects data while it moves between systems. |

**Remember:** Encryption protects sensitive information when stored or transferred.

### Azure Key Vault

Azure Key Vault securely stores and manages sensitive information.

Examples include:
- Encryption keys
- Passwords
- Application secrets
- Certificates

**Remember:** Azure Key Vault helps protect and manage secrets, keys, and certificates.

---

## 4. What Is Governance in Azure?

**Governance means establishing rules and controls to ensure Azure resources are managed according to an organization's requirements.**

It helps organizations:
- Maintain consistent configurations.
- Control resource deployment.
- Restrict unauthorized actions.
- Enforce organizational standards.
- Support compliance requirements.
- Reduce configuration mistakes.

Azure provides tools that help organizations automatically enforce these rules.

---

## 5. Important Azure Governance Tools

### Azure Policy

Azure Policy helps organizations enforce rules across Azure resources.

For example, an organization can create policies to:
- Allow only approved Azure regions.
- Restrict certain virtual machine sizes.
- Require resources to have specific tags.

**What are tags?**

Tags are labels added to Azure resources to help organize and identify them.

For example, a resource might have a tag indicating which department owns it.

**Remember:** Azure Policy helps enforce organizational rules and standards.

### Azure Role-Based Access Control (Azure RBAC)

Azure RBAC controls who can perform specific actions on Azure resources.

It helps organizations:
- Assign permissions to users.
- Restrict access to sensitive resources.
- Allow users to perform only authorized actions.

**Remember:** Azure RBAC determines who can access Azure resources and what actions they can perform.

### Azure Management Groups

Management groups organize multiple Azure subscriptions into a hierarchy.

They allow organizations to apply governance rules across multiple subscriptions.

**Remember:** Management groups help manage governance at a large scale.

### Azure Subscriptions

Azure subscriptions organize resources and provide boundaries for billing and access management.

They can also help organizations apply governance controls to groups of resources.

**Remember:** Subscriptions help organize Azure resource usage, billing, and access.

---

## 6. Security vs. Governance

| Security | Governance |
|---|---|
| Focuses on protecting resources and data. | Focuses on establishing and enforcing rules. |
| Helps detect and prevent security threats. | Helps maintain organizational standards. |
| Uses tools such as Microsoft Defender for Cloud and Azure Key Vault. | Uses tools such as Azure Policy and management groups. |
| Reduces security risks. | Reduces configuration mistakes and unauthorized resource usage. |

**Important:** Security and governance work together to create protected and well-managed cloud environments.

---

## 7. Benefits of Combining Security and Governance

Combining Azure security and governance provides several advantages:

1. **Reduced Risk:** Security controls protect resources from threats.
2. **Improved Compliance:** Governance helps organizations follow required standards and regulations.
3. **Automated Enforcement:** Policies can automatically check or restrict resource configurations.
4. **Consistent Management:** Organizations can apply common rules across different teams and subscriptions.
5. **Reduced Manual Work:** Built-in tools reduce the need to manually review every resource.
6. **Greater Control:** Organizations can deploy cloud resources quickly while maintaining security and governance requirements.

---

## 8. Important AZ-900 Exam Points

- **Security** focuses on protecting cloud resources, identities, applications, and data.
- **Governance** focuses on controlling and standardizing Azure resource management.
- **Microsoft Entra ID:** Identity and access management.
- **Microsoft Defender for Cloud:** Cloud security recommendations and threat protection capabilities.
- **Azure Key Vault:** Secure management of secrets, encryption keys, and certificates.
- **Azure Policy:** Enforces organizational standards and evaluates resource compliance.
- **Azure RBAC:** Controls who can perform actions on Azure resources.
- **Management Groups:** Organize subscriptions and apply governance at scale.
- **Subscriptions:** Provide boundaries for billing and access management.
- **Encryption at Rest:** Protects stored data.
- **Encryption in Transit:** Protects data during transmission.
- The Shared Responsibility Model still applies when using Azure security services.

---

## 9. Quick Revision

| Question | Answer |
|---|---|
| What is Azure security? | Protecting resources, applications, identities, and data. |
| What is Azure governance? | Establishing and enforcing rules for managing cloud resources. |
| Which service manages user identities? | Microsoft Entra ID |
| Which service provides cloud security recommendations? | Microsoft Defender for Cloud |
| Which service stores secrets and encryption keys? | Azure Key Vault |
| Which service enforces organizational standards? | Azure Policy |
| Which service controls user permissions on Azure resources? | Azure RBAC |
| What organizes multiple subscriptions? | Management Groups |
| What protects stored data? | Encryption at Rest |
| What protects data during transmission? | Encryption in Transit |

---

## 10. Lecture Summary

Microsoft Azure provides built-in tools for protecting cloud environments and controlling how resources are managed.

**Security** protects applications, identities, resources, and data through services such as Microsoft Entra ID, Defender for Cloud, and Azure Key Vault.

**Governance** establishes and enforces organizational rules through tools such as Azure Policy, Azure RBAC, management groups, and subscriptions.

**Main Takeaway:** Security protects Azure resources, while governance ensures those resources are managed according to organizational rules.