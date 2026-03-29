---
title: "Support Tickets"
description: "How to triage, respond to, and close student-reported issues from the advisor panel"
weight: 41
draft: false
---

The Support Tickets module is your direct line to students who are having trouble with the platform. This guide explains how to triage incoming requests, update their status, and write resolution messages so students know their issue is being handled.

---

## 1. Opening the Ticket Queue

1. In the sidebar, click **Support Tickets**.
2. The queue loads with a summary row at the top showing counts by status: *Pending*, *In Progress*, *Resolved*, *Closed*.
3. By default, the list is sorted by most recent — oldest unresolved issues may be buried. Reorder by **Priority** immediately.

> **Tip:** Start every support session by filtering for **Priority: Urgent** and **Status: Pending**. These are the issues blocking students right now.

![Support ticket queue showing status summary cards and a filtered list sorted by priority](/images/user-manual/advisor-panel/support-tickets-queue.png)

Image placeholder: Add screenshot of the support ticket queue showing the status summary cards at top and the filtered ticket list below.

---

## 2. Filtering and Prioritising Tickets

1. Use the **Status** filter dropdown to narrow to a single stage (*Pending*, *In Progress*, *Resolved*, *Closed*).
2. Use the **Priority** filter to show only high-urgency items (*Low*, *Medium*, *High*, *Urgent*).
3. Combine both filters for maximum efficiency — e.g., Status: *Pending* + Priority: *High* gives you the most critical unresolved work.
4. Sort the filtered list by **Created Date** (oldest first) to avoid letting old issues age out.

---

## 3. Reviewing a Ticket

1. Click any ticket row or card to open its detail view.
2. Read the **Subject** and full **Description** the student provided.
3. Check the **User Details** panel on the right — this shows which student submitted it, their organisation, and their account status.
4. Note the **Category** badge (e.g., *Account*, *Assessment*, *Billing*, *Technical*). This tells you which team should handle it if escalation is needed.
5. Check the **Timestamps** — is this a fresh ticket or has it been sitting for days?

![Ticket detail view showing subject, description, user details panel, category badge, and timestamps](/images/user-manual/advisor-panel/support-ticket-detail.png)

Image placeholder: Add screenshot of an open ticket detail view with the student info panel, description, and status dropdown visible.

---

## 4. Updating Ticket Status

1. In the ticket detail, locate the **Status** dropdown.
2. Change it to match your current work state:
   - **In Progress** — You have started investigating and the student should expect a reply soon.
   - **Resolved** — You have applied a fix or provided an answer.
   - **Closed** — The issue is fully finalized and archived.
3. Click **Save** (or the status change auto-saves, depending on your platform version).
4. Confirm the status badge in the list view has updated.

*Note: Do not jump directly from **Pending** to **Resolved** without first setting **In Progress**. This leaves a confusing audit trail and the student has no indication you saw their message.*

---

## 5. Writing a Resolution Message

Resolution messages are crucial — they are the student-facing reply that appears in their Help Center.

1. In the ticket detail, find the **Resolution Message** text area.
2. Write a clear, actionable response:
   - Acknowledge the issue.
   - Explain what you found or did.
   - Give any steps the student needs to take next.
3. Click **Save**.
4. Change the status to **Resolved**.

> **Warning:** Some platforms require the Resolution Message to be filled before the status can be changed to *Resolved*. If saving the status fails silently, check that the resolution field is not blank.

![Resolution message text area filled in with a clear response and the Resolved status selected](/images/user-manual/advisor-panel/support-ticket-resolution.png)

Image placeholder: Add screenshot of the resolution message field filled in alongside the status dropdown set to Resolved.

---

## 6. Reopening a Ticket

If a student replies that the issue is still happening after you marked it resolved:

1. Open the closed or resolved ticket.
2. Change the status back to **In Progress**.
3. Add an updated Resolution Message acknowledging the continuation.
4. Investigate further and repeat the resolution flow.

---

## Common Questions

| Situation | What to do |
|---|---|
| I changed the status but it did not save | Check if the Resolution Message field is required — fill it in and try saving again |
| There are too many tickets to manage at once | Apply both Status and Priority filters together. Handle Urgent+Pending first, then High+Pending |
| A student says their issue is unresolved but the ticket is Closed | Reopen it by setting the status back to In Progress, add an updated message, and reinvestigate |
