# Lab 01 — Troubleshooting

## Issue

While testing Azure RBAC, the lab user initially received an **Access Denied** message when attempting to access the Azure resource group.

## Investigation

The following areas were checked:

- Azure subscription access
- Resource group permissions
- Microsoft Entra ID groups
- Azure RBAC role assignments
- User authentication session

The RBAC configuration was designed using the principle of least privilege.

## Root Cause

The required Azure RBAC assignment was not correctly available to the user through the intended group membership.

The `Azure-Users` group was configured with the **Reader** role, while the `Azure-Admins` group was configured with the **Contributor** role at the appropriate scope.

## Resolution

The user's group membership and RBAC assignment were corrected.

After signing out and signing back in to refresh the authentication token, access was successfully restored.

## Lessons Learned

This lab demonstrated that Azure access depends on several layers:

1. Microsoft Entra ID identity
2. Group membership
3. Azure RBAC role
4. RBAC scope
5. Authentication/token refresh

It also demonstrated the importance of using groups rather than assigning permissions individually to users.

## Key AZ-104 Concepts

- Microsoft Entra ID
- Azure RBAC
- Role assignments
- Security groups
- Resource group scope
- Least privilege
- Access troubleshooting
- Authentication token refresh
