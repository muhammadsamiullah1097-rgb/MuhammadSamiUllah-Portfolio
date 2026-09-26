# Muhammad Sami Ullah — Interactive Portfolio

A single-file, interactive portfolio website. No build step, no JS dependencies.

## View it

Open `index.html` directly in any browser (works from `file://` and offline).
For the full experience, serve it or deploy it — the file is self-contained.

## Structure

- `index.html` — the whole site (HTML + CSS + vanilla JS, inline SVG charts)
- `assets/profile.png` — profile photo
- `assets/Muhammad-Sami-Ullah-CV.pdf` — downloadable CV (linked from the header
  Resume button, the hero, and the contact section)

All asset references are **relative** (`assets/...`) so the site works on
GitHub Pages project subpaths (e.g. `username.github.io/repo/`).

## What's inside

- Hero with profile portrait + live interactive data panel (sample data)
- 01 — Pakistan Flood Prediction System (real project, links out to the live
  dashboard and GitHub repo; includes a YouTube demo-URL loader slot)
- 02 — Sales Intelligence Lab (interactive dashboard, deterministic sample data)
- 03 — NLP Sentiment Lab (in-browser lexicon analysis)
- 04 — SQL Explorer (simulated query console)
- 05 — Data Cleaning Lab (before/after)
- 06/07 — Academic projects from the CV (case-study blocks)
- Capabilities (skill chips filter/highlight the projects that demonstrate them),
  Experience & Education, About, Contact (email/phone/GitHub, copy-email button)

Every simulated number is labeled "Interactive demo · sample data". No fake
employers, clients, metrics or testimonials anywhere.

## Editing personal details

All personal links live in one place — the `siteConfig` object at the top of
the inline `<script>` in `index.html`:

```js
const siteConfig = {
  "name": "Muhammad Sami Ullah",
  "email": "muhammadsamiullah1097@gmail.com",
  "phone": "+92 332 1983086",
  "location": "Islamabad, Pakistan",
  "github": "https://github.com/muhammadsamiullah1097-rgb",
  "linkedin": "",                       // empty = LinkedIn button hidden
  "resumeUrl": "assets/Muhammad-Sami-Ullah-CV.pdf",
  "demoVideoUrl": ""                    // paste a YouTube link to embed the demo
};
```

## Deploy on GitHub Pages

1. Create a new repo, push this folder's contents (`index.html`, `assets/`) to
   the `main` branch.
2. Repo Settings → Pages → Deploy from branch → `main` / `/ (root)`.
3. The site is live at `https://<user>.github.io/<repo>/`.
