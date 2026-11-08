# Dhanush R. Giriyan — academic website

Personal academic website at [thenush.github.io](https://thenush.github.io), built with Jekyll and hosted on GitHub Pages.

## Updating the site

| Content | File |
| --- | --- |
| Bio, research introduction, and homepage layout | `_layouts/home.html` |
| Blog index and year groups | `_layouts/archive.html` |
| Individual blog posts | `_layouts/post.html` |
| Blog title and description | `menu/blog.md` |
| Personal and Technical category pages | `menu/blog-personal.md`, `menu/blog-technical.md` |
| Post labels | `_includes/blog-labels.html` |
| Publications, paper links, and BibTeX | `_data/publications.yml` |
| Recent visits and news, newest first | `_data/updates.yml` |
| Navigation and profile links | `_data/settings.yml` |
| Name, description, and canonical URL | `_config.yml` |
| CV PDF | `assets/docs/drg_cv.pdf` |
| Profile photo | `assets/img/drg.jpeg` |
| Layout, typography, and responsive styles | `assets/css/academic.css` |

The homepage shows the four most recent updates. The remaining entries are available under **Earlier updates**. Publications and news are data files so routine additions do not require editing the page layout.

List published papers only. An arXiv link may point to a public version of an already published paper.

To add a post, create `_posts/YYYY-MM-DD-post-title.md` with YAML front matter:

```yaml
---
layout: post
title: "Post title"
author: "Dhanush R. Giriyan"
categories: [technical]
tags: [Probability]
---
```

Use `categories: [personal]` for personal writing and `categories: [technical]` for technical posts. Labels appear on the blog index and post header, and the category pages list matching posts automatically. An optional `excerpt` in the front matter controls the index summary.

Add `math: true` to a page or post to enable MathJax. Blog posts remain at their existing URLs. The About and Contact pages are also retained at `/about` and `/contact`.

## Local preview

With Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll. For a production build, run `bundle exec jekyll build`.

GitHub Pages publishes the `gh-pages` branch. Review changes on a separate branch before merging.

## Credits

The site began with [Lagrange](https://github.com/LeNPaul/Lagrange), a Jekyll theme by Paul Le. Its MIT license is preserved in `LICENSE.md`.
