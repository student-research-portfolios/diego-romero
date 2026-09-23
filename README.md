# Diego Romero — Engineering & Research Portfolio

A static portfolio site built with Jekyll and hosted on GitHub Pages.
No build step, no dependencies to maintain and no hosting cost.

**Live site:** https://student-research-portfolios.github.io/diego-romero/

For day-to-day content editing, read [HANDOVER.md](HANDOVER.md) instead of this file.

## Layout

```
_config.yml              Site-wide settings: student name, titles, base URL
index.html               Landing page
_layouts/                Page templates
_projects/               One Markdown file per project — all project content
_data/upcoming.yml       Projects announced but not yet published
assets/css/style.css     The whole design system, driven by CSS custom properties
assets/img/<project>/    Images, one folder per project
```

## How a project page is built

Each file in `_projects/` carries its front matter (title, tags, hero image, buttons) and its body.
The `project` layout renders the hero, the body and the call-to-action buttons.

A button with an empty `url` renders as a disabled "link pending" chip.
Pasting the Zenodo URL into that field turns it into a live link with no other change.

## Publishing

GitHub Pages builds the `main` branch with Jekyll.
Set the source under **Settings → Pages → Build and deployment → Deploy from a branch → main / (root)**.

`baseurl` in `_config.yml` must match the repository name, and all asset paths go through
`| relative_url` so that the site works under that subpath.

## Starting a portfolio for another student

Use this repository as a GitHub template, then change `student_name` and `baseurl` in `_config.yml`
and replace the contents of `_projects/` and `assets/img/`.
Nothing in `_layouts/` or the stylesheet needs to change.
