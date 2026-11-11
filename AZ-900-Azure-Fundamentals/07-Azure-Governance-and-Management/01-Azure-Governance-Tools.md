# Azure Governance Tools

**Azure Governance** helps organizations control how Azure resources are created, managed, and secured.

## 1. Azure Policy

**Azure Policy** creates and enforces rules for Azure resources to ensure they follow company standards.

**Example:** A company allows virtual machines only in the East US region. Azure Policy can prevent deployments in other regions.

- **Policy Definition:** Defines the rule.
- **Policy Assignment:** Applies the rule to a specific scope, such as a subscription or resource group.
- **Compliance Evaluation:** Checks whether resources follow the rule.

Azure Policy can identify non-compliant resources, block certain deployments, and support automatic remediation.

## 2. Policy Initiatives

A **Policy Initiative** groups multiple Azure Policies together to achieve a larger compliance goal.

**Example:** A company wants to enforce encryption, restrict VM sizes, and allow only approved Azure regions.

Instead of managing each policy separately, it groups them into one initiative.

**Remember: Policy = One rule | Initiative = Collection of rules.**

## 3. Azure Role-Based Access Control (RBAC)

**Azure RBAC** controls **who can perform which actions** on Azure resources.

**Example:** A VM administrator can manage virtual machines but cannot manage company databases unless granted permission.

RBAC follows the **principle of least privilege** — give users only the permissions needed for their jobs.

**Azure Policy vs. Azure RBAC:**

- **Azure Policy:** What configurations are allowed?
- **Azure RBAC:** Who is allowed to perform actions?

## 4. Azure Resource Locks

**Resource Locks** protect Azure resources from accidental deletion or modification.

| Lock Type | What It Allows |
|---|---|
| **CanNotDelete** | Read and modify, but cannot delete |
| **ReadOnly** | Read only; cannot modify or delete |

**Example:** A company applies a CanNotDelete lock to a production database to prevent accidental deletion.

## 5. Azure Blueprints

**Azure Blueprints** was designed to create repeatable Azure environments using resources, policy assignments, role assignments, and ARM templates.

Unlike ordinary ARM template deployments, Blueprints maintained a relationship between the blueprint assignment and deployed resources.

**Important update:** Azure Blueprints is being retired on **January 31, 2027**. Microsoft recommends **Azure Deployment Stacks** and **Template Specs** as replacements.

## Key Takeaway

| Service | Remember |
|---|---|
| **Azure Policy** | Enforce rules |
| **Policy Initiative** | Group multiple policies |
| **Azure RBAC** | Control user permissions |
| **Resource Locks** | Prevent deletion or modification |
| **Azure Blueprints** | Repeatable governed environments (retiring) |