# Understanding of the website (WIP)

Main local command:
- `rm -rf _site`
- `bundle exec jekyll serve -l -H localhost`

Adding a page:
1. Add a page in _pages (see for example `_pages/conferences.md`)
2. Update: `_data/navigation.yml` (to include new page: starting line: 10)

Changing Social Profile:
1. update in `_config.yml` (top level directory), lines: 78+
2. Update: `_includes/author-profile.md` (lines: 64 etc.)
3. (optional) move logo to: `/images`

Also:
 archive/_pages/markdown.md has some info.