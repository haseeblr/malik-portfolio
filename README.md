# Abdul Malik — portfolio

Static site. No build step, no server, no dependencies.

## Files
- `index.html` — the portfolio (single self-contained file)
- `resume.html` — the résumé page linked from the "Résumé" buttons (visitors can print it to PDF)
- `robots.txt`

## Run locally
Open `index.html` in a browser, or serve the folder:

    npx serve .        # or: python3 -m http.server 8080

## Deploy (pick one)
- **Netlify:** drag this folder onto app.netlify.com/drop.
- **Vercel:** `npx vercel` inside this folder, framework preset "Other", no build command.
- **GitHub Pages:** push these files to a repo, Settings → Pages → deploy from branch, root folder.
- **Render:** New → Static Site, publish directory `.`, no build command.

## Updating content
Content and design are edited in the source project (`Abdul Malik Portfolio.dc.html`, `Abdul Malik Resume.dc.html`), then re-exported to `index.html` / `resume.html`.

## Use a PDF résumé instead
Save `resume.html` as PDF (browser Print → Save as PDF, A4), put it here as `resume.pdf`, and set the portfolio's `resumeUrl` to `resume.pdf` before re-exporting.

## After you have a domain
Add `<link rel="canonical">`, `og:url` and `og:image` in the portfolio head, and a `sitemap.xml` listing the URL.
