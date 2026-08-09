# naterthought.com

Personal website of Nathan Johnson, built with [Hugo](https://gohugo.io/) and
deployed to GitHub Pages by the workflow in `.github/workflows/hugo.yml` on
every push to `master`. The custom domain is set in `CNAME`.

## Where things live

| I want to… | Go to |
|---|---|
| Write a new blog post | `content/posts/<slug>/index.md` (see below) |
| Edit my bio / paper list | `content/about/index.md` |
| Edit the homepage intro | `content/_index.md` |
| Upload a paper PDF | `static/papers/` (linked as `/papers/<file>.pdf`) |
| Upload a site-wide image | `static/img/` (linked as `/img/<file>`) |
| Change colors / styling | `assets/scss/styles.scss` |
| Change page structure | `layouts/` |
| Change nav links, title, metadata | `hugo.toml` |

## Writing a new post

Create a folder under `content/posts/` and put an `index.md` in it:

```
hugo new content/posts/my-new-post/index.md
```

Images that belong to the post go in the same folder and are referenced by
filename (`![caption](figure1.jpg)`). Set `draft = false` when it's ready to
publish. Front matter looks like:

```toml
+++
date = '2026-08-09T12:00:00-07:00'
draft = false
title = 'My New Post'
tags = ['opinion']
+++
```

## Local preview

Requires the *extended* edition of Hugo (for SCSS):

```
hugo server
```

then open http://localhost:1313/. `public/` and `resources/` are build output
and are gitignored — never commit them; the GitHub Action rebuilds from
source on every push.

## Layout overrides

The site uses the [maverick](https://github.com/canhtran/maverick) theme as a
base (git submodule at `themes/maverick`), but everything visible is
overridden by the project-level `layouts/` and `assets/` directories, which
take precedence. To change the design, edit the project files — leave the
submodule alone.

## Comments

Post pages can show comments via [utterances](https://utteranc.es), which
stores them as GitHub issues on this repo. For comment posting to work, the
utterances GitHub App must be installed on this repository (one-time setup at
https://github.com/apps/utterances). Toggle with `params.comments.enabled` in
`hugo.toml`.
