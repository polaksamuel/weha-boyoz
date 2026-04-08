# WeHa 07 Boyoz — To Do

Work through these in order. Check off items as they're completed.

---

## ✅ Done

- [x] Full visual redesign of index.html — basketball theme, dark mode
- [x] All 10 player colors and design tokens
- [x] Nav with hamburger mobile menu
- [x] Basketball court grid pattern in hero
- [x] "The League" section with all 10 player cards
- [x] Quiz redesigned — stacked buttons, progress indicator, animated result
- [x] Spin wheel built as real SVG pie chart
- [x] Hall of Champions restored and redesigned as season cards
- [x] Wingmasters table properly styled
- [x] Firebase debug banner removed
- [x] Firebase SDK standardized to 10.12.4
- [x] Mobile-responsive breakpoints throughout
- [x] Corrected full league history 2014–2026 (13 seasons)
- [x] players.json created with real name ↔ nickname mapping
- [x] PROJECT_BRIEF.md written

---

## 🔥 Immediate (finish before pushing live)

- [ ] Execute light mode — basketball court hardwood maple theme, NBA red
      accent, toggle button in nav persisted via localStorage
- [ ] Confirm images/players/ folder has correct files — Mr_Mitt.png,
      PJV.png, A_Leikin.png, Mr_Mitt2.png
- [ ] Fix "Atrain" → "A-Train" display name in PLAYERS array
- [ ] Update HISTORY array with corrected 2014–2026 data and team names
- [ ] Update players.json with full real name ↔ nickname mapping
- [ ] Open site in browser — full visual QA on mobile and desktop
- [ ] Commit all changes and push to GitHub

---

## 🎨 Design Polish (index.html)

- [ ] Update quiz questions to reference all 10 players
- [ ] Player-specific hover colors on quiz answer buttons
- [ ] Expand spin wheel from 3 players to all 10
- [ ] Review and sign off on mobile layout on a real phone

---

## 📄 Other Pages (after index.html is approved)

- [ ] play.html — design critique, then apply new design system
- [ ] admin.html — apply new design system
- [ ] starting5jollies.html — apply new design system, review content

---

## 📊 ESPN Data Integration

- [ ] TIER 1: Get team names for early seasons (2014–2020) from Sam or
      ESPN history and add to HISTORY array
- [ ] TIER 1: Update index.html to read player data from players.json
      instead of hardcoded PLAYERS array
- [ ] TIER 2: Write Python fetch script (fetch_espn.py) using
      cwendt94/espn-api — outputs league-data.json with full season history
- [ ] TIER 2: Update index.html to read HISTORY from league-data.json
- [ ] TIER 2: Document how to get ESPN_S2 and SWID cookies and run the
      fetch script (add to PROJECT_BRIEF.md)
- [ ] TIER 3: GitHub Action to auto-run fetch script and commit updated
      league-data.json on a schedule

---

## ✨ New Features (future)

- [ ] Regular season winner per year (separate from playoff champion)
- [ ] Team name at time of win shown on champion cards (already partially done)
- [ ] Season-by-season team name history — tooltip or dedicated page
- [ ] Current season standings / live leaderboard on homepage
- [ ] Player profile pages — stats, titles, team name history, photo
- [ ] Hall of Wingmasters — fill in real data (get from Sam/group)
- [ ] Review Guess Who gameplay — improve flow if needed
- [ ] Season recap / news section for trash talk and highlights

---

## ⚙️ Project Hygiene

- [ ] Finish setting up Claude Project in Cowork with PROJECT_BRIEF.md
- [ ] Keep TODO.md and PROJECT_BRIEF.md updated each session
- [ ] Confirm Nee and Streim are correctly mapped (ask Sam to verify)
