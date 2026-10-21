# Nicholas Stiles

Personal academic website built with Jekyll and al-folio.

## Editing

- Bio and profile: `_pages/about.md`
- Profile photo: `assets/img/IMG_7828.JPG`
- Site settings: `_config.yml`
- Contact links: `_data/socials.yml`
- Future publications: `_bibliography/papers.bib`
- Future CV: `_data/cv.yml` or `assets/json/resume.json`

The optional content data files are intentionally empty. RenderCV configuration is retained in `assets/rendercv/`; CV rendering and citation updates run only when manually requested in GitHub Actions after adding your own data.

## Preview

With Docker Desktop running, run `docker compose up` and open <http://localhost:8080/>. Stop with Ctrl+C, then run `docker compose down`.

Alternatively, install Ruby and Bundler, run `bundle install`, then `bundle exec jekyll serve --livereload` and open <http://localhost:4000/>.

## Publishing

Commit changes and push to `main`. The Deploy site workflow builds the site and publishes to `gh-pages`. GitHub Pages should serve the root of that branch. Local edits and commits do not publish until pushed.

See [the documentation](docs/README.md) for configuration and feature guides.
