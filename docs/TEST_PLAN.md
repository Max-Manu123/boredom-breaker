# Test Plan — Boredom Breaker

**Status:** Planned; no test execution recorded in this document.

## Critical manual journeys
1. Home → Explore → open activity → back.
2. Home → Surprise Me → detail.
3. Save activity → reload page → verify it remains saved.
4. Remove favorite → verify it disappears from Saved.
5. Search by title and description.
6. Combine category and duration filters.
7. Clear search and return to all results.
8. Switch language and inspect all visible text.
9. Verify empty Saved and no-results states.
10. Use navigation and controls with keyboard only.

## Responsive checks
- 320px narrow phone.
- 375–390px common phone widths.
- 768px tablet.
- 1024px small desktop/tablet landscape.
- 1440px desktop.

Check for horizontal overflow, clipped controls, unreadable text, overlap and usable touch targets.

## Accessibility checks
- Semantic headings and landmarks.
- Accessible names for icon-only controls.
- Visible focus indicators.
- Keyboard-operable navigation, filters and save actions.
- Sufficient text/background contrast.
- Reduced-motion preference respected.

## Automated checks available
- `npm run typecheck`
- `npm run build`

## Reporting format
For every check, record **Passed**, **Failed** or **Not run**, plus date, environment and notes. A successful production build does not prove every user journey works.
