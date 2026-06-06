# Responsive Portfolio Implementation Plan

**Goal**: Ensure the portfolio website (`index.html`, `style.css`, `script.js`) displays optimally on both desktop and mobile devices.

## User Review Required
> [!IMPORTANT]
> Review the proposed breakpoints and design decisions. Approve to proceed.

## Open Questions
> [!QUESTION]
> Do you have any specific mobile design preferences (e.g., collapsed menu style, font sizes) beyond the standard responsive adjustments?

## Proposed Changes
---
### CSS (`style.css`)
- Add media queries for breakpoints at 1024px and 768px.
- Adjust `.nav-links` to become a vertical overlay on mobile and show the `menu-btn`.
- Change `.hero-grid` from two columns to single column on small screens.
- Stack `.about-grid` and `.skills-grid` into single column layout.
- Reduce grid columns in `.projects-grid` from 3 to 2 (tablet) and 1 (mobile).
- Scale typography with `clamp` where needed.
- Ensure images and badges resize.
- Update paddings/margins for sections.

### JavaScript (`script.js`)
- Ensure the mobile menu toggle works with new CSS classes.
- Already present; no changes needed.

## Verification Plan
- Manually resize browser window to test layouts.
- Use Chrome dev tools device mode for common devices (iPhone 13, iPad, desktop).
- Verify navigation links work and menu opens/closes.
- Ensure no overflow or horizontal scroll.
