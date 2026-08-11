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
