# Elyas Saif — personal academic website

A buildless HTML/CSS site for GitHub Pages. No package installation, JavaScript, or external font service is needed. The biography includes the approved teaching wording; the supplied paper abstract is preserved verbatim.

## Repository and website

Repository: https://github.com/simco177/ElyasSaif
Website: https://simco177.github.io/ElyasSaif/

Elyas authorized the initial GitHub push and publication on 10 November 2026. Future additions can be reviewed locally and pushed separately when requested. All asset links are relative to support the project URL.

## Preview

Open index.html directly in a browser, or from this directory run:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Then visit http://127.0.0.1:8765/. Stop the server with Ctrl+C.

## Add a CV or paper

1. Copy the final CV to `assets/cv.pdf` or paper to `assets/job-market-paper.pdf`.
2. In `index.html`, find the corresponding `document-status` paragraph.
3. Replace that paragraph with the ready-to-use anchor in the HTML comment immediately above it.
4. Preview the link, then commit the files and HTML together.

The PDF anchors open a new browser tab without forcing download. Whether a browser displays or downloads a PDF also depends on the visitor's browser settings. Until actual PDFs are supplied, the page shows honest non-clickable statuses instead of broken links.

## Add a portrait

Copy the chosen image to `assets/portrait.jpg`. Replace the `portrait-placeholder` div with the img element provided in the nearby HTML comment. The frame uses a 4:5 crop; adjust object-position in styles.css if needed.

## Future additions

Edit text in index.html and design in styles.css. Add research entries inside the research section or a new section before the closing main tag. Add matching navigation links if useful. Use relative file URLs, e.g. `assets/new-paper.pdf`, rather than `/assets/new-paper.pdf`, so links work under `/ElyasSaif/`.

## Publishing updates

GitHub Pages serves the root of the `codex/personal-website` branch. Commit reviewed changes and push that branch to publish an update. No workflow file or build step is required.

A commit records a local snapshot. A push transfers commits to GitHub. Deployment publishes the website. GitHub Pages hosting from a public repository is free; a custom domain is optional and separately registered.

Documentation: https://docs.github.com/en/pages/quickstart
