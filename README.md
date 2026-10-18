# Nishchal Bhandari — Portfolio

A responsive black-and-white portfolio using HTML, CSS, and vanilla JavaScript. No framework, installation, or build step required.

## Project structure

- `index.html`: content, navigation, metadata, and links.
- `style.css`: responsive styles, focus states, and reduced-motion support.
- `script.js`: accessible mobile menu and copyright year.
- `assets/profile.jpg`: your original portrait.
- `assets/project-images/`: reserved for future screenshots.

## Run locally

Open `index.html` directly in a browser, use VS Code Live Server, or run `python -m http.server 8000` in this folder and visit http://localhost:8000. Stop the server with Ctrl+C.

## Update the portfolio

Edit content directly in `index.html`. Styling variables are at the top of `style.css`.

Replace `assets/profile.jpg` to change the portrait. Keep its filename or update the HTML path. Adjust `.portrait img` to change the crop.

The supplied PDF has an older CGPA and is deliberately not served. All website references use **9.17**. Add the corrected résumé as **`assets/resume-nishchal.pdf`**. Change both résumé buttons to `href="assets/resume-nishchal.pdf" download`, rename the header button to `Download Resume`, remove its pending aria-label, and update/remove the `resume-status` notice. Until then, the buttons lead to a truthful availability notice.

Project URLs were not supplied. Replace the non-clickable spans inside each `project-links` element with real anchors, for example `<a href="YOUR_VERIFIED_URL" target="_blank" rel="noopener noreferrer">Repository ↗</a>`.

GitHub uses `https://github.com/Nishchal-Bhandari` from the PDF. LinkedIn uses the résumé's shortened URL, `https://bit.ly/3YEJQjD`; replace all occurrences with your direct profile URL if desired. External destinations have not been independently verified.

The five projects with documented descriptions in the résumé are included. Other suggested titles can be added once their descriptions and stacks are supplied. No backend stack is claimed because none is established in the résumé. The contact section uses email without a backend or form.

## Deploy when ready

Nothing has been published and no DNS has been changed.

One option is GitHub Pages:

1. Review content, add the corrected PDF, and fill project URLs.
2. Commit website files to GitHub. `.tmp-tools` and `.qa` are ignored local development tools, not website dependencies.
3. In repository **Settings → Pages**, select **Deploy from a branch**, the publishing branch (usually `main`), and **/(root)**.
4. Save, wait for deployment, and check the generated URL.

### Connect nishchalbhandari.dev

1. Verify domain ownership in GitHub Pages settings.
2. Set `nishchalbhandari.dev` as the repository's custom domain.
3. At your DNS provider, configure apex (`@`) A records using GitHub's current documented values, or a supported ALIAS/ANAME to your Pages hostname.
4. For `www`, create a CNAME pointing to `Nishchal-Bhandari.github.io` after confirming that is your publishing account.
5. Wait for DNS/certificate checks, enable **Enforce HTTPS**, and check both domain variants.

Use [GitHub's current custom-domain instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) for exact DNS values and [domain verification instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages) for ownership verification. Preserve unrelated DNS/email records.

Canonical and Open Graph metadata target `https://nishchalbhandari.dev/`; update them if you choose another domain.

## Checks performed

- Headless Chrome at widths 320, 390, 768, 1024, and 1440: no horizontal overflow, portrait loads, and all internal navigation targets exist.
- Mobile menu opens, closes after selecting a link, and closes with Escape while restoring button focus.
- Desktop and mobile screenshots visually reviewed; portrait sizing corrected.
- JavaScript syntax checked with `node --check`; HTML nesting, unique IDs, local asset paths, required sections, and CGPA checked locally.
- `git diff --check` passed. External profile destinations and hosting/DNS have not been tested.
