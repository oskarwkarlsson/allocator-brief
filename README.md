# Oskar's Allocator Brief
Daily brief for hedge fund business relations people: investor relations, capital raising, business development, capital introduction and allocator coverage. Static GitHub Pages site (main, root). Yellow/pink theme in `style.css`. No build step. Sources: SOURCES.md.

Cadence: Sunday to Friday, 06:30 Europe/Berlin. Sunday covers Friday and Saturday; Monday covers since Sunday; other days cover since the previous edition (about 24h).

## Sections (class / chip)
| Class | Chip | Section | Covers |
|---|---|---|---|
| `launch` | Launch | Launches, raises & closures | New funds, capital raised, fund closes, wind-downs, fundraising halts |
| `alloc` | LPs | Allocators & mandates | Pensions, endowments, insurers, SWFs, family offices, FoFs: commitments, results, surveys, policy |
| `gulf` | Gulf | Gulf capital & Abu Dhabi | ADIA, Mubadala, ADQ/L'IMAD, PIF, QIA; managers opening in ADGM/DIFC |
| `perf` | Perf | Performance & flows | Index and peer returns, notable fund numbers, redemptions, prime-book positioning |
| `talent` | Talent | Platforms, PM moves & seeding | Multi-manager hiring, pods, spinouts, seed/acceleration deals |
| `people` | People | IR, capital raising & BD moves | IR, capital formation, client and consultant relations hires/exits |
| `terms` | Terms | Fees, terms & structures | Fees, pass-through, liquidity, share classes, evergreen/semi-liquid |
| `reg` | Rules | Marketing, ops & compliance | AIFMD II, SEC marketing rule, Form PF, FINRA, FCA, FSRA/DFSA, marketing enforcement |
| `events` | Events | Prime, cap intro & events | PB financing and cap intro, conference calendar |
| `acc` | X | From the accounts we follow | Notable posts from SOURCES.md handles |

## Add a brief
1. Copy `template.html` to `briefs/YYYY-MM-DD.html`; fill `{{DATE}}`, `{{DATE_LONG}}` (add " · Weekend edition" on Sundays), `{{HEADLINE}}` (optionally wrap one key figure in `<mark>`).
2. Hero: 4 story cards (copy the S1 article), class from the table above.
3. Fill each `{{..._ITEMS}}` with 2-4 `<li>` bullets, source link inline, one or two sentences, and why it matters to IR/capital raising when not obvious. Empty section: `<li class="empty">Quiet.</li>`. Items older than the window must carry their date.
4. `{{NOTES}}`: window, paywalled or failed sources, unconfirmed items.
5. In `index.html` add under `<!-- ARCHIVE: newest first -->`:
   `<a class="bcard" href="briefs/YYYY-MM-DD.html"><div class="d">DATE_LONG</div><div class="h">HEADLINE</div></a>`
6. No em-dashes. Never invent facts; flag single-source or unconfirmed items. Prefer primary sources; when a scoop is paywalled, cite the reputable write-up and name the original. `git commit` and `git push` to main; check the page returns 200.
