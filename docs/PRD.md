# Product Requirements — Boredom Breaker

**Status:** Draft based on existing implementation  
**Version:** 0.1

## Problem statement
People with unstructured free time may struggle to choose an enjoyable activity and get started. This problem and target segment still require validation.

## Product objective
Help a user move from “I don't know what to do” to a suitable activity with clear next steps.

## Current functional requirements
| ID | Requirement | Current implementation | Status |
|---|---|---|---|
| FR-01 | Show a clear home/discovery entry point | Home hero and category sections | Implemented in source; runtime QA pending |
| FR-02 | Browse activities by category | Six category filters/cards | Implemented in source; runtime QA pending |
| FR-03 | Search activity title/description | Search field | Implemented in source; runtime QA pending |
| FR-04 | Filter by duration | Duration select | Implemented in source; runtime QA pending |
| FR-05 | Suggest a random activity | Surprise Me action | Implemented in source; runtime QA pending |
| FR-06 | Show instructions and materials | Activity detail view | Implemented in source; runtime QA pending |
| FR-07 | Save and remove favorites | localStorage | Implemented in source; persistence QA pending |
| FR-08 | Switch English/Portuguese interface | Language toggle | Partially implemented; activity content needs translation audit |
| FR-09 | Support phone and desktop layouts | Responsive CSS | Implemented in source; visual QA pending |

## UX requirements
- A user should understand the app's purpose immediately.
- Discovery should require few steps.
- Every activity should communicate what it is, approximate duration and difficulty.
- Detail pages should make the first step obvious.
- Save actions must provide clear feedback.
- Empty, no-results and saved states must explain what the user can do next.
- Mobile navigation and controls must remain usable at narrow widths.

## Non-functional requirements
- Mobile-first responsive layout.
- Semantic controls, keyboard access and visible focus.
- Respect reduced-motion preferences.
- No unnecessary collection of personal data.
- Keep the first version lightweight and runnable without an account.
- Avoid introducing paid services without validated need.

## Acceptance criteria for the next review
- Critical user journeys work on phone and desktop.
- Favorites persist after refresh and handle invalid localStorage data gracefully.
- Search, categories and duration filters compose correctly.
- Surprise Me always returns a valid activity for the selected scope.
- Language behaviour is consistent across navigation, filters, categories, cards and detail content.
- No dead controls, horizontal overflow or console errors in tested journeys.

## Out of scope for this version
Accounts, backend sync, AI recommendations, payments and social features.
