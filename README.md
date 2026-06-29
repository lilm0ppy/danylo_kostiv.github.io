# Danylo Kostiv — Portfolio

Static site. No build step. Open `index.html` in a browser, or host the folder anywhere.

## Files
- `index.html` — portfolio homepage (entry point)
- `case-study.html` — SPIFF Module case study
- `support.js` — rendering runtime (loaded by both pages; do not edit)
- `assets/` — images and résumé PDF
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Editing content
Copy and headings live directly in `index.html` and `case-study.html`. The text and
data (work history, skills, hardware list, etc.) are near the bottom of each file inside
the `<script ... data-dc-script>` block — edit the strings there and save.

> The pages load React from a public CDN (unpkg) at runtime, so the site needs an
> internet connection to render. GitHub Pages provides this automatically.

## Deploy to GitHub Pages
1. Create a new GitHub repository.
2. Upload the **contents** of this folder to the repository root
   (so `index.html` sits at the top level), then commit.
3. In the repo: **Settings → Pages**.
4. Under **Build and deployment**, set **Source = Deploy from a branch**,
   pick your branch (e.g. `main`) and folder **`/ (root)`**, then **Save**.
5. Wait ~1 minute. Your site goes live at
   `https://<your-username>.github.io/<repo-name>/`.

To use a custom domain later, add it under Settings → Pages → Custom domain.
