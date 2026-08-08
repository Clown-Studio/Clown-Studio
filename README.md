# Clown Studio website

A static website for Clown Studio (Android & web app development), built for free
hosting on GitHub Pages. No build step — plain HTML/CSS.

## What's included
- `index.html` — homepage (about, apps, contact CTA)
- `app-dot-kolam.html` — Dot Kolam app detail page with screenshots
- `privacy-policy.html` — privacy policy template (fill in the bracketed placeholders)
- `contact.html` — contact page template (fill in the bracketed placeholders)
- `assets/` — CSS and images

## 1. Fill in your real details
Before publishing, search each HTML file for square brackets `[...]` and replace with
your real information:
- `contact.html` — business email, support email, registered address, Play Store link
- `privacy-policy.html` — permissions your app uses, any third‑party SDKs/analytics,
  your support email
- `app-dot-kolam.html` — the real Google Play listing URL (currently a placeholder `#`)

## 2. Deploy on GitHub Pages (free)
1. Create a new **public** GitHub repository, e.g. `clown-studio-site`.
2. Upload everything in this folder to the repo root (keep the `assets/` folder structure).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source: Deploy from a branch**, branch **main**, folder **/ (root)**. Save.
5. GitHub will publish the site at:
   `https://<your-username>.github.io/<repo-name>/`
   (takes a minute or two the first time).
6. Optional: add a **custom domain** under Settings → Pages → Custom domain
   (e.g. `clownstudio.com`) if you own one — this looks more professional for
   Play Console verification and lets you use a matching business email address.

## 3. Notes for Google Play Console organisation verification
A few things Play Console commonly checks when verifying an **organisation** account:
- A **live, public website** that clearly represents the business name (this site
  is built to say "Clown Studio" throughout — make sure your legal entity name on
  file matches exactly, including capitalisation, since you're verifying via D-U-N-S).
- A **working privacy policy URL** — use `privacy-policy.html` once deployed
  (e.g. `https://<your-domain>/privacy-policy.html`), and make sure it accurately
  describes what your apps actually collect.
- A **business contact email**, ideally on a domain that matches your website
  (e.g. `you@clownstudio.com` rather than a personal Gmail address). If you don't
  have a custom domain yet, consider getting one — it's often required for the
  business email step of D-U-N-S/organisation verification.
- Consistent business name/address across: Play Console, your D-U-N-S record, and
  this website's Contact page.

This site does not use any paid services — GitHub Pages hosting is free, and if
you skip a custom domain the `github.io` URL is free too. A custom domain (if you
choose to add one) is the only potential cost.
