# AZ-104 Azure Administration Labs

Hands-on Azure Administration labs created as part of my preparation for the **Microsoft Azure Administrator (AZ-104)** certification.

The labs focus on practical administration, troubleshooting, security, governance, networking, compute, storage, and monitoring.

---

## 🧪 Lab Progress

| Lab | Topic | Status |
|---|---|---|
| 01 | Microsoft Entra ID & Azure RBAC | ✅ Completed |
| 02 | Azure Governance & Policy | ⏳ Planned |
| 03 | Azure Storage | ⏳ Planned |
| 04 | Azure Virtual Machines | ⏳ Planned |
| 05 | Azure Virtual Networking | ⏳ Planned |
| 06 | App Services & Containers | ⏳ Planned |
| 07 | Azure Load Balancing | ⏳ Planned |
| 08 | Monitoring & Backup | ⏳ Planned |
| 09 | Azure CLI & PowerShell | ⏳ Planned |
| 10 | End-to-End Azure Environment | ⏳ Planned |

---

# Lab 01 — Microsoft Entra ID & Azure RBAC

## Objective

Build and test a role-based access control environment using Microsoft Entra ID and Azure RBAC.

The objective was to understand how Azure users, groups, roles, and scopes work together to control access to Azure resources.

---

## Environment

- Microsoft Azure
- Microsoft Entra ID
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
│     └── AZ104 Lab User
│           │
│           └── Reader
│
└── AZ104-Lab-RG
      │
      ├── Azure-Admins
      │     └── AZ104 Lab Admin
      │           │
      │           └── Contributor
      │
      └── Azure-Users
            │
            └── Reader
