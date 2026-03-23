---
title: "Authentication and Account"
description: "Detailed click-by-click parent authentication guide"
weight: 141
draft: false
---

This guide covers parent login, registration, verification, setup-password, and reset-password flows.

## A) Parent Login (Click-by-Click)

1. Open parent login URL from [Access URLs](../getting-started/access-urls/).
2. Click email/username input.
3. Enter your parent account email.
4. Click password input.
5. Enter password.
6. Optional: Click eye icon to reveal password.
7. Click Sign In.
8. Wait for redirect to `/dashboard`.

Expected result:

- Parent auth token cookie is set.
- Parent dashboard loads.

## B) Parent Registration (Click-by-Click)

1. Open Register page.
2. Fill email.
3. Fill full name.
4. Fill password.
5. Enable consent checkbox.
6. Click Register.
7. Verify toast/confirmation message about email verification.
8. Return to login.

## C) Verify Email

1. Open verification link from email.
2. Wait for auto-verification.
3. On success, parent is redirected to dashboard.
4. If token invalid/expired, use resend verification.

## D) Setup Password from Invitation Link

1. Open setup-password URL with token.
2. Wait for token validation.
3. Enter new password (minimum length requirement applies).
4. Confirm password.
5. Submit.
6. Return to login and sign in.

## E) Request Password Reset

1. Open login reset-password page.
2. Enter parent email.
3. Click Send Reset Link.
4. Check inbox/spam folder.

## F) Complete Password Reset

1. Open reset link with token.
2. Enter new password.
3. Confirm password.
4. Submit reset.
5. Log in with updated password.

## Common Parent Questions

Q: Login returns parents-only error.
A: Credentials belong to non-parent role; use correct parent account.

Q: Verification link expired.
A: Use resend verification action on verify-email page.

Q: Reset link works but password submit fails.
A: Ensure minimum length and confirm-password match.

![Parent Login Placeholder](/images/user-manual/parent-panel/parent-login.png)

Image placeholder: Parent login page with successful redirect.

![Parent Verify Placeholder](/images/user-manual/parent-panel/parent-verify-email.png)

Image placeholder: Verify-email success and resend fallback states.
