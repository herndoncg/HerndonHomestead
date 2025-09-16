# Herndon Homestead – Static Site

This folder contains the fully linked, deploy‑ready static HTML for **Herndon Homestead**.

## Structure
```
.
├── index.html
├── about.html
├── subbrands.html
├── herndough.html
├── harvest.html
├── table.html
├── recipes.html
├── blog.html
├── contact.html
├── support.html
├── shop.html
├── privacy.html
└── terms.html
```

> Note: A global external font (Inter via Google Fonts) is referenced inside each page’s `<head>`.
> Headings fall back to Georgia/Times; body falls back to Arial/Helvetica if Inter is unavailable.

## What Was Normalized
- **Links:** All navigation/footer links are **relative** (e.g., `about.html`), not root‑absolute (`/about.html`).
- **Sub‑Brands URL:** Standardized to `subbrands.html` (no hyphen). Any prior `sub-brands.html` references were fixed.
- **Legal Pages:** Added simple placeholders for `privacy.html` and `terms.html` to satisfy footer links.
- **No JS build or bundler required:** This is plain HTML/CSS and will deploy on Netlify/GitHub Pages as‑is.

## Deploying

### GitHub Pages
1. Create a repo (e.g., `HerndonHomestead`).
2. Upload all files at the repo root and push.
3. Enable Pages (Settings → Pages → deploy from `main` / root).

### Netlify
1. Drag & drop this folder into Netlify **or** connect your GitHub repo.
2. No build command needed; publish directory is the repo root.
3. Netlify will assign a URL like `https://herndonhomestead.netlify.app/`.

## Local Preview
Open `index.html` in a browser. All links are relative so navigation works locally.

---

If you add images or a shared CSS later, place them under an `/assets/` folder and reference them with `assets/...` relative paths.
