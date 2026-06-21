# Learning & Certification Tracker

A personal, dark-themed web app to track learning and online certifications, presented as a professional portfolio. Static HTML/CSS/JS — no build tools, no server, free to host.

**Live site:** _(GitHub Pages link added after publishing)_

## Features

- 🌌 Galaxy dark theme (Inter font)
- 🗂️ Tabs: **Certifications** (with an **AI** sub-category) and **Projects** (Phase 2 placeholder)
- ✏️ Password-protected **Edit mode** to add / edit / delete certifications (name, link, completion date)
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

## Roadmap (Phase 2)

- About me / work & education sections
- Real Projects content
