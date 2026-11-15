# Design System — Boredom Breaker

**Status:** Baseline extracted from existing CSS; not yet approved as final.

## Visual direction
Playful, welcoming and energetic, with a dark-purple foundation, warm yellow accent and a friendly mascot. Avoid making the interface visually noisy; content discovery should remain the focus.

## Existing tokens
| Token | Current value | Use |
|---|---|---|
| Background | `#21143d` | Main app background |
| Sidebar background | `#1b1032` | Navigation surface |
| Panel | `#2c1d4b` | Cards and panels |
| Secondary panel | `#352456` | Secondary surfaces |
| Accent purple | `#7550d9` | Brand/illustration |
| Accent yellow | `#f6d34a` | Primary action and highlights |
| Muted text | `#b9aecb` | Supporting text |
| Border | `rgba(255,255,255,.09)` | Subtle separators |
| Font | Nunito | Current interface typography |

## Existing patterns
- Rounded cards and category surfaces.
- Yellow primary button with visible hover feedback.
- Purple category colour variations.
- Desktop sidebar and mobile bottom navigation.
- Activity cards with category, duration and difficulty.
- Detail view with materials, steps and a Bori tip.
- Visible keyboard focus outline.
- Reduced-motion media query.

## Required design review
- Verify contrast for small muted text and coloured category surfaces.
- Check touch target sizes and spacing on small screens.
- Ensure icon-only save and clear buttons have clear accessible names.
- Review long text wrapping and layout stability.
- Verify loading, empty, no-results, success and error states.
- Review the mascot's role and consistency.
- Check all screens at phone, tablet and desktop widths.

## Design approval
The current CSS is a baseline, not a final design approval. Record approved changes in `APPROVAL_LOG.md`.
