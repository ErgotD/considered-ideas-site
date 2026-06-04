# CLAUDE.md

Project working brief for Claude Code.

## What this project is

The static front-door website for **Considered Ideas Ltd** at `consideredideas.com`. A small calm one-page company presence used for Apple Developer review, legal footer requirements, and a contact entry point for both products and consultancy. Sibling to the `in-the-retelling-support` repo; identical visual language, identical editorial voice.

## How to work in this repo

Plan before acting. Editorial changes are typically small and low risk, but copy on a company-facing site should still be reviewed before publication; the owner will say "go ahead" before non-trivial edits are committed.

Make small coherent slices. One section at a time. Keep the page as one HTML file unless and until a second page is genuinely required.

When in doubt, ask. The brand voice on this site has to read as a sibling to the In the Retelling support site; if anything feels off, surface it rather than guess.

## Editorial rules (non-negotiable)

UK English throughout. "Favourites" not "favorites", "behaviour" not "behavior", "centre" not "center", and so on.

Prose first. Avoid heavy bullet lists in copy unless the content is genuinely a list. Whole sentences over fragments.

No em dashes anywhere, in HTML, in CSS comments, or in any document. Use sentence-level rephrasing instead.

Avoid the words "honestly", "genuinely", and "straightforward" in any prose.

No emoji. Not in copy, not in comments.

No motivational, gamified, or startup-marketing language. No claims like "transforming X" or "the future of Y". The brand voice is calm, grown-up, and observational, matching the bedside-book voice used in the In the Retelling product.

## Visual rules

Warm paper background, persimmon accent only in small details (links, the small accent dot if used later), Newsreader serif for the wordmark and headings, Inter or system sans for the body if and where sans is needed. No textures, no gradients, no atmospheric photography, no stock images of people, mountains, or hands. No cards, drop shadows, or dashboard layouts. The visual is the in-the-retelling-support site exactly; if you find yourself reaching for something the support site does not have, pause and check.

## Locked content constraints

- The legal footer must carry the registered name (`Considered Ideas Ltd`), the registered office address, and the Companies House number. These are required for a publicly trading UK Ltd.
- The contact email is `enquiries@consideredideas.com`. No other public-facing email is named on the site.
- Products are linked, not described in marketing detail. The product page lives on its own site (e.g. the in-the-retelling-support repo). The company site lists products and links out.
- The consultancy section is intentionally minimal: a holding paragraph until there is a specific offer to describe.

## File map

```
considered-ideas-site/
  CLAUDE.md           (this file)
  README.md           project overview and publish workflow
  index.html          one-page front door
  styles.css          shared visual language with in-the-retelling-support
  .gitignore
```

## End-of-session checklist

Before declaring a session done:

1. No unresolved TODOs in `index.html` other than the legal-footer placeholders, which stay until the registered office address and Companies House number are confirmed.
2. The page validates as a plain static document (no JavaScript dependencies, no external CSS beyond what is in `styles.css`).
3. No personal data (home address, personal phone, personal email) is present anywhere in the repo.
4. No emoji, no em dashes, no banned words in any copy or comment.
