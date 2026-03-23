---
title: "FAQ"
description: "Frequently asked questions with practical answers"
weight: 62
draft: false
---

## Access and Accounts

### 1. I cannot log in. What should I check first?

1. Confirm you are using the correct panel URL for your role.
2. Re-enter username/email and password carefully.
3. Check whether your email verification is pending.
4. Use password reset if you suspect credential mismatch.

### 2. Why do I get redirected back to login?

Most common causes:

- Expired or invalid auth cookie
- Wrong role token used on another panel
- Backend session/token invalidation

Fix:

1. Sign out.
2. Clear browser cookies for the app domain.
3. Sign in again with correct role URL.

### 3. I completed registration but cannot access dashboard.

1. Verify email from inbox link.
2. Retry login after verification.
3. If link expired, use resend verification.

## Student/Parent Linking

### 4. Parent cannot see linked student immediately.

Linking may remain pending until both sides complete required actions.

1. Parent submits link request with correct student email.
2. Student side confirms matching flow where required.
3. Parent refreshes dashboard.

## Assessments, Recommendations, and Reports

### 5. Why is a module locked?

Some modules unlock only after required assessments or permissions are completed.

### 6. Report download button is missing.

Report export availability may depend on:

- Completion state
- Plan/quota state
- Backend report generation status

## Support and Operations

### 7. Ticket status did not update.

1. Reopen ticket detail.
2. Ensure required fields (for example resolution note) are present.
3. Save again and refresh list.

### 8. Notification reached wrong users.

This is usually a target-selection issue.

1. Verify target type (all/users/groups).
2. Validate selected recipients before send.

## Localization

### 9. Language changed but some text stayed in old language.

1. Refresh page once.
2. Confirm selected language is persisted.
3. Check missing translation key in translations module (admin/advisor).

## Performance

### 10. Dashboard feels slow.

1. Reduce heavy filters/date ranges.
2. Reload once to clear stale state.
3. Check status/log modules for backend latency spikes.
