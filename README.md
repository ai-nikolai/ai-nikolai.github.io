# nikolairozanov.com

Personal academic website of **Nikolai Rozanov** — CS PhD candidate at Imperial College London, working on LLM agents and reasoning.

Built with [Jekyll](https://jekyllrb.com/) on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) theme (a fork of [Minimal Mistakes](https://mademistakes.com/work/minimal-mistakes-jekyll-theme/)), deployed with GitHub Pages to [nikolairozanov.com](https://nikolairozanov.com).

## Local development

Requirements: Ruby, Bundler, and Node.js (Node is only needed to rebuild `assets/js/main.min.js`).

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

The site is served at <http://localhost:4000>. Configuration changes require restarting the server.

If Ruby dependencies are a problem, Docker works too:

```bash
docker compose up
```

## Content

| Path | Purpose |
|---|---|
| `_pages/about.md` | Homepage / about page |
| `_pages/talks.md` | Academic talks |
| `_pages/conferences.md` | Conference and workshop organisation |
| `_data/navigation.yml` | Header navigation |
| `_config.yml` | Site-wide settings, author profile, analytics |
| `files/` | PDFs (CV, slides, certificates) |
| `images/` | Profile photo, social preview card, favicons, icons |
| `_includes/head/custom.html` | Favicon, social preview, extra `<head>` tags |

Use root-relative links (`{{ site.baseurl }}/files/...`) rather than absolute production URLs so local previews work.

## Deployment

Push to `master`. GitHub Pages builds the site and publishes it to the custom domain configured in `CNAME`.

## Credits

Theme: [Academic Pages](https://github.com/academicpages/academicpages.github.io), based on [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes). Both are MIT licensed; see `LICENSE`.
