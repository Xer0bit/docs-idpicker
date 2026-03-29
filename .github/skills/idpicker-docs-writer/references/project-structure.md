# IDPicker Docs — Project Structure

Full file map for `content/en/docs/` with weights and purposes.

---

## Root

| File | Weight | Purpose |
|---|---|---|
| `docs/_index.md` | 5 | Landing page for the manual |
| `docs/getting-started.md` | — | Legacy standalone page (not in sidebar nav) |

---

## Getting Started (weight: 10)

| File | Weight | Purpose |
|---|---|---|
| `getting-started/_index.md` | 10 | Section landing |
| `getting-started/overview.md` | ~11 | Platform overview |
| `getting-started/quick-start.md` | 22 | Login → Dashboard → First action flow |
| `getting-started/access-urls.md` | 23 | Production + staging URL registry |

---

## Student Panel (weight: 20)

| File | Weight | Purpose |
|---|---|---|
| `student-panel/_index.md` | 20 | Section landing |
| `student-panel/authentication.md` | 21 | Email/Google sign-in, register, verify, reset |
| `student-panel/dashboard.md` | 22 | Dashboard blocks, first 5 actions |
| `student-panel/assessment.md` | 23 | Career/skill assessments |
| `student-panel/recommendations.md` | 24 | University & program recommendations |
| `student-panel/personality.md` | 25 | Personality profile feature |
| `student-panel/ai-mentorship.md` | 26 | AI mentor conversations |
| `student-panel/university-search.md` | 27 | University search & filter |
| `student-panel/resources.md` | 28 | Learning resources library |
| `student-panel/help-center.md` | — | In-app help center access |
| `student-panel/subscription.md` | — | Subscription plans & upgrade |
| `student-panel/account-settings.md` | — | Profile, password, notifications |
| `student-panel/assigned-forms.md` | — | Forms assigned by advisor |
| `student-panel/certificates-and-documents.md` | — | Certificates and document uploads |
| `student-panel/language.md` | — | Language/locale preference |

---

## Advisor Panel (weight: 30)

| File | Weight | Purpose |
|---|---|---|
| `advisor-panel/_index.md` | 30 | Section landing |
| `advisor-panel/login-and-dashboard.md` | 31 | Advisor login, sub-advisor caveat, KPIs |
| `advisor-panel/students-and-bulk-import.md` | 32 | Student management, CSV bulk import |
| `advisor-panel/groups.md` | 36 | Cohort creation & management |
| `advisor-panel/forms-and-responses.md` | — | Form assignment & response review |
| `advisor-panel/resources.md` | — | Resource library management |
| `advisor-panel/support-tickets.md` | — | Support ticket handling |
| `advisor-panel/notifications.md` | — | Notification center |
| `advisor-panel/certificates-and-application-documents.md` | — | Certificate issuance & document review |
| `advisor-panel/sub-advisor-management.md` | — | Sub-advisor creation & permission config |
| `advisor-panel/enrollment-family-chat-and-assessments.md` | — | Enrollment tracking, family chat, assessments |
| `advisor-panel/profile-prompts-and-interests.md` | — | Student profile prompts & interest mapping |

---

## Parent Panel (weight: 40)

| File | Weight | Purpose |
|---|---|---|
| `parent-panel/_index.md` | 40 | Section landing |
| `parent-panel/authentication-and-account.md` | 41 | Parent registration, setup, sign-in, reset |
| `parent-panel/dashboard-and-linked-overview.md` | 42 | Parent dashboard, linked student summary |
| `parent-panel/linked-student-guide.md` | 44 | Link request flow, view profile, unlink, permissions |
| `parent-panel/student-detail-journey-map-and-chat.md` | — | Student journey map, family chat |
| `parent-panel/forms.md` | — | Forms assigned to parent |

---

## Admin Panel (weight: 50)

| File | Weight | Purpose |
|---|---|---|
| `admin-panel/_index.md` | 50 | Section landing |
| `admin-panel/login-and-dashboard.md` | 51 | Super-admin login, KPI cards, token usage |
| `admin-panel/user-and-organization-management.md` | 52 | Org setup, user CRUD |
| `admin-panel/admin-and-subadmin-management.md` | — | Admin role management |
| `admin-panel/assessments-and-forms.md` | — | Global assessment & form configuration |
| `admin-panel/prompts-translations-and-content.md` | — | Content, AI prompts, translation management |
| `admin-panel/support-notifications-and-approvals.md` | — | Support queue, notifications, approvals |
| `admin-panel/system-monitoring-and-governance.md` | — | System health, audit logs, governance |

---

## Help (weight: 60)

| File | Weight | Purpose |
|---|---|---|
| `help/_index.md` | ~60 | Section landing |
| `help/faq.md` | 62 | Q&A by topic category |
| `help/troubleshooting.md` | — | Common error resolution |

---

## Misc Sections

| Section | Weight | Notes |
|---|---|---|
| `product/_index.md` | — | Role/panel architecture overview |
| `usage/best-practices.md` | — | Best practices for platform use |
| `usage/common-tasks.md` | — | Quick-reference task list |
| `reference/configuration.md` | — | Configuration reference |

---

## Image Paths

Images live under `static/images/user-manual/` and are referenced as `/images/user-manual/...` in Markdown.

Folder naming mirrors section folder names:
- `student-panel/`
- `advisor-panel/`
- `parent-panel/`
- `admin-panel/`
- `getting-started/`

---

## Hugo Configuration Highlights

| Setting | Value |
|---|---|
| Base URL | `https://xer0bit.github.io/docs-idpicker/` |
| Theme | Docsy v0.14.3 |
| Offline search | Enabled (Lunr.js) |
| Git info | Enabled (last-modified date) |
| Sidebar | Compact mode |
| Raw HTML in Markdown | Allowed |
| Build command | `hugo --gc --minify` |
| Dev server | `hugo server` |
