---
title: "Forms and Responses"
description: "How to create custom forms, collect data, and review student responses"
weight: 35
draft: false
---

The Forms module allows advisors to create custom questionnaires, surveys, or data-collection sheets, distribute them to specific students, and track the responses in one place.

---

## 1. Understanding the Forms Lifecycle

Every form moves through a specific lifecycle:
1. **Draft:** The form is being built and is invisible to students.
2. **Published:** The form is actively collecting data and is visible to assigned students on their dashboard.
3. **Archived:** (If applicable) The form is no longer accepting new responses, but old data is preserved.

---

## 2. Creating and Publishing a Form

1. In the sidebar, click **Forms**.
2. Click **Create New Form**.
3. Enter a **Title** and a helpful **Description**.
4. Use the form builder interface to add your specific fields (e.g., text inputs, dropdowns, checkboxes).
5. Click **Save as Draft** while you are still working on it.
6. When you are completely finished, select your target audience (groups or specific students) and change the status to **Publish**.

### Preview Before Publishing
Always click the **Preview** action before publishing! This lets you see the form exactly as a student will see it, ensuring that your required fields and visual layout behave as expected.

![Form builder interface showing the title field, question editor panel, and a preview of the first question](/images/user-manual/advisor-panel/forms-builder.png)

Image placeholder: Add screenshot of the form builder with the title, a couple of question fields, and the Publish button visible.

---

## 3. Managing Existing Forms

You can manage your forms from the main Forms list view:

- **Search & Filter:** Use the search bar to find a specific form by title, or filter to see only *Drafts* or *Published* forms.
- **Edit:** If a form is still a draft, you can freely edit its structure. Once an active form begins receiving responses, structural edits may be heavily restricted to prevent data corruption.
- **Delete:** Select the delete action to permanently remove the form. *Note: Doing this may also delete associated response records.*

---

## 4. Reviewing Student Responses

Once your form is published and students begin filling it out, you need to review their answers.

1. Locate the active form in your Forms list.
2. You will see a counter indicating the number of Total Responses. Click the **Responses** button.
3. A table will load showing a list of every student who submitted the form and the timestamp.
4. Click on an individual response row to drill down and read the specific answers provided by that student.

![Form responses table listing student names, submission timestamps, and a row-click drill-down panel](/images/user-manual/advisor-panel/forms-responses.png)

Image placeholder: Add screenshot of the form responses table showing student names, timestamps, and the drill-down view of one student's answers.

---

## Common Questions

| Situation | What to do |
|---|---|
| A student says they submitted, but my response count is not updating | The interface does not automatically live-refresh. Manually refresh the page to load the latest data from the server |
| The system prevents me from editing a form | The form is either locked due to your permission policy, or it is locked because it is Published and actively receiving responses |
| I accidentally deleted a form | Form deletion is permanent. Always export response data before taking destructive actions |
