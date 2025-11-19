# final — Personal portfolio site

This repository contains a small personal portfolio site built to satisfy the final project requirements for MI 349.

What's included
- Four valid HTML5 pages: `index.html`, `about.html`, `portfolio.html`, `contact.html`.
- A single external stylesheet at `styles/styles.css`.
- Two project images in `images/` (`photo.svg`, `graphic.svg`) referenced with relative links.
- A `figma/` folder with instructions and placeholders for the brand and prototype.
- `netlify.toml` configured to publish the site root.

Local development
1. Serve the files from a simple static server. For example, using Python 3:

```bash
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

Deployment (GitHub + Netlify)
1. Initialize git and commit the files locally:

```bash
git init
git add .
git commit -m "Initial site commit"
```

2. Create a new GitHub repository and push (you can use the GitHub CLI):

```bash
# create a public repo named 'final'
gh repo create bradylefere/final --public --source=. --remote=origin --push
```

3. Deploy to Netlify
- Option A (recommended): Connect the GitHub repository to Netlify via the Netlify web UI and set the build/publish settings to use the root (no build command needed).
- Option B (CLI): Install the Netlify CLI and run `netlify deploy --prod --dir .` after linking the site.

Figma deliverables
- The course requires a brand and a Figma prototype (minimum 4 pages). Use the `figma/` folder to store exported artboards or a link to your Figma prototype. The included markdown files explain what to export.

Notes and next steps
- Check the pages with an HTML validator to confirm validity.
- Replace placeholder copy and images with your personal content and exported Figma artboards.
