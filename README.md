# Wildbrook Beverage Burros — Coming Soon

A single-page holding site for [wildbrookbeverageburros.com](https://wildbrookbeverageburros.com),
live while the full site is in development. Shares brand tokens (color, type)
with the main site build at
[vibe89slc/wildbrook-bevvy-burros](https://github.com/vibe89slc/wildbrook-bevvy-burros).

Built by [VIBE89](https://vibe89.com).

## Stack

Vanilla HTML/CSS, no build step, no dependencies.

```bash
python3 -m http.server 8096
# then open http://localhost:8096
```

## Deploy

Hosted on Cloudflare Pages, connected to this repo, with
`wildbrookbeverageburros.com` attached as the custom domain in the Cloudflare
dashboard. Framework preset: **None** — build command empty, output
directory `/`.

## Content notes

- Text CTA number: (206) 334-1495
- Photos in `images/` are stock/demo photography, not the client's actual
  herd or event photos — each is labeled "Example photo" on the page.
  Swap in real photography as it becomes available and drop the labels.
- Event blurb (Sept 8 fundraiser, North Bend) should be double-checked with
  the client for the exact venue/lodge name once confirmed, and updated
  if the date or details change.
