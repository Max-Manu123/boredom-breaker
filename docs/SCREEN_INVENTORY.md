# Screen Inventory — Boredom Breaker

**Status:** Initial inventory from source-code inspection; screenshot/visual QA pending.

| Screen / state | Purpose | Main elements | Key actions | Status |
|---|---|---|---|---|
| Home | Explain value and start discovery | Brand, hero, Surprise Me, category cards, featured ideas | Surprise, browse category, open idea | Exists |
| Explore | Find an activity | Search, duration filter, category pills, results grid | Search, filter, open, save | Exists |
| Saved | Revisit favorites | Saved activity grid, empty state | Open, remove favorite, explore | Exists |
| Activity detail | Help user start | Activity illustration, category, duration, difficulty, description, steps, materials, Bori tip | Save/unsave, back | Exists |
| Global navigation | Move between main areas | Desktop sidebar, mobile bottom nav, language toggle | Navigate, switch language | Exists |
| Toast feedback | Confirm save changes | Temporary status message | Dismisses automatically | Exists |

## States to verify or improve
- Initial load.
- Empty saved list.
- Search with results.
- Search with no results.
- Category + duration + search combined.
- Saved item after reload.
- Invalid or unavailable localStorage.
- Long activity title and long translated copy.
- Narrow mobile viewport and keyboard navigation.
- Portuguese translations across all visible content.

## Questions for design review
- Is the primary action obvious without competing calls to action?
- Is the mascot helping comprehension or only decoration?
- Are category descriptions and activity metadata readable on small screens?
- Does the detail page make the first action clear?
- Are icon-only controls understandable to assistive technology?
