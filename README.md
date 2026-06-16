# esmailoghli.github.io

My personal website. Plain HTML + CSS — no build step, no JavaScript, no frameworks.

> **This is my personal site.** The source lives in this repo only because GitHub Pages
> serves from it. It is **not** a template — please don't copy, reuse, or modify it.
> © Mahdi Esmailoghli. All rights reserved.

## Files

```
index.html        all the page content
style.css         all the styling (colors/width live in the variables at the top)
assets/mahdi.jpg  profile photo
.nojekyll         tells GitHub Pages to serve files as-is (no Jekyll build)
```

## Preview locally

Open `index.html` in a browser. Or, for a closer match to production:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy

The repo is `esmailoghli/esmailoghli.github.io`, so it publishes to
`https://esmailoghli.github.io`. Pushing to `master` deploys; because `.nojekyll`
is present, Pages serves the files directly and changes go live within a minute or two.
