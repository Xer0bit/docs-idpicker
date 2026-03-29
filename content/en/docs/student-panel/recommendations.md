---
title: "Recommendation"
description: "How to use AI-driven university and career recommendations, refine by exam scores or personality, and filter results by country and city"
weight: 24
draft: false
---

The Recommendations page is the heart of the IDPicker platform. Once your assessments are complete, the AI generates a personalized list of universities or career paths that match your profile. You can then sharpen those results in two powerful ways: by feeding in your real exam scores and rankings, or by leaning entirely on your completed personality profile. This guide walks through every option step by step.

---

## 1. Opening Your Recommendations

1. In the left sidebar, click **Recommendations**.
2. The page loads your results and displays a summary banner — for example, **"Found 3 personalized recommendations"** — along with a pass counter (e.g. **1/2**) that tracks how many refinement passes have been applied.
3. Scroll down to see your university or career cards ranked by match strength.
4. Click any card title to open its full detail view, which explains precisely why the AI selected it for your profile.

> **Tip:** The pass counter next to the summary banner increments each time you apply a new set of filters. Use it to compare how your results change between refinement passes.

![Recommendations summary banner showing found count, pass counter, and ranked university cards below](/images/user-manual/student-panel/recommendations-overview.png)

*Image placeholder: Add screenshot of the Recommendations page — show the summary banner with found count and pass counter, and at least 2 university cards ranked below it.*

---

## 2. Choosing a Recommendation Input Mode

Before the AI refines your results, you must tell it what data to prioritise. Click **Refine Results** (top-right button) to open the refinement panel, then select one of the two **Recommendation input** modes:

| Mode | What it uses | Best for |
|---|---|---|
| **Test Scores** | Your entrance exam names, scores, and rankings | Students who have sat official exams and know their results |
| **Personality** | Your completed personality assessment on IDPicker | Students who want a purely trait-based match without exam data |

Click the tile for the mode you want — the selected tile gets a highlighted border.

![Recommendation input section showing Test Scores tile and Personality tile with selection highlight](/images/user-manual/student-panel/recommendations-input-mode.png)

*Image placeholder: Add screenshot of the refinement panel showing both input mode tiles (Test Scores and Personality) with one selected and highlighted.*

---

## 3. Refining With Test Scores (Exam-Based Mode)

This mode lets you enter the entrance exams you have actually sat, together with your score and ranking. Universities use these figures as admission criteria, so providing them produces the most accurate shortlist.

### 3a. How the Score Palette Works

IDPicker supports up to **3 exam slots** (shown as **1/3** in the panel). Each slot captures:

- **Exam name** — the official name of the test (e.g. *IELTS*, *SAT*, *TOEFL*)
- **Score** — the numeric result you received
- **Ranking** *(optional)* — your position or percentile, e.g. *Top 5%* or *1000th*

> **Design tip shown in the panel:** Blend aptitude, language, and speciality exams for a balanced story. For example, adding both a language exam (IELTS) and an aptitude exam (SAT) gives the AI richer data to match against university requirements.

### 3b. Adding Your First Exam (Step by Step)

1. In the refinement panel, confirm **Test Scores** is selected.
2. You will see a numbered row labelled **1** with three input fields: **Exam name**, **Score**, and **Ranking (optional)**.
3. Click the **Exam name** field and type the name of your exam (e.g. *YKS-SAY*).
4. Click the **Score** field and enter your numeric score.
5. Click the **Ranking (optional)** field and enter your rank if known (e.g. *Top 5%* or *15000th*).

![Exam score palette showing exam name, score, and ranking input fields for the first exam slot](/images/user-manual/student-panel/recommendations-exam-slot.png)

*Image placeholder: Add screenshot of the exam score palette with the first slot’s Exam name, Score, and Ranking (optional) fields visible and empty.*

### 3c. Adding a Second or Third Exam

1. Click the **+** button on the right side of the palette row counter.
2. A new numbered row appears.
3. Fill in **Exam name**, **Score**, and **Ranking** for the additional exam.
4. Repeat for a third exam if needed (maximum 3 slots).

> **Note:** The **+** button is disabled once all 3 slots are filled. To replace an exam, clear an existing row first.

### 3d. Real-World Example — Turkish YKS Exam

Turkey uses the **YKS** university entrance system, which includes several sub-tests. A typical student entry looks like this:

| Field | Example Value |
|---|---|
| Exam name | YKS – SAY (Science) |
| Score | 487.32 |
| Ranking | 8500th |

The SAY sub-score is the figure Turkish universities use to rank applicants for science and engineering faculties. Entering it gives IDPicker the exact criterion those universities apply, so the recommendation list mirrors real admission eligibility.

Other common Turkish exam entries:
- **YKS – EA** (Equally Weighted) — used for economics, law, business
- **YKS – SÖZ** (Verbal) — used for humanities and social sciences
- **YKS – DİL** (Language) — used for foreign language degree programmes

![Score palette with YKS-SAY exam name, numeric score, and ranking filled in as a real example](/images/user-manual/student-panel/recommendations-yks-example.png)

*Image placeholder: Add screenshot of the score palette with YKS–SAY entered as exam name, a numeric score, and a ranking value filled in as a demonstrative example.*

