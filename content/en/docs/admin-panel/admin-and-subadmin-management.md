---
title: "Admin and Subadmin Management"
description: "Detailed click-by-click admin access governance"
weight: 153
draft: false
---

## Create Admin User

1. Open Admin Management.
2. Click Add Admin.
3. Fill identity fields (email, username, first/last name).
4. Set temporary password.
5. Choose role.
6. Save and confirm creation.

## Edit Admin Profile

1. Open admin row detail.
2. Update identity fields.
3. Save updates.
4. Confirm list refresh reflects changes.

## Permission Assignment

1. Open permission panel for target admin.
2. Set feature scopes per module:
   - write
   - read
   - none
3. Set organization-level scope where applicable.
4. Save permissions.
5. Ask user to relogin if permissions do not refresh immediately.

## Subadmin Self View

1. Open Subadmin page.
2. Review effective permission summary.
3. Use refresh permissions action to sync latest grants.

## Common Questions

Q: Admin can see module but cannot perform action.
A: Verify action-level permission is write, not read.

Q: Updated permissions not applied.
A: Refresh permissions and reauthenticate.

![Admin Permissions Placeholder](/images/user-manual/admin-panel/admin-permissions.png)

Image placeholder: Permission matrix with feature and organization scopes.
