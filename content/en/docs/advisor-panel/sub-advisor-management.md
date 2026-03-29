---
title: "Sub-Advisor Management"
description: "How to invite sub-advisors, delegate your workload, and restrict their permissions"
weight: 40
draft: false
---

If you are a primary Advisor managing a large organization, you can invite sub-advisors (like assistants or specialized tracking counselors) to help you. This guide explains how to invite them and safely restrict their access.

---

## 1. Creating a New Sub-Advisor

1. In the sidebar, click **Sub-Advisors**.
2. Click the **Create Sub-Advisor** button.
3. Fill in their identity details:
   - **Full Name**
   - **Email** (This will be their login)
4. Set their **Assigned Scope**:
   - If you want them to text *only* 12th graders, assign them explicitly to the "12th Graders" Group. They will not be able to see any students outside of that group.
5. Configure their **Permission Set**:
   - Decide exactly which modules they can see (e.g., enable *Students* and *Chat*, but disable *Forms* and *Settings*).
6. Click **Save / Create**.
7. The system will email them an invitation link to set up their password.

![Sub-advisor creation form showing name, email, scope selector, and permission checkboxes](/images/user-manual/advisor-panel/sub-advisor-create.png)

Image placeholder: Add screenshot of the sub-advisor creation form with name, email, and permission matrix visible.

---

## 2. Editing Sub-Advisor Permissions

If a sub-advisor's role changes, you can adjust their access on the fly.

1. Open the **Sub-Advisors** module.
2. Click on the target sub-advisor's name.
3. Scroll down to the Permission Matrix.
4. Toggle specific module access on or off as needed. You can also change which exact groups they govern here.
5. Click **Save**. The changes will apply the next time they log in or refresh their page.
![Permission matrix editor for a sub-advisor showing module toggles with some enabled and some disabled](/images/user-manual/advisor-panel/sub-advisor-permissions.png)

Image placeholder: Add screenshot of the sub-advisor permission matrix editor with some modules toggled on and others off.
### Validating Their Access
If you want to be completely sure you set the permissions correctly:
1. Ask the sub-advisor to log in while you watch, OR
2. Temporarily log in using a designated "test" sub-advisor account setup with the identical permission matrix.
3. Verify that restricted modules are completely hidden from the sidebar.

---

## 3. Revoking Access (Deactivation)

If a sub-advisor leaves your organization, you must revoke their access immediately to protect student privacy.

1. Open their sub-advisor record.
2. Change their status to **Inactive** (or click the **Revoke Access** button, depending on your UI version).
3. Click **Save**.
4. The sub-advisor is immediately logged out of all active sessions and cannot sign back in.

---

## Common Questions

| Situation | What to do |
|---|---|
| My sub-advisor cannot see any students | Check their Assigned Scope. If they are not assigned to any groups, and not given "All Students" access, their roster will be blank |
| A sub-advisor sees too many modules | You granted them too many checkboxes in the Permission Matrix. Uncheck the modules you want hidden and Save |
| I deactivated an account but they are still logged in | While the system attempts to kill active sessions immediately, a hard refresh on the sub-advisor's browser will forcefully enforce the new locked state |
