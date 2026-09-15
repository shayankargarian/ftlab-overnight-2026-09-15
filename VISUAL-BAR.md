# Phone reports visual bar

Standing standard for **all** files under `/workspace/phone-reports/`. Friend Desk UI is a separate product. Do not mix Bloomberg terminal chrome into phone reports.

## Must

- **Phone-first** - design and QA at **390px** width (typical viewport height ~844).
- **Hero visual** at top - image (`assets/…`) or strong CSS hero. Not a plain text header alone.
- **Chart.js** (CDN) for any **Proven** numeric series only. Never invent points. Unknown years/values stay labelled, not plotted as fake data.
- **Soft / Proven / Unknown** colour system:
  - Soft → gold (`#c9a227` / `#d4af6a`)
  - Proven → teal (`#3d9b8f` / `#5cb8ab`)
  - Unknown → risk red (`#c45c5c` / `#d47878`)
- **Dinner callout** - sticky or early highlighted card titled **Dinner / what to say**, **3-5 bullets max**.
- **DRAFT / noindex** - `robots` noindex; visible DRAFT banner; Australian English; **no em dashes**.
- **Colour, graphs, images** - not sparse text cards. Prefer badges, charts, hero, and visual hierarchy over walls of prose.

## Must not

- Invent credit, BNPL, or other stock volumes.
- Plot Unknown API nulls as chart points.
- Import Friend Desk / Bloomberg terminal chrome (multi-pane watchlists, equity quotes chrome, dense status rails).
- Publish without `draft_needs_approval` framing when content is Gate-paused.

## Files

- Reports: `YYYY-MM-DD-*.html`
- Shared assets: `assets/`
- Index: `index.html` (light list; same Soft/Proven colours, DRAFT, noindex)
