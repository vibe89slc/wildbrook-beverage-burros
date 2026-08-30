# Wildbrook Beverage Burros, Coming Soon

A single-page holding site for [wildbrookbeverageburros.com](https://wildbrookbeverageburros.com),
live while the full site is in development. Shares the brand's real logo and
type family with the main site build at
[vibe89slc/wildbrook-bevvy-burros](https://github.com/vibe89slc/wildbrook-bevvy-burros),
but runs its own darker, higher-contrast palette (see Design notes below).

Built by [VIBE89](https://vibe89.com).

## Stack

Vanilla HTML/CSS/JS, no build step, no dependencies. The gallery carousel and
scroll reveals are native (CSS scroll-snap + `IntersectionObserver`), no
animation library.

```bash
python3 -m http.server 8096
# then open http://localhost:8096
```

## Deploy

Hosted on Cloudflare Pages, connected to this repo, with
`wildbrookbeverageburros.com` attached as the custom domain in the Cloudflare
dashboard. Framework preset: None. Build command empty, output directory `/`.

## Design notes

Built against `.claude/skills/taste-skill` (installed at the workspace root)
for the "amp it up to luxury" pass. Deliberate choices worth knowing before
editing:

- **Palette:** a "Forest" system (deep near-black forest green, bone, one
  amber accent), not the beige and cream and terracotta and brass combo used
  on the main site render. That combo is explicitly the AI-default premium
  palette the skill flags as overused; this page rotates away from it while
  staying in the same brand hue family.
- **Type:** kept Fraunces and Inter on purpose, even though the skill
  discourages both as defaults. They are the client's real, already-live
  brand type on the main site, so matching them here is a brand-consistency
  call, not a default pick.
- **Zero em-dashes** anywhere in visible page copy, per the skill's
  non-negotiable rule. Keep it that way in future copy edits.
- **One CTA label** ("Text (206) 334-1495", "Text us" only in tight spaces)
  used everywhere on the page, one accent color (amber), one corner-radius
  system (pill buttons, 20px soft image corners, 6px utility tags).
- The event section's background logo is a deboss effect (`.event__watermark`
  in styles.css), two offset copies of the same fine-line mask, not a flat
  watermark image.

## Content notes

- Text CTA number: (206) 334-1495.
- Photos in `images/` are stock and demo photography, not the client's
  actual herd or event photos. Each is labeled "Example photo" on the page.
  Swap in real photography as it becomes available and drop the labels.
  `wildbrook-bevvy-burros/images/scene-detail.jpg` was deliberately excluded
  from this project, it carries a visible `@milagroranch_tx` watermark from
  a real, different ranch business and should not be used anywhere on either
  site.
- Event blurb (Sept 8 fundraiser, North Bend) should be double-checked with
  the client for the exact venue and lodge name once confirmed, and updated
  if the date or details change.
