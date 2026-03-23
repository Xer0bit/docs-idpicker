---
title: "Prompts, Translations, and Content"
description: "How to edit the AI system prompts and localize the platform interface text"
weight: 155
draft: false
---

The core intelligence and language of IDPicker is not hard-coded; it is entirely manageable via the Admin Panel. This allows you to tune the AI Mentors and translate the UI on the fly without requiring engineering deployments.

---

## 1. Managing System Prompts

The system prompts dictate exactly how the AI Mentors behave, what tone they use, and how they analyze student data.

1. Open the **Prompts** module.
2. Select the specific category and subcategory you want to tune (e.g., *Mentor Persona > Academic Strict*).
3. Open the target prompt template.
4. Edit the instructions in the code editor.
5. **CRITICAL:** Do not delete dynamic variables (e.g., `{{student_name}}` or `{{assessment_score}}`). Removing these breaks the AI's contextual awareness.
6. Validate the syntax and click **Save**. The updated prompt version is now live instantly.

---

## 2. Interface Translations (Localization)

If you need to fix a typo in the UI, or launch the platform in a brand new language, use the Translations manager.

1. Open the **Translations** module.
2. Use the filters to select a specific **Namespace** (e.g., `student_dashboard`) and **Locale** (e.g., `es-ES` for Spanish).
3. Use the search bar to locate the specific key or the incorrect phrase.
4. Click Edit, type the corrected translation, and save.
5. If you are adding a completely new phrase required by a recent UI update, use the **Create Translation** action to add the missing key.

*Cache Warning: Translations are heavily cached in users' browsers for speed. Force clear your local browser cache to verify the UI updated correctly.*

---

## 3. Configuring Mentor Personalities

You can directly manage the roster of AI Mentors available to students.

1. Open the **Mentor Personality** section.
2. You can tweak a mentor's localized name, short description, and their internal *Expertise Array* (which dictates what tags they are allowed to give advice on).
3. Ensure you save your changes before leaving the page.

---

## Common Questions

| Situation | What to do |
|---|---|
| I saved an updated Prompt but it threw a "Template Syntax Error" | You likely broke a brace bracket around a variable, like typing `{student_name}}` instead of `{{student_name}}`. Fix the brackets and retry |
| I updated a Translation but the user still sees the old text | Instruct the user to perform a "Hard Refresh" (Ctrl+F5) to clear their browser cache, or wait for the CDN cache to expire |
| The AI Mentor is going "off script" | Revisit your System Prompt. Ensure the instructions are explicit, using commands like 'DO NOT EVER suggest...'. AI models require explicit, rigid boundaries |
