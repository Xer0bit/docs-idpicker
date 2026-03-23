---
title: "Parent Forms"
description: "Detailed click-by-click parent form response guide"
weight: 145
draft: false
---

Parent panel supports dynamic form responses through `/form/{responseId}` routes.

## A) Open Parent Form

1. Open form link from dashboard, notification, or direct URL.
2. Wait for form load.
3. Confirm form title/description is visible.
4. If organization banner exists, review context section at top.

## B) Fill Form Fields (Click-by-Click)

For each question:

1. Read label and required marker.
2. Enter/select answer according to field type.
3. Continue until all required fields are complete.

Supported field types include:

- text
- email
- number
- textarea
- dropdown
- date/time/datetime
- rating
- radio
- checkbox

## C) Submit Form

1. Scroll to submit action.
2. Click Submit.
3. Wait for success toast.
4. Confirm form state updates.

## D) Read-Only Form State

If a response already exists and edit is disabled:

- Form displays prior answers.
- Inputs are non-editable.
- Parent can review but not change.

## Common Parent Questions

Q: Form did not load.
A: Link may be invalid/expired or response ID may be incorrect.

Q: Submit failed.
A: Recheck required fields and retry.

Q: Why cannot I edit previous answer?
A: Form is configured as non-editable after submit.

![Parent Form Placeholder](/images/user-manual/parent-panel/parent-form-response.png)

Image placeholder: Parent form with mixed question types and submit action.
