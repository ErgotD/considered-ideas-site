# CLAUDE.md

Project working brief for Claude Code.

## What this project is

The static front-door website for **Considered Ideas Ltd** at `consideredideas.com`. A small calm one-page company presence used for Apple Developer review, legal footer requirements, and a contact entry point for both products and consultancy. Sibling to the `in-the-retelling-support` repo; shared editorial voice and a shared warm-paper-and-persimmon palette, but Considered Ideas has its own mark and may evolve its own typographic and layout decisions independently as the parent brand develops.

## How to work in this repo

Plan before acting. Editorial changes are typically small and low risk, but copy on a company-facing site should still be reviewed before publication; the owner will say "go ahead" before non-trivial edits are committed.

Make small coherent slices. One section at a time. Keep the page as one HTML file unless and until a second page is genuinely required.

When in doubt, ask. The editorial voice on this site has to read as a sibling to the In the Retelling support site; if anything feels off in tone, surface it rather than guess. Visual decisions can diverge from the support site as the Considered Ideas brand grows.

## Editorial rules (non-negotiable)

UK English throughout. "Favourites" not "favorites", "behaviour" not "behavior", "centre" not "center", and so on.

Prose first. Avoid heavy bullet lists in copy unless the content is genuinely a list. Whole sentences over fragments.

No em dashes anywhere, in HTML, in CSS comments, or in any document. Use sentence-level rephrasing instead.

Avoid the words "honestly", "genuinely", and "straightforward" in any prose.

No emoji. Not in copy, not in comments.

No motivational, gamified, or startup-marketing language. No claims like "transforming X" or "the future of Y". The brand voice is calm, grown-up, and observational, matching the bedside-book voice used in the In the Retelling product.

## Visual rules

Warm paper background, persimmon accent only in small details, Newsreader serif for the wordmark and headings, Inter or system sans for the body if and where sans is needed. No textures, no gradients, no atmospheric photography, no stock images of people, mountains, or hands. No cards, drop shadows, or dashboard layouts.

The Considered Ideas brand mark is the petal-plus-dot vesica: a vesica piscis lens filled in persimmon, with a small persimmon dot baseline-aligned to the petal's foot. It appears inline as an SVG before the h1 in the hero, and as the favicon set (SVG primary, PNG fallbacks, multi-res ICO for older browsers). The mark stays in persimmon on cream paper; do not flood persimmon as a background and do not introduce a second accent colour.

The two sites share the warm-paper-and-persimmon palette and the Newsreader-and-Inter typographic stack, but the In the Retelling support site uses a simple persimmon disc as its mark (mirroring the app icon) while Considered Ideas uses the petal-plus-dot. The marks are siblings, not the same.

## Locked content constraints

- The legal footer must carry the registered name (`Considered Ideas Ltd`), the registered office address, and the Companies House number. These are required for a publicly trading UK Ltd.
- The contact email is `enquiries@consideredideas.com`. No other public-facing email is named on the site.
- Products are linked, not described in marketing detail. The product page lives on its own site (e.g. the in-the-retelling-support repo). The company site lists products and links out.
- The consultancy section is intentionally minimal: a holding paragraph until there is a specific offer to describe.

## File map

```
considered-ideas-site/
  CLAUDE.md              (this file)
  README.md              project overview and publish workflow
  index.html             one-page front door
  styles.css             warm-paper-and-persimmon styles; self-hosted @font-face block at top
  favicon.svg            tight-viewBox petal-plus-dot mark in persimmon (primary modern favicon)
  favicon.ico            multi-resolution fallback (16, 32, 48)
  favicon-16.png         PNG favicons for browsers that prefer per-size links
  favicon-32.png
  favicon-48.png
  apple-touch-icon.png   180x180 iOS home-screen icon
  icon-192.png           PWA icons (currently unwired; available if a manifest is added later)
  icon-512.png
  fonts/                 self-hosted Newsreader and Inter WOFF2, with OFL.txt
  images/                in-page imagery (app shots and similar)
  CNAME                  GitHub Pages custom-domain pointer
  .gitignore
```

## End-of-session checklist

Before declaring a session done:

1. No unresolved TODOs in `index.html` other than the legal-footer placeholders, which stay until the registered office address and Companies House number are confirmed.
2. The page validates as a plain static document and makes no third-party network requests at load time (no JavaScript dependencies, no external CSS, no CDN-loaded fonts; the brand serif and sans are self-hosted under `fonts/`).
3. No personal data (home address, personal phone, personal email) is present anywhere in the repo.
4. No emoji, no em dashes, no banned words in any copy or comment.
