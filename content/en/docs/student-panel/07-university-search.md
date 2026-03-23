---
title: "07. University Search Guide"
description: "Detailed click-by-click university search walkthrough"
weight: 127
draft: false
---

This guide explains exactly how students search, filter, and compare universities/programs.

## Open University Search

1. In sidebar, click University Search.
2. Wait for filter panel and results area to load.
3. Confirm default result set appears.

## Basic Search (Keyword)

1. Click search input.
2. Type university or program keyword.
3. Pause briefly (search is debounced).
4. Review refreshed results.

## Filter Search (Click-by-Click)

### Category filter

1. Click Category dropdown.
2. Select one category.
3. Wait for results refresh.

### Degree filter

1. Click Degree dropdown.
2. Select degree type.
3. Wait for results refresh.

### Language filter

1. Click Language dropdown.
2. Select instruction language.
3. Wait for results refresh.

### Page size

1. Click Page Size.
2. Choose 6, 12, or 24.
3. Results repaginate automatically.

## Pagination and Load More Behavior

1. Scroll through current page results.
2. Use pagination/load action to fetch next set.
3. Continue until target programs are found.

Important:

- Changing any filter resets pagination to first page.
- Combined filters can reduce results to zero.

## Reset to Default Search

1. Click reset/clear filter action.
2. Remove keyword if needed.
3. Confirm full default result set returns.

## Compare Programs Efficiently

For each card, note:

- University name
- Program name
- Degree
- Language
- Tuition
- Duration
- Country

Then shortlist in your own note-taking sheet.

## Common Student Questions

Q: Search feels delayed when typing.
A: Input is debounced to avoid unnecessary API requests.

Q: I have no results after adding one filter.
A: Remove filters one by one to find restrictive combination.

Q: Results order changed after filter update.
A: New query produces a fresh paginated result set.

![University Search Placeholder](/images/user-manual/student-panel/university-search.png)

Image placeholder: Search bar + active filters + result cards + pagination.
