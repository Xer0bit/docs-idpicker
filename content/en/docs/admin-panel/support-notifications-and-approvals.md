---
title: "Support, Notifications, and Approvals"
description: "How to handle incoming support tickets, broadcast global alerts, and manage admission gates"
weight: 56
draft: false
---

This module covers the operational workflows for global customer support and gating access to the platform via formal approvals.

---

## 1. Managing Support Tickets

When a student or advisor submits a Help Center request, it routes to this global queue.

1. Open **Support Tickets**.
2. Immediately filter the queue by **Priority: Urgent** and **Status: Pending** to catch blockers.
3. Click into a ticket to read the user's description and reproduction steps.
4. Once you have a fix or answer, change the **Status** (e.g., from *In Progress* to *Resolved*).
5. Type your official response in the Resolution Message field.
6. Click **Save**. The user will see your response on their local Help Center dashboard.

*Note: If a ticket transition fails silently, re-open it. You likely forgot to fill out a mandatory "Resolution Message" field before trying to change the status to Resolved.*

![Global support ticket queue showing filter controls, ticket rows with priority and status badges, and a resolution message field](/images/user-manual/admin-panel/support-tickets-admin.png)

*Image placeholder: Add screenshot of the admin support ticket queue filtered to Urgent + Pending, with an open ticket showing the resolution message field.*

---

## 2. Generating Global Notifications

While Advisors notify their specific students, Super Admins can push alerts globally across all active organizations on the platform.

1. Open **Notifications**.
2. Click **Create Notification**.
3. Choose your target scope extremely carefully:
   - **All Users:** Every active student, parent, and advisor. (Use for major platform maintenance warnings only).
   - **All Students:** All students regardless of organization.
   - **Selected Groups:** Specific subsets if necessary.
4. Write your Title and Message, then hit **Send**.
5. Once sent, verify it appears correctly in your broadcast history.

![Global notification composer showing target scope dropdown set to All Students, title and message fields, and Send button](/images/user-manual/admin-panel/notifications-global.png)

*Image placeholder: Add screenshot of the global notification composer with target scope, title, and message filled in before sending.*

---

## 3. Demo Approvals and Admission Criteria

If IDPicker is operating a gated launch or pilot program, you must manually approve access.

1. Open the **Demo Approvals** or **Admission Criteria** queue.
2. Review the incoming request details submitted by prospective users or schools.
3. Click **Approve** to officially provision their workspace and trigger the welcome email sequence.
4. Click **Reject** if they do not meet compliance standards (you can usually append an internal note explaining the rejection).

---

## Common Questions

| Situation | What to do |
|---|---|
| I accidentally sent a Global Notification to everyone | Platform notifications are instant and cannot be recalled. If the error was severe, send an immediate correction broadcast apologizing for the error |
| I approved a Demo request but the user got an error logging in | Verify the organization template mapped to their approval was fully provisioned. Sometimes the backend provisioning queue takes 30-60 seconds |
| Can I assign a ticket to a specific subadmin? | If your Support module supports assignment flags, use the 'Assignee' dropdown inside the ticket detail before saving |
