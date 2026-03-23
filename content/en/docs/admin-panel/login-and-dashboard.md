---
title: "Admin Login and Dashboard"
description: "Detailed click-by-click admin authentication and dashboard workflow"
weight: 151
draft: false
---

## Admin Login (Click-by-Click)

1. Open the Admin dashboard login URL.
2. Enter username or email.
3. Enter password.
4. Click Sign In.
5. Wait for redirect to dashboard.

Expected result:

- Admin auth cookie is set.
- Dashboard loads KPI cards and recent activity.

## Password Reset

1. Open reset-password route.
2. Enter account email.
3. Submit reset request.
4. Open reset link from inbox.
5. Set new password.
6. Log in again.

## Dashboard First Checks

1. Confirm KPI cards load.
2. Check recent assessments table.
3. Review registration trend chart.
4. Verify system activity panel updates.

## Token Usage and Activity

1. Open token usage section.
2. Select date range/interval.
3. Review input/output token trends.
4. Cross-check spikes with logs module.

## Common Questions

Q: Login works but dashboard widgets are empty.
A: Wait for API load and refresh once; verify API base URL and token validity.

Q: I keep returning to login.
A: Session cookie may be invalid/expired; clear cookies and reauthenticate.

![Admin Login Placeholder](/images/user-manual/admin-panel/admin-login.png)

Image placeholder: Admin login and post-login dashboard KPI cards.
