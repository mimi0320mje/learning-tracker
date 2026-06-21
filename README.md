# Learning & Certification Tracker

A personal, dark-themed web app to track learning and online certifications, presented as a professional portfolio. Static HTML/CSS/JS hosted free on GitHub Pages, with a free Firebase (Firestore) backend so edits go live everywhere in real time.

**Live site:** https://mimi0320mje.github.io/learning-tracker/

## Features

- 🌌 Galaxy dark theme (Inter font)
- 🗂️ Tabs: **Overview** (Phase 2 placeholder), **Projects**, and **Certifications** (with an **AI** sub-category)
- ✏️ Password-protected **Edit mode** to add / edit / delete:
  - **Certifications** — name, link, completion date
  - **Projects** — name, link, date/year, tech/tools tags, description
- ☁️ Edits save to the cloud and appear **instantly for every visitor and on every device** — no manual publishing
- ✉️ **Contact me** button (email is never shown on the page)

## How to use

Visit the live link (or open `index.html`).

### Editing

1. Click **✎ Edit** (top-right) and enter your password.
2. Add, edit, or delete certifications and projects.
3. That's it — each change saves to the cloud and is **live everywhere immediately**. (Click **✓ Done** to lock editing again.)

The **⬇ Backup** button downloads a copy of your data as a safety net (optional).

### Password & security

- Default password: **Mia666%**
- Change it anytime in Edit mode (**🔑 Change password**).
- **Anyone can view** the portfolio, but **only you can edit** it (enforced by Firebase Auth + Firestore security rules — your email is the only account allowed to write).
- **Forgot your password?** Reset it from the Firebase console (Authentication → Users) at https://console.firebase.google.com.

## How it's wired (for future reference)

- **Backend:** Firebase project `learning-tracker-944f8` (free Spark tier).
- **Data:** Firestore collection `portfolio`, single document `data` → `{ certifications, projects }`. The page subscribes with `onSnapshot` for real-time updates.
- **Auth:** Firebase Email/Password. One editor account (`miachen1155665@gmail.com`); the password box signs into it behind the scenes.
- **Security rule:** public read; write only when signed in as the editor email.
- **Authorized domain** in Firebase Auth settings: `mimi0320mje.github.io`.
- `data.json` is now only a fallback seed used before the cloud document exists.

## Files

- `index.html` — the entire app (theme, tabs, edit UI, Firebase wiring, contact)
- `data.json` — fallback seed data (cloud is the live source of truth)
- `README.md`, `.gitignore`

## Roadmap (Phase 2) — Overview tab

Turn the **Overview** placeholder into a personal intro, editable and published just like Projects/Certifications. Planned layout:

1. **About me** — a short headline/role, a 2–4 sentence bio, optional location, and link buttons (LinkedIn, GitHub, etc.).
2. **Work experience** — a timeline of roles: role · company · dates · description.
3. **Education** — a timeline of schools: school · program · dates · description.
4. *(Optional)* **Skills** — small tag pills.

Everything stays password-gated and saves to the cloud (Firestore) the same way the other tabs do.
