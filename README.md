# hamed-d.github.io

Personal website of Hamed Damirchi, built with [al-folio](https://github.com/alshedivat/al-folio) v1.2 (Jekyll). Its MIT licence is in `LICENSE`.

## Where the content lives

| What | File |
|---|---|
| Home page text, "Recent" list | `_pages/about.md` |
| Projects | `_projects/*.md` (`importance` sets the order, `category` sets the group) |
| Publications | `_bibliography/papers.bib`. Add `selected = {true}` to show a paper on the home page |
| Teaching | `_teachings/*.md` |
| CV | `assets/pdf/hamed-damirchi-cv.pdf`. `data/HamedDamirchi-CV.pdf` is a copy that keeps the old URL working |
| Blog posts | `_posts/YYYY-MM-DD-title.md` (none yet) |
| Contact icons | `_data/socials.yml` |
| Site settings | `_config.yml` |

The CV PDF is built in the separate `overleaf-cv` repository; copy it here, don't edit it.

## Changes from stock al-folio

Keep this list current. It's what to check when upgrading.

- Removed the demo content, the bookshelf, repositories, people, plugins and news pages, and al-folio's own agent and CI files. Only `.github/workflows/deploy.yml` is kept.
- Turned off the RenderCV/JSON Resume CV feature and Distill posts in `_config.yml` (`al_folio.features`). The CV page (`_pages/cv.md`) is a plain page that shows the PDF.
- `_includes/footer.liquid` overrides the gem's footer to show contact icons on every page.
- `_pages/blog.md` shows "No posts yet." when there are no posts, and is last in the menu.
- `enable_navbar_social: true`, publication badges off, and all authors shown (`max_author_limit` blank).
- `figs/` holds interactive plots from the old site, kept at the same URLs in case they are linked elsewhere.

## Preview locally

With Docker: `docker compose up`, then open <http://localhost:8080>.

Without Docker, you need Ruby 3.3, Bundler and ImageMagick: `bundle install`, then `bundle exec jekyll serve`.

## Deploying

`.github/workflows/deploy.yml` builds the site on every push to `master` and publishes the result to the `gh-pages` branch. In the repository settings, under Pages, the source must be "Deploy from a branch: gh-pages / (root)".
