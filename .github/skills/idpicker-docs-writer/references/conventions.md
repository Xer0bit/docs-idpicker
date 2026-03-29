# IDPicker Docs — Writing Conventions

Full style guide for all content under `content/en/docs/`.

---

## Front Matter

### Leaf Pages (all `.md` except `_index.md`)
```yaml
---
title: "Feature Name"
description: "One-line summary of what this page covers"
weight: <int>
draft: false
---
```

### Section Index (`_index.md`)
```yaml
---
title: "Panel Name"
description: "One-line audience + scope summary"
weight: <int>
---
```

`_index.md` files **never** include `draft`.

---

## Weight Schema

Sections occupy "decade" slots; children increment by 1 from the section base:

| Section | Base Weight | Child range |
|---|---|---|
| `docs/_index.md` | 5 | — |
| `getting-started/` | 10 | 11–19 |
| `student-panel/` | 20 | 21–29 |
| `advisor-panel/` | 30 | 31–39 |
| `parent-panel/` | 40 | 41–49 |
| `admin-panel/` | 50 | 51–59 |
| `help/` | 60 | 61–69 |

Leave gaps when inserting in the middle (e.g., if 41 and 42 exist, insert at 43, not 41.5).

---

## Page Body Structure

### Opening Paragraph
Start every page with **1–3 lines of prose** (no heading) explaining:
- Who this guide is for
- What the page covers

Do **not** repeat the `title` or `description` in the body.

### Heading Levels

| Level | Rule | Example |
|---|---|---|
| `##` H2 | Major sections — always **numbered** | `## 1. Requesting a Link` |
| `###` H3 | Sub-sections — **not** numbered | `### What You CAN Do` |
| `####` H4 | Rare; only for deeply nested topics | — |

### Section Separators
Place a horizontal rule `---` **after every H2 block** (before the next `##` or end of file).

---

## Text Formatting

| Element | Format | Example |
|---|---|---|
| UI buttons, fields, clickable labels | `**Bold**` | `**Sign In**`, `**Email**` |
| Tips (inline, end of section) | `*Italic*` | `*Tip: You can also...* ` |
| Notes (inline, mid-section) | `*Italic*` | `*Note: Sub-advisors cannot...* ` |
| Optional steps | `*(Optional)*` prefix | `*(Optional)* Click **Skip** to proceed later.` |
| Code / URLs | No backticks — use inline plain text or raw link | — |

---

## Procedural Steps

All how-to instructions use **numbered ordered lists**, one action per item:

```markdown
1. Navigate to the login page.
2. Click the **Email** field and type your address.
3. Click **Sign In**.
```

- Do NOT use bullets for steps that must happen in sequence.
- Outcome branches after a step use **bold bullet labels**:

```markdown
- **Instant Link:** The student's profile appears immediately.
- **Pending Link:** A request is sent; wait for the student to approve.
```

---

## Callouts (Blockquotes)

Use native Markdown blockquotes — **no Hugo/Docsy shortcodes**.

| Pattern | When to Use |
|---|---|
| `> **Tip:** text` | Helpful hints, shortcuts |
| `> **Warning:** text` | Destructive, irreversible, or risky actions |
| `> **Note:** text` | Important but non-destructive caveats |
| `> **Quota Warning:** text` | Subscription/limit notices |
| `> **Why X?** text` | Inline rationale for non-obvious behavior |

Example:
```markdown
> **Warning:** Removing access is immediate and cannot be undone from the parent side.
```

---

## Tables

### Common Questions (required, every leaf page)
Must be the **last section** of every leaf page:

```markdown
## Common Questions

| Situation | What to do |
|---|---|
| I cannot see my student's profile | Confirm the link request was accepted in the student's notification inbox. |
| The link is showing as "Pending" | Ask your student to open their notifications and approve the connection. |
```

### Feature Overview Tables
For dashboards or multi-attribute feature listings:

```markdown
| Block | What It Shows | Action |
|---|---|---|
| Progress Ring | Overall completion % | Click to open detail view |
```

### Permission Split Tables
When documenting access levels, prefer `### What You CAN Do` / `### What You CANNOT Do` H3 + bullet lists over a table (matches existing pattern in the codebase).

---

## Images

Every visual should have a placeholder until the real screenshot is available:

```markdown
![Feature Name Placeholder](/images/user-manual/<panel-folder>/<feature-name>.png)

Image placeholder: Add screenshot of [brief description] (mask any sensitive data).
```

**Path convention:** `/images/user-manual/<panel-name>/<descriptive-filename>.png`

Panel folder names: `student-panel`, `advisor-panel`, `parent-panel`, `admin-panel`, `getting-started`

---

## Cross-Links

Always use Hugo's `{{< relref >}}` shortcode for internal links. This is the only pattern that works correctly under the `/docs-idpicker/` base path — both in local dev and on GitHub Pages. Plain absolute `/docs/...` paths do **not** include the base path prefix and will 404.

```markdown
[Parent Dashboard]({{< relref "/docs/parent-panel/dashboard-and-linked-overview" >}})
[Access URLs]({{< relref "/docs/getting-started/access-urls" >}})
```

Omit the trailing `/` inside `relref`. Hugo will resolve to the correct URL automatically.

---

## Section Index (`_index.md`) Body Structure

```markdown
<1-3 paragraph intro: audience, scope, what they can do>

## Who Should Use This Guide
<bullet list of roles>

## Suggested Reading Order
1. [Page Title](/docs/<section>/<slug>/)
2. ...

## Core Features & Responsibilities
- Feature one
- Feature two

![Section Overview Placeholder](/images/user-manual/<panel>/overview.png)
Image placeholder: Add screenshot of the <panel> dashboard.
```

`_index.md` files do **not** end with a "Common Questions" table.

---

## What NOT to Do

- No `{{< alert >}}`, `{{< tabpane >}}`, `{{< cardpane >}}` — other Docsy shortcodes are not used in content
- No plain absolute `/docs/...` links — use `{{< relref >}}` instead (bare paths break under the base URL prefix)
- No `linkTitle` front matter field
- No `date` front matter field — Git info handles this
- No backticks for URLs or UI labels
- No un-numbered H2 headings
- No `---` separator on the very last line of a file (only between sections)
