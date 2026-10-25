# zahidasghar.com — Quarto Website

This is the source for [zahidasghar.com](https://zahidasghar.com), built with [Quarto](https://quarto.org/).

## Quick start

1. Open this folder (`quarto-site-files/quarto-site/`) in Positron or RStudio.
2. Preview while editing: `quarto preview`
3. Render the whole site: `quarto render` (output goes to `docs/` inside this folder).
4. GitHub Pages serves the **repo-root** `docs/` folder, so copy the render there and push:

```bash
# from the repo root
rm -rf docs && cp -r quarto-site-files/quarto-site/docs docs
git add -A && git commit -m "Update site" && git push
```

`CNAME` is listed under `project: resources`, so the custom domain file is kept on every render.

## Brand and theme

- `_brand.yml` holds the palette and fonts (dark green `#2C5F2D`, muted brown `#8B7355`;
  Source Serif 4 for headings, standing in for Georgia; Cabin for text, standing in for Gill Sans MT).
  You can copy it into any other Quarto project to get the same look.
- `custom.scss` holds the layout rules (letterhead navbar, hero, ledger lists, footer).
- The homepage (`index.qmd`) is written in HTML blocks so the layout stays exact; edit the text directly there.

## Images

- `images/profile.jpg` (800x1000) and `images/profile-sm.jpg`: hero portrait
- `images/avatar.jpg`: square portrait used on the About page
- `images/og-card.jpg`: 1200x630 card shown when the site is shared on LinkedIn, WhatsApp or X
- `images/favicon.svg`: "ZA" monogram

## Adding a blog post

Create `posts/my-post/index.qmd` with `title`, `description`, `date` and `categories` in the YAML header,
then render. The Blog page and the RSS feed (`blog.xml`) update automatically.
