
# Azure Governance Methodologies | AZ-900

Azure governance helps organizations **control access, enforce rules, protect resources, and maintain consistent cloud environments**.

## 1. Azure Policy

Azure Policy creates and enforces rules that Azure resources must follow to meet organizational standards and compliance requirements.

- Evaluates both existing and newly created resources.
- Identifies resources as **compliant** or **non-compliant**.
- Can deny non-compliant resource deployments.
- Can automatically remediate certain non-compliant configurations.
- Includes built-in policies for compute, storage, networking, security, and monitoring.
- Can integrate policy checks into Azure DevOps deployment pipelines.

**Example:** A policy can restrict which VM sizes are allowed or prevent VMs from being created with public IP addresses.

### Three Steps to Implement a Policy

1. **Policy Definition:** Specify what should be evaluated and what action to take.
2. **Policy Assignment:** Apply the definition to a scope, such as a management group, subscription, or resource group.
3. **Compliance Evaluation:** Review compliant and non-compliant resources and take corrective action.

Policy assignments are **inherited by child resources** within their scope.

## 2. Policy Initiatives

A policy initiative is a **collection of Azure Policy definitions** managed together to achieve a broader compliance goal.

- **Initiative Definition:** Groups several policy definitions.
- **Initiative Assignment:** Applies the group to a specific scope.
- Helps track overall compliance without managing every policy separately.
- Useful when compliance requirements grow over time.

**Remember:** A policy is one rule. An initiative groups rules together.

## 3. Azure Role-Based Access Control (RBAC)

Azure RBAC determines **who can access Azure resources and what actions they can perform**.

It follows the principle of **least privilege**: give users only the permissions necessary for their jobs.

Examples:
- A VM administrator can manage VMs without managing virtual networks.
- A database administrator can manage SQL databases without accessing unrelated resources.

### Important Concepts

- RBAC uses an **allow model**: assigned roles grant permissions such as read, write, or delete.
- Permissions can be assigned at management group, subscription, resource group, or resource scope.
- Role assignments can be inherited by child scopes.
- RBAC supports separation of duties between teams.
- Azure RBAC is available without an additional charge.

**Azure Portal:** Access Control (IAM) is used to view, grant, and remove role assignments.

**Exam Tip:** If the question asks who can access a resource or what they can do, think **Azure RBAC**.

## 4. Azure Resource Locks

Resource locks protect Azure resources from accidental modification or deletion.

| Lock Type | Read | Modify | Delete |
|---|---|---|---|
| CanNotDelete | Yes | Yes | No |
| ReadOnly | Yes | No | No |

- **CanNotDelete:** Prevents deletion but permits authorized modifications.
- **ReadOnly:** Prevents both modification and deletion.
- Locks can be applied to individual resources or resource groups.
- Locks can affect child resources through inheritance.
- Locks restrict management operations even when a user has RBAC permissions.

**Exam Tip:** If an administrator must edit a resource but must not delete it, choose **CanNotDelete**.

## 5. Azure Blueprints (Legacy Service)

Azure Blueprints was designed to create **repeatable, standardized Azure environments** that follow organizational requirements.

A blueprint could package:
- Azure Policy assignments
- RBAC role assignments
- Azure Resource Manager (ARM) templates
- Resource groups and other deployment artifacts

### Blueprint Workflow

1. Create a blueprint definition.
2. Assign the blueprint to a scope.
3. Track blueprint assignments and compliance.

### Azure Blueprints vs. ARM Templates

| Azure Blueprints | ARM Templates |
|---|---|
| Packages governance and deployment artifacts | Defines infrastructure resources |
| Maintains an association between a blueprint definition and its assignment | Does not maintain an equivalent ongoing blueprint-assignment relationship |
| Designed for repeatable governed environments | Designed for repeatable infrastructure deployment |

### Important 2026 Update

Azure Blueprints is being retired on **January 31, 2027**.

Microsoft recommends:
- **Azure Deployment Stacks** for resource lifecycle management and deployment protection.
- **Template Specs or Git** for storing and versioning templates.

Learn the historical Blueprint concept from the lecture, but remember the modern replacement.

## 6. Quick Comparison: All Governance Tools

| Service | Main Purpose |
|---|---|
| Azure Policy | Enforce resource compliance rules |
| Policy Initiative | Group multiple policies |
| Azure RBAC | Control user permissions |
| Resource Locks | Prevent accidental modification or deletion |
| Azure Blueprints (Legacy) | Standardize governed Azure deployments |
| Azure Deployment Stacks | Manage resource deployments and lifecycle |

## 7. AZ-900 Exam Quick Revision

| Question Keyword | Correct Concept |
|---|---|
| Enforce organizational standards | Azure Policy |
| Evaluate compliance | Azure Policy |
| Group multiple policies | Policy Initiative |
| Grant permissions to users | Azure RBAC |
| Least-privilege access | Azure RBAC |
| Prevent accidental deletion | CanNotDelete Lock |
| Prevent modification and deletion | ReadOnly Lock |
| Standardized environment deployment (legacy) | Azure Blueprints |
| Modern replacement for Blueprint deployment management | Azure Deployment Stacks |

### Final Memory Trick

**Policy = Rules**  
**Initiative = Group of Rules**  
**RBAC = Permissions**  
**Locks = Protection**  
**Blueprints = Standardized Deployment (Legacy)**
