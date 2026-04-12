---
title: "Authentication"
description: "How students sign in, register, verify email, and recover access — complete step-by-step walkthroughs"
weight: 21
draft: false
---

Everything students need to create an account, sign in, and recover access starts here. Follow each section from top to bottom the first time through; returning users can jump directly to the relevant flow.

---

## 1. Before You Begin

Make sure you have:

- The **student login URL** for your environment — see [Access URLs]({{< relref "/docs/getting-started/access-urls" >}})
- A valid email address you can check immediately
- A stable internet connection and an up-to-date browser

---

## 2. Sign In with Email and Password

This is the fastest path for returning students.

1. Open the student login URL.
2. Click the **Email** field and type your registered email.
3. Click the **Password** field and type your password.
4. *(Optional)* Click the **eye icon** next to the password field to reveal what you typed.
5. Click **Sign In** and wait for the redirect.

**What happens next:**
- You land on your **Dashboard**.
- If you were navigating to a specific page before login, you are sent directly there instead.

**If sign-in fails:**
- Double-check for typos — passwords are case-sensitive.
- If you see a message about email verification, follow the [Verify Your Email](#verify-your-email) section below.
- If you have forgotten your password, use [Forgot Password](#forgot-password).

![Student login page showing email and password fields with Sign In button](/docs-idpicker/images/user-manual/student-panel/authentication-login.png)

---

## 3. Sign In with Google

Faster sign-in without a separate password.

1. Open the student login page.
2. Click **Continue with Google**.
3. A Google account picker opens — select the account you want to use.
4. Approve the consent screen if prompted.
5. You are redirected back to IDPicker and land on the dashboard.

**If the login window stays on the same page:**
- Your browser may be blocking popups. Allow popups for this site and try again.
- Make sure you are not using a private/incognito window with strict tracking prevention.

![Continue with Google button and Google account picker dialog](/docs-idpicker/images/user-manual/student-panel/authentication-google-signin.png)

---

## 4. Register a New Account

New students follow a multi-step wizard. The exact steps depend on whether you received an invitation link.

1. Click **Sign Up** on the login page.
2. Fill in your **name**, **email**, and a strong **password**.
   - Password must contain at least one uppercase letter, one number, and one special character.
3. Confirm the password and check the consent checkbox.
4. Complete the **interests and goals** step.
5. Fill out your **profile** (education level, gender, social links, occupation).
6. Select an organization if prompted, or continue with invitation-prefilled values.
7. Complete the **human verification** step.
8. Click the final **Register** button.

> **Tip:** If you were invited by an advisor, your organization field may already be filled in. Do not change it unless instructed.

**Common registration blockers:**
- Duplicate email → use a different address or try [Forgot Password](#forgot-password) if you already registered.
- Consent checkbox not checked → scroll down and tick the box.
- Weak password → make sure it meets all strength requirements shown on screen.

![Multi-step registration wizard showing name, email, password, interests, and profile fields](/docs-idpicker/images/user-manual/student-panel/authentication-register.png)

---

## 5. Verify Your Email

After registration, IDPicker sends a verification email.

1. Open your **email inbox** (check your spam/junk folder too).
2. Find the email from IDPicker with subject **Verify your email**.
3. Click the **verification link** inside.
4. Wait for the verification confirmation page.
5. Once verified, you are directed to your dashboard or profile completion.

**If the link says it has expired:**

1. Return to the login page.
2. Enter your email and click **Resend Verification Email**.
3. Open the new email and click the fresh link.

![Email verification page confirming the link was clicked successfully](/docs-idpicker/images/user-manual/student-panel/authentication-verify-email.png)

---

## 6. Forgot Password

Use this if you cannot remember your current password.

1. Open the login page and click **Forgot Password**.
2. Enter your registered email address.
3. Click **Send Reset Link**.
4. Check your inbox and spam folder for the reset email.

![Forgot password form with registered email input and Send Reset Link button](/docs-idpicker/images/user-manual/student-panel/authentication-forgot-password.png)

---

## 7. Reset Password From the Email Link

After requesting a reset, you will receive a link by email.

1. Click the link from the IDPicker reset email.
2. Wait a moment for the token to be validated.
3. Enter your **new password**.
4. Enter the same **password again** to confirm.
5. Watch the strength indicator — make sure it reaches acceptable strength.
6. Click **Reset Password**.
7. Return to the login page and sign in with your new password.

**If the link says the token is invalid or expired:**
- Request a new reset link from the [Forgot Password](#forgot-password) step above.

![Reset password form with new password field, confirm password field, and strength indicator](/docs-idpicker/images/user-manual/student-panel/authentication-reset-password.png)

---

## Common Questions

| Situation | What to do |
|---|---|
| Correct password rejected | Likely unverified email — resend verification from the login page |
| Google login popup closed immediately | Enable popups for the IDPicker domain in your browser settings |
| Reset link opens but password field is grayed out | Token expired — request a fresh reset link |
| Registration stuck on verification | Check spam folder; if email is over 30 minutes old, resend |
