---
title: "Profile, Prompts, and Interests"
description: "How to update your advisor profile, fine-tune AI prompts for your students, and manage interest data"
weight: 38
draft: false
---

This guide covers three configuration areas that affect both your own advisor identity and how IDPicker's AI behaves for your specific student cohort: your profile, the AI prompt templates, and the student interest records.

---

## 1. Updating Your Advisor Profile

Your profile information appears inside student and parent-facing chat windows when they interact with you. Keeping it accurate builds trust.

1. In the sidebar, click your **Avatar** or **Profile** link.
2. Click **Edit Profile**.
3. Update any of the following:
   - **Display Name** and **Title** (e.g., *Senior Career Counselor*)
   - **Bio** — A short paragraph about your background and specialties
   - **Avatar** — Upload a clear headshot (recommended: square, at least 400×400 px)
   - **Contact Details** — Office hours, phone extension, or secondary email if relevant
   - **Organization Data** — Department, branch, or campus information if your platform supports it
4. Click **Save Profile**.
5. Verify the preview panel on the right shows the updated name and avatar correctly.

![Advisor profile editor showing name, title, bio, and avatar upload fields](/docs-idpicker/images/user-manual/advisor-panel/profile-editor.png)

---

## 2. Editing AI Prompt Templates

If your organisation has been granted permission to configure regional AI prompts, you can adjust how the AI Mentor communicates with *your specific students* — independent of the global settings the Admin controls.

1. In the sidebar, click **Prompts**.
2. The prompt list is organized by **Category** (e.g., *Mentor Persona*, *Career Guidance*, *University Selection*) and **Subcategory**.
3. Use the filter bar to navigate to the specific prompt you want to adjust.
4. Click the prompt name to open the editor.
5. Read the existing instruction text carefully before editing.
6. Make your changes — keep them concise and imperative (e.g., *"Always recommend at least two Turkish universities when a student specifies Turkey as their preferred country"*).

> **Warning:** Never delete or rename the dynamic variables inside double curly braces, such as `{{student_name}}` or `{{trait_score}}`. These inject real student data into the AI's context. Removing them will break personalisation.

7. Click **Save**. The updated prompt is live immediately for your students.
8. Re-open the prompt to confirm the saved version reflects your edit.

![Prompt editor showing category filter, prompt text area, and dynamic variable placeholders highlighted](/docs-idpicker/images/user-manual/advisor-panel/prompts-editor.png)

---

## 3. Managing Student Interest Records

The Interests module shows the career domains and fields of study each student has expressed interest in. These interests feed directly into the AI's recommendation logic.

1. In the sidebar, click **Interests**.
2. The table shows a list of student-interest pairs: which student expressed interest in what domain, and when.
3. Filter by **Student** or **Interest Domain** to find a specific entry.
4. Click a row to open the interest detail.
5. If a student has been mis-tagged (for example they changed their mind), you can update the status or remove the interest from their profile.
6. Click **Save** and verify the list refreshes.

> **Note:** Interests set directly by students on their own profiles take priority in the recommendation engine. Changes you make here may be overridden if the student re-sets their preferences from their own account.

![Interests table showing student names, interest domain labels, and status badges](/docs-idpicker/images/user-manual/advisor-panel/interests-table.png)

---

## Common Questions

| Situation | What to do |
|---|---|
| My profile avatar is not updating | Check that the file is a JPG or PNG and under the maximum allowed size (typically 2–5 MB). Try a different browser if it still fails |
| I saved a prompt but an error says "Invalid Template Syntax" | Look for broken `{{` brackets. Every opening `{{` must have a matching `}}`. Fix the broken variable and retry |
| A student's interests look wrong or outdated | Open their interest detail, update the status to reflect their current goals, and save — then ask the student to confirm their interests from their own profile settings |
