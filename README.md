# Nicole Walker — Portfolio Site

A single-page portfolio website. No build step, no frameworks: everything lives in `index.html`.

## Editing the site

Open `index.html` in any text editor.

- **To change words, numbers, projects or roles:** find the block that starts with `const CONTENT = {` near the bottom of the file. Every section of the page is listed there, top to bottom (hero, stats, about, case studies, how I work, sample plans, AI, experience, toolkit, contact). Edit the text between the quotes and save.
- **To change colors or fonts:** find the `THEME` block at the very top of the `<style>` section. Change a color there and it updates everywhere.
- **Don't edit below the `RENDERING` comment** unless you're changing layout. That code builds the page from `CONTENT`.

Tip: keep quotes and commas intact when editing `CONTENT`. If the page goes blank after an edit, a missing quote or comma is almost always the cause.

## Previewing locally

Double-click `index.html` to open it in your browser.

## Hosting

The site is hosted with GitHub Pages from the `main` branch (root folder). Every push to `main` updates the live site within a minute or two.

The `.nojekyll` file tells GitHub Pages to serve the files as-is.

### Adding a custom domain later

1. Buy the domain (Namecheap, Squarespace Domains, Cloudflare, etc.).
2. In the repo on GitHub: **Settings → Pages → Custom domain**, enter the domain and save. This creates a `CNAME` file in the repo.
3. At your domain registrar, add the DNS records GitHub shows you (four `A` records for the root domain, plus a `CNAME` record for `www` pointing to `<username>.github.io`).
4. Once DNS is verified, tick **Enforce HTTPS**.
