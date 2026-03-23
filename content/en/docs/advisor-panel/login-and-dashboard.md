---
title: "Advisor Login and Dashboard"
description: "Detailed click-by-click login, session, and dashboard guide"
weight: 131
draft: false
---

This guide covers advisor access, role-based session behavior, and first dashboard checks.

## A) Advisor Login (Click-by-Click)

1. Open advisor login URL from [Access URLs](../getting-started/access-urls/).
2. Click Email field and enter advisor email.
3. Click Password field and enter password.
4. Click Sign In.
5. Wait for session initialization.
6. Confirm redirect to dashboard.

Expected result:

- Advisor session is loaded with role and permission set.
- User lands on advisor dashboard.

If login fails:

- Re-check email/password.
- Confirm account status is active.
- Use request/reset password flow if needed.

## B) First-Time Password Setup

For invited advisors/sub-advisors:

1. Open setup-password link from email.
2. Enter new password and confirm.
3. Submit setup form.
4. Return to login and sign in.

## C) Password Reset Flow

1. Open request-password/reset-password page.
2. Enter advisor email.
3. Request reset email.
4. Open reset link and set new password.
5. Sign in again.

## D) Dashboard Navigation (Click-by-Click)

1. After login, open dashboard home.
2. Review top overview blocks (metrics/summary widgets).
3. Open Assigned Forms block and verify current pending items.
4. Use sidebar to verify access to Students, Groups, Resources, and Support Tickets.
5. Confirm language preference control works if available in dashboard header.

## E) Role and Permission Behavior

Advisor role:

- Full operational access based on organization policies.

Sub-advisor role:

- Access is limited to delegated permissions.
- Some modules/actions may be hidden or disabled.

## Common Advisor Questions

Q: I logged in but cannot see expected modules.
A: Check whether account is sub-advisor with restricted permissions.

Q: Login succeeds but dashboard appears partially loaded.
A: Wait for session and dashboard API calls to finish, then refresh once.

Q: Password setup link does not work.
A: Request a fresh password setup/reset email.

![Advisor Login Placeholder](/images/user-manual/advisor-panel/advisor-login.png)

Image placeholder: Add login screen and post-login dashboard landing view.
