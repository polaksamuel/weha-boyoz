# WeHa 07 Boyoz — CLAUDE.md

## What This Is
A fantasy basketball fan site for a 10-person friend group. Live at **weha07boyoz.com**, hosted on GitHub Pages. Sam (polaksamuel) owns the repo, Matt/Mittsy (mmittelmann) is the collaborator doing the rebuild.

## Tech Stack
- Pure HTML / CSS / JS — no framework, no build step
- Firebase Firestore for real-time multiplayer state (Guess Who game)
- Google Fonts: Bebas Neue (display) + Poppins (body)
- GitHub Pages + CNAME (`weha07boyoz.com`)

## Repo Structure
| File | Purpose |
|------|---------|
| `index.html` | Main hub — player cards, quiz, wheel, Hall of Champions, Wingmasters |
| `play.html` | Live multiplayer "Guess Who?" yearbook photo game |
| `admin.html` | Admin panel to control the Guess Who game |
| `starting5jollies.html` | Draft grid / Starting 5 picker |
| `images/players/` | Player avatars and yearbook photos |
| `images/pages/` | Yearbook pages used in Guess Who |

## Design System
Two themes — light is the default, dark is opt-in via `data-theme` attribute.

### Dark mode (`:root`)
```css
--bg: #080b14; --surface: #0f1420; --surface-raised: #141a2e;
--border: rgba(255,255,255,0.08); --ink: #f0f4ff; --muted: #8896b3;
--accent: #f97316; --gold: #fbbf24;
```

### Light mode (`html[data-theme="light"]`)
```css
--bg: #E8C87A; --surface: #FBF3DC; --surface-raised: #F5E8C0;
--border: rgba(0,0,0,0.10); --ink: #0D1117; --muted: #7A4F1A;
--accent: #C8102E; --gold: #B8730A;
```

Light mode uses a wood grain court hero pattern and amber nav with red stripe border-bottom. Theme persists via localStorage (`theme: 'dark'` only saved when user switches away from the default light).

### Typography
- **Bebas Neue** — logo, section headers, stats, scores
- **Poppins 400/600/800** — body, labels, buttons

### Key Rules
- Mobile-first, all layouts via CSS Grid/Flexbox
- Touch targets minimum 44px
- No horizontal overflow on any screen size
- `clamp()` for fluid font sizes
- Nav collapses to hamburger at `< 640px`
- Do not add dark mode changes under `html[data-theme="light"]` — keep them in `:root`

## The 10 Players
| Nickname | Color | Has Avatar |
|----------|-------|-----------|
| Shmoo | `#3b82f6` | — |
| Mittsy | `#22c55e` | `Mr_Mitt.png`, `Mr_Mitt2.png` |
| A-Train | `#f97316` | — |
| Dmac | `#ef4444` | — |
| PJV | `#a855f7` | `PJV.png` |
| Roc | `#06b6d4` | — |
| Sco | `#ec4899` | — |
| Nee | `#84cc16` | — |
| Streim | `#f59e0b` | — |
| Leikin | `#64748b` | `A_Leikin.png` |

"Gunner" appears in the Hall of Champions history data — confirm with Sam whether Gunner = Streim or someone else before adding to the player roster.

## Working Style
- Work one page at a time — finish and review `index.html` before touching other pages
- Always commit working changes before starting a new feature
- Do not redesign `play.html` or `admin.html` until `index.html` is complete and approved
- Commits go under Matt's identity: `Mittsy <matthew.mittelmann@gmail.com>`
- Do not include `Co-Authored-By` lines in commit messages
