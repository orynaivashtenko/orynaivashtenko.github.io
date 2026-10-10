# orynaivashtenko.github.io

Personal academic website of Oryna Ivashtenko, built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme and hosted on GitHub Pages.

## Where things live

- `_pages/about.md` — the front page (biography, photo, selected papers).
- `_bibliography/papers.bib` — the publication list; `selected = {true}` marks papers shown on the front page.
- `_projects/*.md` — research project pages.
- `_pages/cv.md` — the CV page (Markdown); the PDF is in `assets/pdf/`.
- `_data/socials.yml` — contact and profile links (email, ORCID, GitHub, ADS).
- `assets/img/prof_pic.jpg` — the portrait photo.

## How it deploys

Every push to `main` runs the "Deploy site" GitHub Action, which builds the site and pushes the result to the `gh-pages` branch. GitHub Pages serves that branch (Settings → Pages → Branch: `gh-pages`). Do not edit `gh-pages` by hand.

Template documentation: see [`docs/`](docs/).
