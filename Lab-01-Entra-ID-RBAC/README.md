# Lab 01 — Microsoft Entra ID & Azure RBAC

## Objective

Build and test a role-based access control environment using Microsoft Entra ID and Azure RBAC.

The objective was to understand how Azure users, groups, roles, and scopes work together to control access to Azure resources.

---

## Environment

- Microsoft Azure
- Microsoft Entra ID Free
- Azure Subscription
- Resource Group: `AZ104-Lab-RG`
- Region: South Africa North

---

## Architecture

```text
Azure Subscription
│
├── Azure-Users
│   └── AZ104 Lab User
│       └── Reader
│
└── AZ104-Lab-RG
    │
    ├── Azure-Admins
    │   └── AZ104 Lab Admin
    │       └── Contributor
    │
    └── Azure-Users
        └── Reader
---

## Evidence

Screenshots demonstrating the completed configuration:

1. [Entra ID Users](./evidence/01-entra-users.png)
2. [Entra ID Groups](./evidence/02-entra-groups.png)
3. [Azure Resource Group](./evidence/03-resource-group.png)
4. [Azure-Admins — Contributor Role](./evidence/04-admins-contributor.png)
5. [Azure-Users — Reader Role](./evidence/05-users-reader.png)

## Lab Status

✅ **Completed**

The lab demonstrates Microsoft Entra ID users and groups, Azure RBAC role assignments, resource-group scope, subscription inheritance, and basic RBAC troubleshooting.
