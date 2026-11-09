# Understanding Azure Subscriptions

## 1. What Is an Azure Subscription?

An **Azure Subscription** is a logical unit that allows users to create, access, and manage Azure resources.

- Required for deploying most Azure resources.
- Associated with a Microsoft Entra ID tenant (formerly Azure Active Directory).
- An organization can have multiple subscriptions.
- Each subscription can have its own access controls and billing arrangements.

**Remember:** Azure Subscription = Organizes resources, access, and billing.

## 2. Two Main Purposes of Azure Subscriptions

### A. Billing Boundary

A subscription helps organizations track and manage Azure costs.

- Tracks costs associated with resources in the subscription.
- Allows costs to be separated by department, project, or environment.
- Supports different billing arrangements.

**Example:** A company creates separate subscriptions for its HR and IT departments to track their Azure spending independently.

### B. Access Control Boundary

A subscription provides a boundary for managing access to Azure resources.

- Permissions can be assigned at the subscription level.
- Different subscriptions can have different access rules.
- Helps organizations restrict resource access to authorized users.

**Example:** HR employees receive access to the HR subscription, while IT employees receive access to the IT subscription.

## 3. Why Create Multiple Subscriptions?

Organizations may use multiple subscriptions to:

- **Separate environments:** Development, testing, and production.
- **Organize departments:** HR, Finance, and IT.
- **Manage costs:** Track spending for different projects.
- **Control access:** Assign different permissions.
- **Manage service limits:** Some Azure resources have limits per subscription.

**Service Limits:** Restrictions on how many resources of a particular type can be created within a subscription or region.

## 4. Azure Billing Structure

For eligible Microsoft Customer Agreement billing accounts, Azure provides billing profiles and invoice sections to organize charges.

| Component | Purpose |
|---|---|
| **Billing Account** | Represents the organization's billing relationship with Microsoft. |
| **Billing Profile** | Manages invoices and payment information. |
| **Invoice Section** | Groups subscription charges by department, team, or project. |
| **Subscription** | Contains Azure resources whose usage generates charges. |

### How They Are Organized

Billing Account  
↓  
Billing Profile  
↓  
Invoice Section  
↓  
Azure Subscription

- A billing account can contain multiple billing profiles.
- Each billing profile generates its own invoice.
- Invoice sections help divide charges within that invoice.
- Subscriptions can be assigned to invoice sections.

**Note:** The available billing structure depends on the organization's Microsoft billing agreement.

## 5. Azure Resource Group vs. Subscription

| Resource Group | Subscription |
|---|---|
| Organizes related Azure resources | Organizes resources and resource groups |
| Helps manage resource lifecycles | Provides billing and access boundaries |
| Can contain multiple resources | Can contain multiple resource groups |
| Example: Web-App-RG | Example: Development-Subscription |

## ⭐ Important AZ-900 Exam Points

- **Azure Subscription:** Logical unit used to organize Azure resources.
- **Billing Boundary:** Helps track and manage Azure spending.
- **Access Control Boundary:** Helps control who can manage resources.
- **Microsoft Entra ID:** Provides the identity directory associated with Azure subscriptions.
- **Multiple Subscriptions:** Used for billing, access control, organizational separation, and resource limits.
- **Billing Profile:** Defines an invoice and associated billing information.
- **Invoice Section:** Groups charges within a billing profile's invoice.

### Easy Way to Remember

**Resource → An individual Azure item.**

**Resource Group → Organizes related resources.**

**Subscription → Controls billing and access for Azure resources.**

**Billing Profile → Organizes invoices.**