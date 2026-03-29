---
title: "Students and Bulk Import"
description: "How to search your student roster, review profiles, and perform bulk imports from Excel"
weight: 32
draft: false
---

The Students module is your CRM for managing the individuals you advise. You can view their progress individually, assign them to groups, or import hundreds of students at once.

---

## 1. Searching and Filtering Your Roster

When you open the **Students** module from the sidebar, you see your entire authorized roster.

1. **Search:** Use the search bar to find a student quickly by name or email.
2. **Filter:** Narrow down your list using the drop-down filters. You can filter by:
   - Assigned Groups
   - Chat status (e.g., awaiting reply)
   - Assessment signals (e.g., completed, missing)
   - Joined date or location
3. **Sort:** Click the column headers (Name, Email, Joined Date) to reorder the list.

### Viewing Student Details
Click on any student row or card to open their detailed profile. Here you get full context on their background, activities, and current plateau.

![Student roster list showing search bar, filter dropdowns, and student rows with name and email columns](/images/user-manual/advisor-panel/students-roster.png)

Image placeholder: Add screenshot of the students module showing the search bar, filter controls, and several student rows.

---

## 2. Managing Group Assignments

To help organize your communications, you can assign students to Groups right from the roster.

1. From the Students list, select the checkbox next to one or more students.
2. Click the **Assign to Group** action button.
3. Check the boxes for the target groups.
4. Click **Save**. The membership updates instantly.

*(Note: See the [Groups Management]({{< relref "/docs/advisor-panel/groups" >}}) guide for how to create groups in the first place).*

---

## 3. Bulk Importing Students (Excel)

If you have a large cohort starting simultaneously, do not add them one by one. Use the Bulk Import tool.

1. On the Students page, click **Bulk Actions > Import**.
2. Prepare your `.xlsx` or `.xls` file. Your spreadsheet **must** contain these three exact column headers in the first row:
   - `email`
   - `first_name`
   - `last_name`
3. Upload the file.
4. The system will parse the file and show a **Preview Table**.
5. Select the rows you wish to actually import, or select all.
6. Click **Confirm Import**.
7. Wait. The system will summarize successes and any skipped rows (failures).

### Important Import Rules
- **File Limits:** There is a maximum file size limit (usually a few megabytes).
- **Duplicates:** If an email already exists in the system, that row will be skipped/flagged.
- **Group Assignment:** Imported students are *not* automatically placed in a group upon import. You must assign them afterward.

![Bulk import dialog showing the file upload area, preview table with rows and checkboxes, and Confirm Import button](/images/user-manual/advisor-panel/students-bulk-import.png)

Image placeholder: Add screenshot of the bulk import flow — show the file upload step or the preview table with student rows ready to be confirmed.

---

## Common Questions

| Situation | What to do |
|---|---|
| I uploaded an Excel file but the preview is totally blank | Make sure your file is a valid `.xlsx` and exactly matches the required lowercase header names (`email`, `first_name`, `last_name`) |
| The filters say "0 students found" but I know they exist | You likely have conflicting filters applied. Clear all filters and reapply them one by one |
| I just imported students; how do I message them all? | Create a Group for the new cohort, assign them, and then use the [Notifications]({{< relref "/docs/advisor-panel/notifications" >}}) module to broadcast a message |
