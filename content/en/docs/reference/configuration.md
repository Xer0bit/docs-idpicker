---
title: "Configuration Reference"
description: "Environment variables, route conventions, auth cookies, and operational settings"
weight: 51
draft: false
---

This page documents high-impact configuration values used across IDPicker modules.

## 1. Core Environment Variables

| Key | Typical Value (Local) | Used By | Purpose |
|---|---|---|---|
| NEXT_PUBLIC_API_BASE_URL | http://localhost:8000/api | Student, Advisor, Parent, Admin dashboards | Base API URL for frontend requests |
| NODE_ENV | development / production | All frontends | Runtime mode and behavior switches |

Notes:

1. Frontends append role-specific paths in API clients where needed.
2. Some shared endpoints remove role suffix at runtime in client helper logic.

## 2. Local Frontend Dev URLs

| App | Typical Local URL |
|---|---|
| Student module frontend | http://localhost:3000 |
| Admin dashboard | http://localhost:3001 |
| Advisor dashboard | http://localhost:3002 |
| Parent dashboard | http://localhost:3003 |

## 3. Authentication Cookies (Frontend)

| Role | Cookie Name | Purpose |
|---|---|---|
| Student | authToken | Student API authorization token |
| Advisor | authTokenAdvisor | Advisor API authorization token |
| Parent | authTokenParent | Parent API authorization token |
| Admin | authTokenAdmin | Admin API authorization token |

Operational notes:

1. Most clients send token using `Authorization: Token <value>`.
2. Expiry and refresh behavior depend on backend auth policy.

## 4. High-Impact Routing Conventions

| Pattern | Meaning |
|---|---|
| /dashboard | Default authenticated landing route |
| /dashboard/{module} | Module-specific workspace |
| /dashboard/{entityId} | Entity detail page |
| /form/{responseId} | Dynamic form response route |
| /login, /reset-password, /verify-email, /setup-password | Authentication utility routes |

## 5. Status and Priority Conventions

Support tickets commonly use:

- Status: pending, in_progress, resolved, closed
- Priority: low, medium, high, urgent

These values should be treated as canonical unless backend schema changes.

## 6. Localization Conventions

| Item | Convention |
|---|---|
| Supported locales | English and Turkish |
| Namespace usage | Feature/module namespace prefixes |
| Fallback behavior | Default locale used when key missing |

## 7. Safe Configuration Change Process

1. Update environment variable in target deployment.
2. Restart relevant frontend/backend services.
3. Validate login and one API call per role.
4. Validate one localized page in EN and TR.
5. Validate one ticket/notification flow for operational modules.

## 8. Configuration Validation Checklist

1. API base URL resolves from frontend container/browser.
2. Auth cookie is created after login for target role.
3. Protected routes redirect correctly for unauthenticated users.
4. Form response route and dashboard route both resolve.
5. Translation API and language switch operations respond correctly.
