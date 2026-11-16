# Site notes

Local preview:

```bash
rm -rf _site
bundle exec jekyll serve -l -H localhost
```

Adding a page:

1. Add a file in `_pages/` (see `_pages/conferences.md`).
2. Add it to `_data/navigation.yml` if it should appear in the header.

Changing the social profile:

1. Update the `author:` block in `_config.yml`.
2. Update `_includes/author-profile.html` only if you need a custom label or icon.
3. Put any custom logo in `images/`.

Changing the CV:

1. Replace the PDF in `files/`.
2. Update the link text in `_pages/about.md` and `_includes/author-profile.html` if the filename changes.

`archive/` contains old template pages that are excluded from the build and are kept only for reference.
