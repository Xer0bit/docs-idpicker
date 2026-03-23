---
title: "01. Authentication Guide"
description: "Detailed click-by-click authentication walkthrough"
weight: 121
draft: false
---

This guide explains exactly how a student signs in, registers, verifies email, and recovers account access.

## What You Need Before Starting

- Student login URL from [Access URLs](../getting-started/access-urls/)
- Valid email address
- Stable internet connection
- Access to your email inbox (and spam folder)

## A) Sign In with Email and Password (Click-by-Click)

1. Open the student login page.
2. Click the Email field.
3. Type your registered email.
4. Click the Password field.
5. Type your password.
6. Optional: Click the eye icon to reveal password and verify typing.
7. Click Sign In.
8. Wait for redirect.

Expected result:

- You are redirected to dashboard.
- If you were opening a protected page before login, you are redirected there.

If it fails:

- Check that both fields are filled.
- Recheck uppercase/lowercase in password.
- If message indicates verification is required, follow section C.

## B) Sign In with Google (Click-by-Click)

1. Open login page.
2. Click Continue with Google.
3. Choose Google account.
4. Approve consent if prompted.
5. Return to IDPicker tab/window and wait for callback completion.

Expected result:

- You are authenticated and redirected to dashboard flow.

If it fails:

- Allow popups/new tab in browser.
- Retry from login page.
- If account linking is incomplete, complete requested follow-up prompts.

## C) Register New Student Account (Click-by-Click)

Registration is multi-step. The exact order can vary by invitation and configuration.

Typical sequence:

1. Click Sign Up on login page.
2. Fill account details (name, email, password).
3. Confirm password and consent.
4. Continue to interests and goals selections.
5. Fill profile information (education level, gender, social links, occupation).
6. Select organization or continue with invitation-prefilled values.
7. Complete human verification.
8. Click final registration action.

Validation rules to watch:

- Password must satisfy strength checks (length, uppercase, lowercase, number, special character).
- Duplicate email is blocked.
- Consent is required.

## D) Verify Email After Registration

1. Open your email inbox.
2. Find verification email from IDPicker.
3. Click verification link.
4. Wait for verification status page.
5. If valid, continue to dashboard/profile completion.

If link is expired:

1. Return to login.
2. Enter your email.
3. Use resend verification action.
4. Open latest verification email and retry.

## E) Forgot Password (Request Reset Link)

1. Open login page.
2. Click Forgot Password.
3. Click email input.
4. Enter registered email.
5. Click Send Reset Link.
6. Check inbox and spam for reset message.

## F) Reset Password from Email Link

1. Open reset link from email.
2. Wait for token validation screen to finish.
3. Enter new password.
4. Enter confirm password.
5. Verify password strength indicator is acceptable.
6. Click Reset Password.
7. Return to login and sign in with new password.

If token is invalid/expired:

- Go back to Forgot Password and request a fresh link.

## Common Student Questions

Q: I entered correct password but still cannot access account.
A: Most common cause is unverified email. Use resend verification from login.

Q: I clicked Google login but stayed on same page.
A: Check popup blocking, then retry.

Q: Reset link opened but does not allow password update.
A: Reset token likely expired; request a new one.

![Student Login Placeholder](/images/user-manual/student-panel/auth-login-email.png)

Image placeholder: Login form with filled fields and Sign In button.

![Google OAuth Placeholder](/images/user-manual/student-panel/auth-login-google.png)

Image placeholder: Google selection + successful callback state.

![Password Reset Placeholder](/images/user-manual/student-panel/auth-password-reset.png)

Image placeholder: Token-valid reset page with password strength checks.
