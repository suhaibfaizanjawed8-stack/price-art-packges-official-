# Printside Packaging — GitHub-ready website

**Important:** This project is a **reconstruction**, not extracted source code from the Meta AI shared artifact. The Meta AI public share displayed a filename but did not provide downloadable HTML/source files at the time this package was assembled.

## Files

- `index.html` — homepage
- `about.html` — company overview
- `products.html` — filterable product catalogue
- `capabilities.html` — service workflow
- `quality.html` — quality approach
- `innovation.html` — innovation themes
- `industries.html` — market segments
- `contact.html` — editable email-draft inquiry form
- `css/style.css` — all styling and mobile responsiveness
- `js/main.js` — mobile navigation, filtering, inquiry form
- `assets/` — original, locally hosted SVG illustrations, logo and favicon
- `vercel.json` — Vercel configuration

## View locally

Open `index.html` in a browser. Navigation and product filtering work without a build process or a server. All assets are local: **no image host, framework, CDN or API key is required**.

## Before you publish

1. Change the placeholder brand name and all demo marketing copy as needed.
2. Enter your verified business phone, email, office address, production details and certifications. The demo deliberately makes no unverified compliance or certification claims.
3. In `js/main.js`, change `CONTACT_EMAIL = 'REPLACE_WITH_YOUR_EMAIL'` to your business email. The form uses `mailto:`; it **does not send mail in the background**. For a true web form, connect your own secure server-side form endpoint.
4. Replace the sample SVG illustrations with approved brand photography or commissioned images if you need photorealistic factory imagery.

## Publish to your existing empty repository

Use a terminal **inside the extracted `PAP-official` folder**:

```bash
git init
git add .
git commit -m "Add Printside Packaging website"
git branch -M main
git remote add origin https://github.com/suhaibfaizanjawed8-stack/PAP-official.git
git push -u origin main
```

**If Git was already initialised and `origin` already exists**, do not add it again; run:

```bash
git remote set-url origin https://github.com/suhaibfaizanjawed8-stack/PAP-official.git
git add .
git commit -m "Add Printside Packaging website"
git push -u origin main
```

If nothing changed, Git may correctly report that there is nothing to commit.

## Publish using Vercel

1. Import the `PAP-official` repository into Vercel.
2. Framework preset: `Other`.
3. Root Directory: project root (the folder containing `index.html`).
4. Build command: leave blank.
5. Output Directory: leave blank (Vercel serves the static files).
6. Deploy and test every navigation link, especially `about.html`, `products.html` and `contact.html`.

The HTML links are all **relative URLs**, so the same files work locally, on Vercel and with GitHub Pages.
