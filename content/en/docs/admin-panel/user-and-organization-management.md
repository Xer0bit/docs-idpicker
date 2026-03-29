---
title: "User and Organization Management"
description: "How to provision new organizations, audit user accounts, and safely delete records"
weight: 52
draft: false
---

As a platform administrator, you control the foundational structure of IDPicker. This module allows you to manage the top-level Organizations (schools, agencies) and manually audit the individual users beneath them.

---

## 1. Organization Management

Organizations are the containers that hold Advisors, Students, and Parents. Before onboarding a new school, you must create their Organization record.

1. In the sidebar, click **Organization Management**.
2. Click **Create Organization**.
3. Fill in the organization's public profile details (Name, Location, Branding if applicable).
4. Assign the **Primary Admin** (the head advisor or IT contact for that school). 
5. Click **Save**. The organization is now active and its admin can begin inviting students.
6. *To edit or delete an organization, use the action menu next to its name in the list view.*

![Organization list showing school names, primary admin, location, and action menus, with Create Organization button](/images/user-manual/admin-panel/organization-list.png)

*Image placeholder: Add screenshot of the organization management list with several school rows and the Create Organization button.*

---

## 2. Auditing Student Accounts

While Advisors manage their own rosters, Super Admins have global visibility over every student in the system for support and auditing purposes.

1. Open **Student Management** from the sidebar.
2. Use the global search bar to locate any student by name or email across all organizations.
3. Expand a student's row to view their full diagnostic detail, including:
   - Email verification status
   - Premium subscription status
   - Total login/activity counters
4. **Global Deletion:** If requested for GDPR/CCPA compliance, you can hard-delete a student from this menu. *Use extreme caution and always confirm before executing.*

![Student management search showing name/email search results with expanded row displaying verification and activity details](/images/user-manual/admin-panel/student-management.png)

*Image placeholder: Add screenshot of the student management global search results with an expanded row showing account verification status and activity data.*

---

## 3. Managing Parent Accounts

Parents exist independently but are relationally linked to students. 

1. Open **Parent Management**.
2. Search and filter to locate a specific parent profile.
3. Expand their detail view to manually manage their relationships: you can forcefully **Link** them to a student by ID, or **Unlink** a relationship if a mistake was made.
4. You can also manually trigger a new invitation email from this panel if a parent claims they never received theirs.

---

## 4. Safety Checklist Before Deletion

When an organization ceases operation, or a user requests account deletion, follow these steps to prevent data corruption:

1. **Verify Dependencies:** Ensure there are no active financial subscriptions tied to the account.
2. **Export Data:** If required by your SLA or compliance policy, export their assessment records before deletion.
3. **Execute:** Delete the dependent users first (e.g., Students/Parents) before deleting the parent Organization container. 
4. **Confirm:** Rely on the system's confirmation dialogue, but always double-check the target ID.

---

## Common Questions

| Situation | What to do |
|---|---|
| I created an Organization but the head Advisor cannot log in | Reopen the organization record and double-check you spelled their Admin Email correctly. Check their verification status |
| I linked a parent manually but they cannot see the student | They may need to refresh their session. Also, verify that the student account is actively fully registered, not just a draft |
| I accidentally deleted a user | Hard deletions via the Admin panel are permanent and cascade through the database. You will need to restore from a database backup if recovery is critical |
