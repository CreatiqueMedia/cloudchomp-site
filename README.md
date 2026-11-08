# Cloud Chomp Site

Static website, privacy policy, support page and terms of use for **Cloud Chomp: Math & Spelling** (in-app title "Cloud Chomp: The Hungry Sky"), a kids' learning game for kindergarten through 8th grade, published by [CreatiqueMedia LLC](https://creatiquemedia.com).

**Live site:** https://creatiquemedia.github.io/cloudchomp-site/

## Overview

This repository contains the public web presence for the Cloud Chomp app. It is a plain HTML site with no build step, served directly by GitHub Pages. The pages are the marketing landing page plus the legal and support pages needed for app store listings.

## About the app

Cloud Chomp is a tap-to-shoot learning game: answers float down and the player taps the right one while the character, Chompy, transforms. According to the site:

- **Math, K-8**: addition, subtraction, multiplication, division and pre-algebra, matched to grade level.
- **Spelling, K-8**: 162 built-in words with a clue for each, read by offline Boy or Girl voices; grown-ups can add custom word lists.
- **Shapes and polygons**: bright shapes plus a Polygons mode; matching never relies on color alone.
- **Light and Dark adventures**: twelve Chompy forms.
- **Pacing options**: harder problems fall slower, speed is adjustable, and Practice mode has no game over.
- **Privacy**: no ads, no analytics, no accounts, and it works offline.
- **Pricing**: Matching games plus Math and Spelling for K-2 are free. Cloud Chomp Plus unlocks grades 3-8, custom spelling lists and future lessons (yearly subscription with a free trial, or a one-time lifetime purchase). App Store and Google Play badges are marked "Coming soon".

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Landing page: hero with promo video, feature cards, screenshots, pricing summary |
| `privacy.html` | Privacy policy |
| `support.html` | Support and common questions (restoring purchases, canceling subscriptions, game speed) |
| `terms.html` | Terms of use |

## Project structure

```
index.html, privacy.html, support.html, terms.html   Site pages
images/                                               Screenshots, cover and social preview images
                                                      (No video files are stored here: the landing page plays the commercial from YouTube, click to play)
.nojekyll                                             Tells GitHub Pages to serve files as-is (no Jekyll)
README.md                                             This file
```

## How it is served

The site is published with GitHub Pages from the root of the repository's `main` branch. The empty `.nojekyll` file disables Jekyll processing, so the HTML files are served exactly as committed. Pages link to each other with relative paths, and `index.html` declares a canonical URL and Open Graph/Twitter preview metadata pointing at the Pages address above.

## Editing the site

1. Clone the repository.
2. Edit the HTML files directly; styles and markup for each page are in the file itself.
3. Preview locally by opening `index.html` in a browser, or run a simple static server, for example `python -m http.server` from the repository root.
4. Commit and push to `main`. GitHub Pages republishes automatically, usually within a minute or two.

When changing policy text, update the "Last updated" date on `privacy.html` or `terms.html`. Keep screenshots and the promo video in `images/` and `media/` and reference them with relative paths.

## Contact

Support: info@creatiquemedia.com

---

© CreatiqueMedia LLC. All rights reserved.
