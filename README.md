# Amici Pitch Deck

Pre-seed pitch deck for Amici, the event platform for businesses without an event team.

**Live deck:** [amici-pitch.vercel.app](https://amici-pitch.vercel.app)

## How to view

Open `index.html` in any browser or visit the live URL above. Navigate with arrow keys, dot navigation, or swipe on mobile.

## How to update

1. Edit `index.html` (locally or on GitHub)
2. Commit and push to `main`
3. Vercel auto-deploys — the live URL updates within a minute

## Structure

The deck is a single self-contained HTML file. No build step, no dependencies, no framework. All CSS, JS, and content live in one file.

### Slides

1. Cover
2. The Problem
3. Why Now
4. Journey So Far (traction)
5. What We've Learned (insights)
6. Product flow (instant pricing)
7. Product vision — mockups
8. Product vision — supplier engine
9. Competitive Landscape
10. Market Opportunity
11. Business Model
12. Team
13. The Platform (technical foundation)
14. The Ask

The deck is bilingual (Swedish default, English available via the top-right toggle). All text edits must update both `translations.sv` and `translations.en` in the `<script>` block in `index.html`.

## Design system

- Dark theme with blue accent (`#3B82F6`)
- Typography: Quattrocento (display), Quattrocento Sans (body), Roboto Mono (monospace)
- Responsive: works on desktop, tablet, and mobile
- Animations: staggered fade-up on slide transitions
