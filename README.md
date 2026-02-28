# ExoRNA Project Website

**Exosomal circular RNA Biomarkers for Early Detection and Prognosis of Pancreatic Cancer**

A redesigned, premium multi-page static website for the ExoRNA research project — ready to deploy on GitHub Pages.

---

## Files

| File | Description |
|---|---|
| `index.html` | Project overview — background, aims, outcomes, literature |
| `phases.html` | 5-phase interactive timeline with week-by-week breakdown |
| `methods.html` | 11-step pipeline with connected visual layout and figure plan |
| `team.html` | Tabbed page: team, Google Calendar, Google Docs, meeting format |
| `style.css` | Shared design system (light editorial aesthetic) |
| `main.js` | Shared script: custom cursor, nav scroll, reveal animations |

---

## Deploy to GitHub Pages

1. Create a repo named `YOUR-USERNAME.github.io` (or any repo)
2. Upload all 6 files to the repo **root**
3. Go to **Settings → Pages → Source → main branch / (root)**
4. Site goes live at `https://YOUR-USERNAME.github.io` within minutes

---

## Customise the Team Page

### Add a Team Member
In `team.html` → `#tab-people`, copy any `.team-card` block and update the initials, name, role, and bio.

### Embed Google Calendar
1. Google Calendar → Settings → Your calendar → **Integrate calendar** → copy embed code
2. In `team.html`, find the `embed-frame` with the calendar comment
3. Replace the `<div class="embed-body">` block with: `<iframe src="YOUR_EMBED_URL" class="live-embed" frameborder="0" scrolling="no"></iframe>`

### Embed Google Doc
1. Google Doc → **File → Share → Publish to web → Embed tab** → copy iframe
2. Replace the first `<div class="embed-body">` in the docs tab with your iframe (add `class="live-embed"`)

### Embed Google Sheets
Use src: `https://docs.google.com/spreadsheets/d/YOUR_SHEET_ID/pubhtml?widget=true&headers=false`

### Embed Google Drive Folder
Use src: `https://drive.google.com/embeddedfolderview?id=YOUR_FOLDER_ID#list`

### Update Quick Access Links
In `team.html` → find `.quick-links` → update the `href` values on each `.qlink` anchor.

---

## Design Notes

- **Typography**: Playfair Display (headings) + Plus Jakarta Sans (body) + JetBrains Mono (labels)
- **Theme**: Premium light — off-white paper background, deep navy ink, emerald accent
- **Features**: Custom cursor, scroll reveal animations, nav scroll shadow, phase switcher (phases page), tabbed interface (team page)
- **No build tools** — pure HTML, CSS, and vanilla JS
- **Mobile responsive** — stacks to single column below 900px