### 3e. Applying Your Scores

1. After filling in all your exam rows, click **Apply All Filters** (bottom-right of the refinement panel).
2. The platform saves your score palette and triggers a new recommendation pass.
3. The pass counter in the summary banner increments (e.g. from **1/2** to **2/2**).
4. Your ranked list updates to reflect universities whose admission criteria your scores meet.

![Apply All Filters button highlighted at the bottom of the refinement panel](/images/user-manual/student-panel/recommendations-apply-filters.png)

*Image placeholder: Add screenshot of the Apply All Filters button at the bottom of the refinement panel, highlighted or in focus.*

---

## 4. Refining With Personality (Trait-Based Mode)

If you have completed the Personality assessment on IDPicker, you can let the AI use your psychological trait scores instead of exam data.

1. In the refinement panel, click the **Personality** tile.
2. The exam score fields disappear — no manual input is required.
3. Click **Apply All Filters**.
4. The AI re-ranks your recommendations based on trait compatibility with each university or career programme.

> **Note:** This mode requires a completed Personality assessment. If you have not finished it, the tile may be locked. Go to [Assessment](/docs/student-panel/assessment/) first.

![Personality tile selected in the recommendation input section with no additional input fields visible](/images/user-manual/student-panel/recommendations-personality-mode.png)

*Image placeholder: Add screenshot of the refinement panel with the Personality tile selected — no exam input fields should be visible.*

---

## 5. Filtering by Country

The **Refine by Country** dropdown narrows results to universities located in a specific country before the AI applies its ranking logic.

1. In the refinement panel, click the **Select country** dropdown under **Refine by:**.
2. Scroll or type to find your target country.
3. Select it — the dropdown updates to show the chosen country.
4. Click **Apply All Filters** to reload results for that country only.

> **Tip:** Combine country filtering with an exam mode for the tightest shortlist. For example, selecting *Turkey* + entering YKS–SAY scores surfaces only Turkish universities that accept your specific score range.

![Country dropdown open with a country selected in the Refine by section of the recommendations panel](/images/user-manual/student-panel/recommendations-country-filter.png)

*Image placeholder: Add screenshot of the country dropdown open with a country selected inside the Refine by section.*

---

## 6. Filtering by City

After country-level filtering, you can drill down further by city using the **Filter by city** control that appears above the results list.

1. Scroll past the refinement panel to the **Filter by city** row.
2. Click the city dropdown (defaults to **All cities**).
3. Select the city you want — only universities in that city will show.

> **Note:** City-level filtering is applied independently of the refinement panel. You do not need to click **Apply All Filters** again — city changes take effect immediately.

![Filter by city dropdown showing All cities default and a city selection in context of the results list](/images/user-manual/student-panel/recommendations-city-filter.png)

*Image placeholder: Add screenshot of the Filter by city row above the results — show the dropdown open with All cities default and one city option highlighted.*

---

## 7. Reading the Recommendation Cards

Each university card in your results list displays key admission and programme information at a glance:

| Element | What it shows |
|---|---|
| **University name** | Full official name including city and type (state/private) |
| **Premium badge** | Marks universities available to Premium-tier subscribers only |
| Programme details | Faculty, degree type, and language of instruction |
| Match indicators | Visual signals showing how closely the university fits your profile |

Click the university name to open its full detail page showing all programmes, requirements, and the AI's reasoning for the match.

![University recommendation card showing name, city, Premium badge, and programme detail summary](/images/user-manual/student-panel/recommendations-card-detail.png)

*Image placeholder: Add screenshot of a recommendation card showing university name, city, Premium badge, and programme detail summary (mask any real student data).*

---

## 8. Downloading Your Full Report

If your account plan supports it, you can export your recommendation profile as a PDF.

1. Look for the **Download My Report** button at the top of the recommendations page.
2. Click it and wait for the document to be prepared.
3. A secure link opens in a new tab — click it to save the PDF.

> **Note:** If the button is hidden, report export is not enabled for your current plan or organisation policy. Check your subscription under **Settings**.

![Download My Report button and secure PDF link in a new tab](/images/user-manual/student-panel/recommendations-report-download.png)

*Image placeholder: Add screenshot of the Download My Report button at the top of the page, and optionally the PDF open in a new browser tab.*

---

## Common Questions

| Situation | What to do |
|---|---|
| The recommendations feel inaccurate | Retake the assessment if you rushed through it, then apply filters again |
| I want career results, not universities | Use the Guidance Track switcher to change focus — see [Assessment](/docs/student-panel/assessment/) |
| The Personality tile is locked | Complete the Personality assessment first under the Assessment module |
| I entered my YKS score but the list did not change | Make sure you clicked **Apply All Filters** after entering the score |
| The **+** button to add more exams is disabled | You have reached the 3-exam limit. Clear one row to replace it |
| City filter shows no results | The selected country may not have city-level data. Try **All cities** |
| Report download failed | Wait 60 seconds and try again — intermittent network drops can interrupt PDF generation |
| Pass counter is stuck at 1/2 | A failed filter apply may have stopped the count. Re-apply your filters and check your connection |
