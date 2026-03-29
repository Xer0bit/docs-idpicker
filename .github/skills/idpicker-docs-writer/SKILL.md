---
name: idpicker-docs-writer
description: 'Write, review, and extend Hugo/Docsy user documentation for the IDPicker platform. Use when: creating new doc pages, writing panel guides (student, advisor, parent, admin), adding sections, reviewing existing docs for convention compliance, or generating frontmatter. Knows IDPicker feature set, all panels, section weight schema, Markdown conventions, callout patterns, image placeholder syntax, and cross-link format.'
argument-hint: 'Describe the page or feature to document, e.g. "student dashboard page" or "advisor bulk import section"'
---

# IDPicker Docs Writer

A skill for writing, reviewing, and extending user-facing documentation for the **IDPicker** platform — a Hugo site built with the Docsy theme, hosted at `https://xer0bit.github.io/docs-idpicker/`.

## When to Use

- Creating a **new leaf page** for any panel section
- Creating or updating a **section `_index.md`**
- **Reviewing** an existing page for convention compliance
- Drafting **feature documentation** from a description or screenshot
- Generating the correct **frontmatter** for a new page
- Determining the correct **weight** and **path** for a new page
- Writing **Common Questions** tables, callouts, permission tables

---

## Project Overview

IDPicker is a career and university guidance platform with five user roles, each documented in its own panel section.

| Panel | Audience | Section Weight |
|---|---|---|
| Getting Started | All users | 10 |
| Student Panel | Students | 20 |
| Advisor Panel | Advisors & Sub-advisors | 30 |
| Parent Panel | Parents/Guardians | 40 |
| Admin Panel | Super-admins & Org-admins | 50 |
| Help | All users | 60 |

See [project structure reference](./references/project-structure.md) for the full file map and weight assignments.

---

## Procedure

### 1. Identify Page Type & Location

- **Leaf page** → goes under the relevant panel folder; follow [leaf page template](./assets/leaf-page-template.md)
- **Section index** → `_index.md` in the relevant folder; follow [section index template](./assets/section-index-template.md)
- Confirm the **weight** by checking the [project structure reference](./references/project-structure.md)

### 2. Set Frontmatter

```yaml
---
title: "Feature Name"            # Sentence case, concise
description: "One-line purpose"  # Shown in sidebar + meta; max ~20 words
weight: <section_base + offset>  # e.g. 43 for the 3rd page in parent-panel (40s)
draft: false                     # Always explicit on leaf pages
---
```

`_index.md` files omit `draft`.

### 3. Write the Body

Follow the full [writing conventions](./references/conventions.md). Key rules:

- Open with **1–3 lines of prose** — who this page is for and what it covers
- Use `---` to separate every H2 section
- Number all H2 headings: `## 1. Title`, `## 2. Title`, …
- Use `**Bold**` for every UI button, field, or clickable element
- Use **numbered lists** for all procedural steps
- Use `> **Label:** text` blockquotes for callouts — no Hugo/Docsy shortcodes
- End every leaf page with a `## Common Questions` table
- Add image placeholders: `![Feature Placeholder](/images/user-manual/<panel>/<file>.png)`

### 4. Review Checklist

Before finalising any page, verify:

- [ ] Frontmatter has `title`, `description`, `weight`, `draft: false`
- [ ] Weight fits the section decade and doesn't clash with existing pages
- [ ] Every H2 is numbered starting at `## 1.`
- [ ] `---` separator after every H2 block
- [ ] All button/field names are `**Bold**`
- [ ] All steps are numbered lists
- [ ] Callouts use `> **Label:** text` format
- [ ] Page ends with `## Common Questions` table
- [ ] Cross-links use absolute `/docs/...` paths (no `relref`)
- [ ] Image placeholders follow `/images/user-manual/<panel>/<feature>.png` path pattern

---

## Reference Files

| File | Contents |
|---|---|
| [Writing Conventions](./references/conventions.md) | Full style guide — headings, callouts, tables, images, links |
| [Project Structure](./references/project-structure.md) | Complete section/file map with weights |
| [Leaf Page Template](./assets/leaf-page-template.md) | Blank template for a new feature page |
| [Section Index Template](./assets/section-index-template.md) | Blank template for a new `_index.md` |
