# esmailoghli.github.io

My personal website. Plain HTML + CSS — **no build step, no JavaScript, no frameworks.**
Just two files you can edit by hand: `index.html` (content) and `style.css` (look).

## Files

```
index.html        all the page content
style.css         all the styling (colors/width live in the variables at the top)
assets/mahdi.jpg  your profile photo (a square headshot crops best)
.nojekyll         tells GitHub Pages to serve files as-is (no Jekyll build)
```

## Preview locally

Just open `index.html` in a browser. Or, for a closer match to production:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## How to edit

- **Add a publication** — in `index.html`, copy one `<li class="pub">…</li>` block,
  paste it at the top of the list, edit the title/authors/venue. Wrap your own name in
  `<strong>…</strong>`.
- **Add a news item** — copy one `<li>` in the News list, change the date and text.
- **Change colors or width** — edit the variables at the top of `style.css`
  (`--accent`, `--text`, `--maxw`, …). There's a dark-mode block right below; delete it
  if you don't want a dark version.
- **Replace the photo** — swap in your own `assets/mahdi.jpg` (a square headshot crops best).
- **Fill in the profile links** — replace the `href="#"` placeholders (Google Scholar,
  DBLP, LinkedIn) in the intro with your real URLs.

## Deploy to GitHub Pages

The repo is `esmailoghli/esmailoghli.github.io`, so it publishes to
`https://esmailoghli.github.io`.

```bash
git add .
git commit -m "Update site"
git push
```

In **Settings → Pages**, set **Source → Deploy from a branch → `master` (or `main`) / root**.
Because `.nojekyll` is present, Pages serves the files directly — there is no build to fail.
Changes go live within a minute or two.
