---
title: "Troubleshooting"
description: "Operational playbooks for common platform issues"
weight: 61
draft: false
---

Use these playbooks when users report blocked workflows.

## Playbook 1: Cannot Sign In

Symptoms:

- Invalid credentials error
- Redirect loop to login
- Role mismatch message

Checks:

1. Confirm correct role URL.
2. Confirm account exists and is active.
3. Confirm email verification status.
4. Clear cookies and retry login.

Escalate when:

- Multiple users fail with same error pattern.
- Login endpoint responds with server errors.

## Playbook 2: Form Cannot Submit

Symptoms:

- Submit button fails silently
- Validation error persists
- Response not saved

Checks:

1. Verify required fields are filled.
2. Verify field type input is valid (email/number/date).
3. Retry submit after reload.
4. Validate response route ID is correct.

Escalate when:

- Reproducible failure on same form for multiple users.
- Backend returns repeated 5xx errors.

## Playbook 3: Parent-Student Link Not Visible

Symptoms:

- Link request sent but student not listed
- Link status remains pending

Checks:

1. Verify student email exact match.
2. Verify student account exists in same environment.
3. Ask both users to refresh after completing link steps.

Escalate when:

- Link status remains pending beyond expected SLA.

## Playbook 4: Ticket Queue Not Updating

Symptoms:

- Status change appears unsaved
- Resolved tickets reappear as pending

Checks:

1. Reopen ticket and confirm latest status in detail view.
2. Ensure required resolution message fields are populated.
3. Save and refresh list.

Escalate when:

- Persistence fails across multiple ticket IDs.

## Playbook 5: Notification Delivery Issues

Symptoms:

- Notification sent to unintended audience
- Expected recipients missing

Checks:

1. Verify target type.
2. Verify selected user/group IDs.
3. Re-send with a small test target first.

Escalate when:

- Delivery metrics mismatch persisted target selection.

## Playbook 6: Dashboard Performance Degradation

Symptoms:

- Slow initial load
- Chart/table timeout
- Intermittent failed fetches

Checks:

1. Reduce date range/filter complexity.
2. Compare behavior in another module.
3. Inspect status/realtime logs for error bursts.
4. Retry after short interval.

Escalate when:

- p95 latency remains elevated across modules.
- Logs indicate systemic backend faults.

## Incident Handoff Template

When escalating, include:

1. Role and panel (student/advisor/parent/admin)
2. Exact URL/route
3. Timestamp and timezone
4. Reproduction steps
5. Error text and screenshot
6. Expected vs actual behavior
7. Whether issue is single-user or widespread
