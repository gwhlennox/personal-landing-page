# Changelog

All notable changes to this project will be documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased]

### Added
- Individual company pages via Astro dynamic routing (`/experience/[slug]`)
- `src/data/experience.js` — single source of truth for all experience data
- Company pages include: summary, headcount, team size, website link, case studies
- "View more →" arrow link on each experience card linking to its page
- "Read more →" link in hero scrolling to About section
- "Case Studies" label replacing "Projects" on cards and company pages

### Changed
- Hero title: "Customer Success & Chief of Staff" → "Strategic Partnerships & Operations Leader"
- Hero subheader updated to "10+ years building partnerships..."
- Section label: "Portfolio" → "Experience" (nav and heading)
- Nav anchor updated: `#portfolio` → `#experience`
- Olapic role: → "Project Manager"
- Incopro role: → "Database Manager"
- Location updated to "London, UK" (footer and About section)

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
