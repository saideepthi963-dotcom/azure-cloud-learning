# Azure Resources and Resource Groups

## 1. What Is an Azure Resource?

An **Azure Resource** is an item that you create and manage in Microsoft Azure.

**Examples:**
- Virtual Machines (VMs)
- Storage Accounts
- Web Apps
- Databases
- Virtual Networks
- SQL Servers

**Remember:** Resource = An individual item managed in Azure.

## 2. What Is a Resource Group?

A **Resource Group** is a logical container used to organize and manage related Azure resources.

For example, a resource group for a web application might contain:
- Virtual Machine
- Virtual Network
- Storage Account
- Database

### Important Rules

- Every Azure resource belongs to **one resource group**.
- A resource cannot belong to multiple resource groups simultaneously.
- Many resources can be moved between resource groups, although some have restrictions.
- Resource groups **cannot be nested** (one resource group cannot exist inside another).
- You can organize resources based on your organization's needs.

## 3. Why Use Resource Groups?

### A. Organize Resources

Group resources based on:
- **Function:** VMs, databases, or networking resources.
- **Lifecycle:** Resources created, managed, and deleted together.
- **Purpose:** Development, testing, or production environments.

### B. Manage Resource Lifecycle

Resources with a similar lifecycle are often placed in the same resource group.

**Example:**

A development resource group contains:
- 1 VM
- 1 Virtual Network
- 1 Storage Account

When the project is finished, deleting the resource group also deletes the resources inside it.

**Important:** Deleting a resource group deletes its contained resources. Resource locks can prevent deletion until the locks are removed.

### C. Control Access Using Azure RBAC

**Azure Role-Based Access Control (RBAC)** controls who can access Azure resources and what actions they can perform.

Permissions can be assigned at the resource group level.

**Example:**
- SQL administrators → Access to the SQL resource group.
- VM administrators → Access to the VM resource group.

This makes access management easier.

## 4. Resource vs. Resource Group

| Azure Resource | Resource Group |
|---|---|
| Individual Azure service or item | Container for Azure resources |
| Example: Virtual Machine | Example: Development Resource Group |
| Used to perform specific tasks | Used to organize and manage resources |
| Belongs to one resource group | Can contain multiple resources |

## ⭐ Important AZ-900 Exam Points

- **Resource:** A manageable item in Azure.
- **Resource Group:** A logical container for Azure resources.
- Each resource belongs to only one resource group at a time.
- Resource groups cannot contain other resource groups.
- Many resources can be moved between resource groups, subject to restrictions.
- Deleting a resource group deletes its contained resources.
- Resources with similar lifecycles should generally be grouped together.
- Azure RBAC permissions can be assigned at the resource group level.

### Easy Way to Remember

**Resource → An individual Azure item.**

**Resource Group → A folder-like container that organizes Azure resources.**

**RBAC → Controls who can manage those resources.**