# Microsoft Entra ID Roles and RBAC

## What Is Role-Based Access Control (RBAC)?

**RBAC (Role-Based Access Control)** determines what actions a user is allowed to perform based on their assigned role.

Imagine a company where different employees have different responsibilities:

- An IT administrator manages employee accounts.
- A billing administrator manages billing.
- A global administrator manages the entire identity system.

Instead of giving everyone full administrative access, Microsoft Entra ID assigns roles with specific permissions.

## Built-in Roles

Microsoft Entra ID provides predefined roles for common administrative tasks.

| Role | Permissions |
|---|---|
| **Global Administrator** | Manages all administrative features in Microsoft Entra ID |
| **User Administrator** | Manages users and groups |
| **Billing Administrator** | Manages billing-related tasks and purchases |

**Built-in roles** come with predefined permissions.

## Custom Roles

If built-in roles don't meet an organization's requirements, administrators can create **custom roles** with selected permissions.

Creating and assigning a custom role involves two steps:

1. **Role Definition:** Specifies which actions the role is allowed to perform.
2. **Role Assignment:** Gives that role to a user at a particular scope.

A **scope** determines where the permissions apply.

For example, an administrator can assign a role across the organization or limit it to a specific application.

Custom roles require Microsoft Entra ID Premium P1 or P2 licensing.

## Active vs. Eligible Role Assignments

When Microsoft Entra Privileged Identity Management (PIM) is enabled, privileged roles can be assigned in two ways.

| Assignment | Meaning |
|---|---|
| **Active** | User can use the assigned permissions immediately |
| **Eligible** | User must activate the role before using its permissions |

For example, an eligible administrator might need to complete MFA or provide a business justification before activating a privileged role.

## Microsoft Entra Roles vs. Azure RBAC

These are related but manage different things.

**Microsoft Entra Roles:** Control who can manage identities, users, groups, and other Entra ID settings.

**Azure RBAC:** Controls who can manage Azure resources such as virtual machines, storage accounts, and networks.

For example:

- Creating employee accounts → **Microsoft Entra User Administrator**
- Managing an Azure virtual machine → **Azure RBAC**

## Key Takeaway

**RBAC = Give users only the permissions they need for their responsibilities.**

- **Built-in role:** Predefined permissions.
- **Custom role:** Selected permissions for specific needs.
- **Role assignment:** Grants permissions at a specified scope.
- **Eligible assignment:** Requires activation before use.
- **Active assignment:** Permissions are available immediately.