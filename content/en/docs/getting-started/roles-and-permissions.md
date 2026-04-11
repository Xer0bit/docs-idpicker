---
title: "Roles and Permissions"
description: "A side-by-side comparison of what each user role can access and do on the IDPicker platform"
weight: 13
draft: false
---

IDPicker has five distinct user roles, each with a specific set of capabilities. Understanding what each role can and cannot do helps you set up accounts correctly and avoid confusion about access rights.

---

## 1. The Five Roles at a Glance

| Role | Who holds it | Primary purpose |
|---|---|---|
| **Super Admin** | Platform owner / IT operations staff | Full control of technical settings, all organisations, global content, and billing |
| **Advisor** | Head counselor or primary school contact | Manages their student roster, runs forms, distributes resources, chats with families |
| **Sub-Advisor** | Assistant counselor or specialist staff | Operates within a restricted subset of the Advisor's permissions and student scope |
| **Student** | The young person using the platform | Completes assessments, explores recommendations, chats with their advisor and AI mentor |
| **Parent / Guardian** | Parent or legal guardian of a student | Monitors a linked child's progress and communicates with the advisor |

---

## 2. Permission Comparison Table

### Students and Core Assessment

| Action | Super Admin | Advisor | Sub-Advisor | Student | Parent |
|---|---|---|---|---|---|
| Take self-assessments | — | — | — | ✅ | — |
| View own assessment results | — | — | — | ✅ | Read-only view |
| View any student's results | ✅ | ✅ | Scoped only | — | Own child only |
| Edit another user's answers | ✅ | — | — | — | — |

### Forms and Documents

| Action | Super Admin | Advisor | Sub-Advisor | Student | Parent |
|---|---|---|---|---|---|
| Create global forms | ✅ | — | — | — | — |
| Create organisation forms | — | ✅ | If permitted | — | — |
| Submit a form response | — | — | — | ✅ | ✅ |
| View form responses | ✅ | ✅ | If permitted | Own only | — |
| Upload application documents | — | — | — | ✅ | — |
| Review / verify documents | ✅ | ✅ | If permitted | — | — |

### Communication

| Action | Super Admin | Advisor | Sub-Advisor | Student | Parent |
|---|---|---|---|---|---|
| Send notifications to all students | ✅ | — | — | — | — |
| Send notifications to own cohort | — | ✅ | If permitted | — | — |
| Chat with their advisor | — | — | — | ✅ | ✅ |
| Chat with a student's parent | — | ✅ | ✅ | — | — |
| Join a family group chat | — | ✅ | ✅ | ✅ | ✅ |

### User and Organisation Management

| Action | Super Admin | Advisor | Sub-Advisor | Student | Parent |
|---|---|---|---|---|---|
| Create organisations | ✅ | — | — | — | — |
| Invite advisors | ✅ | — | — | — | — |
| Invite sub-advisors | — | ✅ | — | — | — |
| Import students in bulk | — | ✅ | If permitted | — | — |
| Link a parent to a student | ✅ | — | — | — | Request only |
| Delete any account | ✅ | — | — | — | — |

### AI and Content

| Action | Super Admin | Advisor | Sub-Advisor | Student | Parent |
|---|---|---|---|---|---|
| Edit global AI system prompts | ✅ | — | — | — | — |
| Edit organisation-level prompts | — | ✅ | — | — | — |
| Use AI mentor chat | — | — | — | ✅ | — |
| Issue certificates | — | ✅ | If permitted | — | — |
| Generate a Journey Map PDF | ✅ | — | — | ✅ | ✅ |

---

## 3. How Sub-Advisor Permissions Work

Sub-Advisors do not have a fixed permission set. Their access is configured entirely by their primary Advisor using the **Permission Matrix**.

- An Advisor can grant a Sub-Advisor access to *any combination* of modules they themselves hold.
- An Advisor **cannot** grant a Sub-Advisor more rights than the Advisor has.
- Sub-Advisors can also be scoped to a specific student group — for example, only the students in "Class of 2026" — so they cannot see any other students even within the same organisation.

> **Example:** An Advisor might create a Sub-Advisor account for an office assistant, giving them access only to *Forms* and *Notifications* but no access to *Students*, *Groups*, or *Support Tickets*.

---

## 4. How Parent Access Works

Parents have a deliberately limited view to protect student privacy:

- A parent can only see data for students they are explicitly linked to.
- The student controls the link — they must approve a parent's request from their own dashboard.
- Parents can view progress, recommendations, and Journey Maps, but they cannot edit anything.
- In schools where Parent Chat is enabled, parents can message the advisor through a secure thread that is separate from the student-advisor channel.

![Diagram showing the relationship between Admin, Advisor, Sub-Advisor, Student, and Parent roles with arrows indicating who can see or manage whom](/docs-idpicker/images/user-manual/getting-started/roles-diagram.png)

Image placeholder: Add a diagram showing the five roles and the directional relationships between them \u2014 e.g., Admin oversees all, Advisor manages Sub-Advisor and Students, Parent links to Student.

---

## Common Questions

| Situation | What to do |
|---|---|
| A sub-advisor says they cannot see a specific student | Check their Assigned Scope in Sub-Advisor Management — they may only be scoped to certain groups, and the student is in a different group |
| A parent can see their child but cannot chat with the advisor | Family Chat must be enabled by the Advisor. The advisor can open the Chat module and confirm the parent thread is active |
| I need to give an advisor admin-level access to one feature only | Use the Sub-Admin (Admin-level) permission matrix rather than making them a full Super Admin |
