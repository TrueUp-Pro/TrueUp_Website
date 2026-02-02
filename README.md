# TrueUp Website

Jekyll-based site for [TrueUp](https://trueup.com)—expert guidance over video for skilled professionals.

## Local setup

1. Install Ruby (2.7+).
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Serve locally:
   ```bash
   bundle exec jekyll serve
   ```
4. Open [http://localhost:4000](http://localhost:4000).

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. In the repo: **Settings → Pages**.
3. Under "Build and deployment", choose **GitHub Actions** (recommended) or **Deploy from a branch** with branch `main` and folder `/ (root)` or `/docs` depending on how you host.

To use GitHub’s built-in Jekyll build with the `github-pages` gem:

- Add to `Gemfile`: `gem "github-pages", group: :jekyll_plugins`
- In `_config.yml`, uncomment the `plugins` section.
- Run `bundle update` and commit `Gemfile` and `Gemfile.lock`.

## Structure

- `_config.yml` — Jekyll config
- `_layouts/default.html` — Default layout
- `_includes/` — Header, footer
- `index.md` — Home page
- `pricing.md` — Pricing page
- `css/main.css` — Styles
- `assets/images/` — Logo and images

Brand and pricing content are derived from `docs/brand_foundation.md` and `docs/pricing_page.md`.
