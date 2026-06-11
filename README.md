# Considered Ideas — company website

The static front-door site for Considered Ideas Ltd at `consideredideas.com`.

A small calm one-page presence that introduces the company, lists current products, names the consultancy offer, and carries the UK Ltd legal footer. Hosted on GitHub Pages with a custom domain. Sibling to the `in-the-retelling-support` repo; same visual aesthetic and editorial voice.

## What this site does

- Establishes a real, contactable company presence for Apple Developer review when In the Retelling is submitted under Considered Ideas Ltd.
- Carries the registered company information required for a UK Ltd that is publicly trading.
- Surfaces current products with links to their own support pages.
- Names the consultancy offer briefly without overcommitting on the form it takes.

## What this site does not do

- Sell anything directly. There is no e-commerce or payment flow.
- Collect data. No analytics, no cookies, no contact form. The only invitation to contact is a `mailto:` link.
- Run a blog or news section. If those become useful later, they can be added as static pages without changing the hosting story.

## Structure

```
considered-ideas-site/
  index.html          one-page front door
  styles.css          shared visual language with in-the-retelling-support
  README.md           this file
  CLAUDE.md           project brief for Claude Code
  .gitignore          OS / editor noise
```

## Editorial rules

UK English throughout. No em dashes anywhere. No emoji. Calm grown-up tone matching the voice used across the In the Retelling product. The brand wordmark is "Considered Ideas" set in Newsreader serif, same family as the In the Retelling app.

## Publish workflow

The same shape as the In the Retelling support site:

1. Edit files locally on a branch.
2. Commit and push.
3. GitHub Pages serves from the `main` branch.
4. Custom domain `consideredideas.com` points at the repo via a `CNAME` file once the DNS is configured.

DNS is owned by the registrar where the domain is held; the GitHub Pages side needs an `A` record set (or `CNAME` if using `www` as the canonical host).

## Status

Live at consideredideas.com. The legal footer carries the registered office (66 Paul Street, London EC2A 4NA) and Company No. 17258515, consistent with the App Store listing and the support site. The consultancy paragraph is a holding statement; it can be expanded once the offer is concrete.
