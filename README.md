# Learning & Certification Tracker

A personal, dark-themed web app to track learning and online certifications, presented as a professional portfolio. Static HTML/CSS/JS — no build tools, no server, free to host.

**Live site:** https://mimi0320mje.github.io/learning-tracker/

## Features

- 🌌 Galaxy dark theme (Inter font)
- 🗂️ Tabs: **Overview** (Phase 2 placeholder), **Projects**, and **Certifications** (with an **AI** sub-category)
- ✏️ Password-protected **Edit mode** to add / edit / delete:
  - **Certifications** — name, link, completion date
  - **Projects** — name, link, date/year, tech/tools tags, description
- 💾 Edits save instantly in your browser, plus **Export** to publish for everyone
- ✉️ **Contact me** button (email is never shown on the page)

## How to use

Open `index.html` in any browser, or visit the live link.

### Editing your certifications

1. Click **✎ Edit** (top-right) and enter your password.
2. Add, edit, or delete certifications. Changes save in your browser automatically.
3. To make changes appear for **everyone / on all your devices**, click **⬇ Export data.json**, then upload that file to this repo (replace the existing `data.json`). The live site updates within a minute or two.

### Password

- Default password: **Mia666%**
- You can change it in Edit mode (**🔑 Change password**). After changing, **Export & publish data.json** so the new password applies everywhere.
- **Recovery:** `Mia666%` always works as a built-in master key, even after you change the password.
- **Important — this is light protection only.** The page runs entirely in the browser, so the password is not bank-level security; it only keeps casual visitors from editing. The real, strong lock is your **GitHub account** — only you can log in and change the published files. If you ever get locked out, just edit `data.json` (or the password) directly in GitHub.

## Files

- `index.html` — the entire app (theme, tabs, edit UI, password, contact)
- `data.json` — published certification data (and optional custom password hash)
- `README.md`, `.gitignore`

## Roadmap (Phase 2) — Overview tab

Turn the **Overview** placeholder into a personal intro, editable and published just like Projects/Certifications. Planned layout:

1. **About me** — a short headline/role, a 2–4 sentence bio, optional location, and link buttons (LinkedIn, GitHub, etc.).
2. **Work experience** — a timeline of roles: role · company · dates · description.
3. **Education** — a timeline of schools: school · program · dates · description.
4. *(Optional)* **Skills** — small tag pills.

Everything stays password-gated and saves to `data.json` the same way the other tabs do.
