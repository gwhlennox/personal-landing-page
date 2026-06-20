# Changelog

All notable changes to this project will be documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased]

### Added
- Nav logo replaced with circular headshot avatar (greyscale, colour on hover)
- Hero portrait photo to the right of name
- Contact pills in hero: Email, WhatsApp, Telegram (with SVG icons)
- Nested projects within portfolio cards: SideShift.ai → Akindo Buildathon, Pay API Growth; Accenture → Kingfisher PLC, Modern Data Stack; NTT Data → McDonald's, Value Retail, Howdens

### Changed
- Nav order updated to: Portfolio, Articles, Media, About, Contact
- Kingfisher PLC and McDonald's/Value Retail removed as standalone top-level cards (now nested under Accenture and NTT Data respectively)
- Headshot removed from About section (now in hero)

### Todo
- Update Telegram username in `src/pages/index.astro` (currently placeholder)

---

## [2026-06-20]

### Changed
- Replaced Tailwind CDN with plain CSS (`src/styles/global.css`) — more reliable, no runtime dependency
- Removed `@astrojs/tailwind` and `tailwindcss` from dependencies
- Rewrote HTML to use semantic class names instead of utility classes
- Upgraded semantic HTML: `<article>` for portfolio cards, `aria-label` on contact nav

### Added
- `.gitignore` (node_modules, dist, .env, .astro)
- `CHANGELOG.md`

### Removed
- Stray UUID-named photo file from repo root
- Unused Tailwind dependencies from `package.json`

### Fixed
- CSS not loading on production Vercel URL

---

## [2026-06-19]

### Added
- Astro project scaffold with minimal template
- Sticky navigation with smooth scroll links
- Hero section with name and positioning statement
- Portfolio section: 2-column grid of 9 brand cards (Accenture, Kingfisher PLC,
  Value Retail, NTT Data, McDonald's, SideShift.ai, Olapic, Peerius, Incopro)
- Media and Articles sections linking to Linktree
- About section with bio and circular headshot
- Contact section with email, LinkedIn, and Linktree links
- Footer
- Headshot as favicon (square-cropped PNG)
- Vercel deployment via GitHub integration
- `README.md` with stack, local dev, and deploy instructions

### Content
- Dates and roles populated from CV for Accenture, Kingfisher PLC, Value Retail,
  NTT Data, SideShift.ai, and Peerius
- Bio and hero copy added
- LinkedIn URL: `linkedin.com/in/george--lennox`
- Placeholder lorem ipsum descriptions (to be replaced)
- Placeholder dates for McDonald's, Olapic, Incopro (to be updated)

---

[Unreleased]: https://github.com/gwhlennox/personal-landing-page/compare/HEAD...HEAD
