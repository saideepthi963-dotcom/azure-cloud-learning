# Azure Subscriptions and Management Groups

## 1. Azure Subscriptions

An **Azure Subscription** is a way to organize Azure resources, manage costs, and control access.

Imagine a company has two departments: **HR and Finance**.

The company can create separate Azure subscriptions for each department.

This allows it to:
- Track how much each department spends.
- Control who can access each department's resources.

These are called the two main subscription boundaries:

**Billing Boundary →** Tracks and organizes Azure costs.

**Access Control Boundary →** Controls who can access and manage resources.

An organization can have multiple subscriptions, and Azure subscriptions are associated with a Microsoft Entra ID tenant.

### Why Use Multiple Subscriptions?

Companies commonly separate subscriptions by department, project, or environment (Development/Production). Separate subscriptions can also help manage Azure resource limits.

---

## 2. Azure Management Groups

**Management Groups are containers used to organize and manage multiple Azure subscriptions together.**

Imagine a company has 10 Azure subscriptions.

The company wants to prevent employees from creating resources outside approved Azure regions.

Instead of applying the same rule separately to all 10 subscriptions, it can place them under one management group and apply the rule once.

All subscriptions under that management group **inherit the rule automatically**.

This is called **Policy Inheritance**.

Management groups can also be used to assign Azure RBAC permissions across multiple subscriptions.

### Azure Management Hierarchy

```text
Management Group
       │
       ├── Subscription 1
       │       └── Resource Group
       │              └── Resources
       │
       └── Subscription 2
               └── Resource Group
                      └── Resources
```

### Important Rules

- Management groups exist above subscriptions.
- Policies and RBAC permissions can be inherited by subscriptions below them.
- All subscriptions in a management group hierarchy belong to the same Microsoft Entra ID tenant.
- A management group can contain other management groups.
- Each subscription or management group has only one parent.

---

## ⭐ Important AZ-900 Exam Points

| Concept | Remember |
|---|---|
| **Resource** | Individual Azure item |
| **Resource Group** | Organizes related resources |
| **Subscription** | Billing and access control boundaries |
| **Management Group** | Manages multiple subscriptions together |
| **Policy Inheritance** | Rules applied at a higher level affect resources below |
| **Azure RBAC** | Controls who can perform actions |

### Easy Way to Remember

**Resource Group → Organizes resources.**

**Subscription → Manages billing and access.**

**Management Group → Manages multiple subscriptions.**

**Main Takeaway:** Azure uses a hierarchy to organize resources and apply management rules efficiently.