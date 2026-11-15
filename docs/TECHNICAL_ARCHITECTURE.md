# Technical Architecture — Boredom Breaker

**Current architecture:** React 19 + TypeScript + Vite 7, client-side single-page application.

## Repository structure (observed)
- `src/main.tsx` — React entry point and global stylesheet import.
- `src/App.tsx` — page state, navigation, filtering, favorites and view composition.
- `src/data/activities.ts` — static categories and activity catalogue.
- `src/styles.css` — global styles, components and responsive rules.
- `index.html` — document metadata and font loading.

## State and persistence
- React component state for current page, selected activity, language, category, search and duration.
- Favorites stored in browser localStorage under `bb-saved`.
- No backend, authentication, database or analytics dependency in the current implementation.

## Architectural principles
- Preserve the current stack unless a concrete product requirement justifies a change.
- Keep the first version lightweight.
- Separate content data from presentation.
- Move reusable UI and domain logic into focused modules when changes make App.tsx difficult to maintain.
- Validate and safely parse persisted browser data.
- Do not introduce Supabase until accounts, cross-device sync or shared data are validated requirements.
- Add product analytics only when there is a clear measurement question, consent/privacy approach and implementation plan.

## Risks / technical debt to inspect
- Main application component currently contains multiple views and helper components.
- Toast timeout lifecycle should be checked.
- Category/content localisation is incomplete in source.
- No test framework or automated component tests were observed in package scripts.
- Accessibility and runtime behaviour need browser verification.

## Environment and security
- No credentials are required for the current static/localStorage MVP.
- Keep secrets out of source control.
- If a backend is introduced later, document data ownership, access policies and migrations before implementation.
