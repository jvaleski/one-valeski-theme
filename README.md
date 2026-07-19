# Minima

A super-minimalist theme for [Ghost](https://ghost.org), built for quiet, readable long-form writing. System sans-serif type, lots of whitespace, a text-only post list. Keeps Ghost's **subscribe** (Members/Portal) and **search** (Sodo Search) functionality fully wired.

## What it looks like

- **Homepage** — site title + nav + search + Subscribe button, an optional one-line site description, then a clean text-only list of posts (title on the left, date on the right).
- **Post/page** — centered ~680px reading column, restrained typography, feature image only if set.
- **Footer** — an email subscribe box (shown to non-members), copyright, secondary nav, "Powered by Ghost".

## Install

1. Zip the theme (already done for you — see `minima.zip`), or run:
   ```
   zip -r minima.zip . -x ".git/*" "*.DS_Store" "minima.zip"
   ```
2. In Ghost admin (`https://jvaleski.ghost.io/ghost`) go to **Settings → Design & branding → Change theme → Upload theme**.
3. Upload `minima.zip`, then click **Activate**.

Your existing Casper theme stays installed, so you can switch back anytime from the same screen.

## Customizing

- **Colors** — Minima uses your Ghost **accent color** (Settings → Design → Brand) for the Subscribe buttons.
- **Fonts** — pick heading/body fonts in **Settings → Design → Typography**; Minima falls back to the system sans stack when none is set.
- **Theme settings** — Settings → Design → Site-wide:
  - *Accent links* — color in-article links with your accent color instead of underlined black.
  - *Signup heading* — heading for the footer subscribe box (defaults to your site title).
- **Nav & search** — driven by your Ghost navigation settings; search needs no config.
- **Posts per page** — 25 (edit `config.posts_per_page` in `package.json`).

## Validated

Passes `gscan` with **0 errors, 0 warnings** — compatible with Ghost 6.x.
