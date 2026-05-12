# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

Static single-page marketing website for **Tau Optics** — a UCF spinout commercializing the SpectraMini Raman spectrometer. Hosted at `tauoptics.com` via GitHub Pages (CNAME file present).

## Files

- `index.html` — the live website (all HTML, CSS, and JS in one file)
- `TauOptics website.html` — legacy draft kept for reference; not served
- `Images/` — partner/collaborator logos and product photos
- `TauOpticsLogoBlack2.png` — company logo (referenced from parent path `../` in index.html due to GitHub Pages serving from the repo root)

## Development

No build step, no dependencies, no package manager. Open `index.html` directly in a browser to preview. The site is pure HTML/CSS/JS — edit the file and refresh.

## Architecture

Everything lives in `index.html`:

- **CSS**: all styles are in a single `<style>` block using CSS custom properties defined on `:root` (colors, fonts, max-width). The design system uses three font families — `Playfair Display` (headings), `IBM Plex Mono` (labels/badges), `Source Serif 4` (body) — all loaded from Google Fonts.
- **Sections** (in order): nav → masthead (`#top`) → `#technology` → `#applications` → `#about` → `#partners` → `#news` → `#publications` → `#backed` → `#contact` → footer
- **No team section** — do not add team members, team cards, or any "Meet the Team" content. User has explicitly requested this be omitted.
- **JS**: two small inline scripts — an `IntersectionObserver` that highlights the active nav link, and a contact form `submit` handler that opens a `mailto:` link (no backend).
- **Responsive**: a single `@media (max-width: 768px)` breakpoint collapses grids to single-column and hides the nav links.

## Content notes

- Product: **SpectraMini** — uses patented **r-CBG (rotated chirped Bragg grating)** technology
- Funding: **NSF STTR Phase I** (referred to as "NSF Seed Fund" in logo/badge copy)
- Affiliation: UCF Business Incubation Program, CREOL (College of Optics & Photonics)
- Contact email: `info@tauoptics.com`
- The inline SVG in `#technology` diagrams the r-CBG operating principle — edit carefully, coordinates are hand-tuned
