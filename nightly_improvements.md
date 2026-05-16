# Tau Optics — Nightly Improvements Log

## 2026-05-16 — Animated metrics strip (count-up numbers) + publications reveal fix — No new files in Additional info/ (all 7 already processed). Added a four-column metrics strip between the masthead and Technology section displaying the four key performance claims (10×, 60×, ~5 cm², 95%) as large serif numerals that count up from zero via eased requestAnimationFrame animation when scrolled into view; respects prefers-reduced-motion. Also fixed missing scroll-reveal class on the Publications section.

## 2026-05-14 — Staggered use-case card entrance + spec-row hover micro-interactions — No new files in Additional info/ (all 7 already processed by prior runs). Added CSS/JS staggered cascade animation to the 6 Use Case cards using IntersectionObserver + nth-child transition-delay (0–375 ms), so cards roll in as a wave rather than all at once; respects prefers-reduced-motion. Added spec-row micro-interaction: on hover each row indents 0.6 rem, brightens the label to text color and lightens the accent value — creating a subtle data-table feel consistent with the editorial dark aesthetic.

## 2026-05-13 — Sticky floating "Request a Demo" CTA — No new files in Additional info/ since last run (all 7 already processed). Added a fixed-position "Request a Demo" button that fades in via IntersectionObserver once the masthead scrolls out of view, and auto-hides when the contact section becomes visible — keeping the conversion nudge persistent without obscuring the destination.

## 2026-05-12 — Competitor comparison table + scroll-reveal animations — The comparison table makes SpectraMini's key advantages (10× smaller, 60× throughput, fewer parts, lower cost) immediately scannable against Portable and Benchtop Raman, while IntersectionObserver-based scroll reveals give every section a polished, purposeful entrance without any external libraries.

## 2026-05-12 — Added r-CBG grating dimensions + AR-coating validation news + restored publications + enriched spec card — Extracted 6 PPTX files (PDF skipped, no pdftotext); key new facts: grating element is 3×6×25 mm, AR-coated samples achieved 2.4 nm FWHM at 900–920 nm in Feb 2026. Added r-CBG element row to spec card, restored PTR glass + X-CBG + Bluetooth paragraphs in technology section, added Feb 2026 and May 2025 MIT news items, restored publications section with Research nav link. Merged with existing comparison table and scroll-reveal implementation.

## 2026-05-12 — Mobile hamburger nav — All 7 files in Additional info/ confirmed processed. Implemented accessible hamburger menu: animated 3-bar icon (CSS transforms, no images) toggles a full-width frosted-glass dropdown on mobile, closes on link click or outside tap, with aria-expanded for screen readers — fixing the critical gap where mobile visitors previously had zero navigation.

## 2026-05-15 — Company milestone timeline + University of Utah collaboration mention — No new files; feature run only

### Part 1 — Files processed
All 7 files in `Additional info/` were already in `processed_files.md` from prior runs. No new files found.

### Part 2 — Website improvement: Company milestone timeline
Added `#milestones` section between About and Partners — a vertical timeline showing the company's journey from 2023 (CREOL demonstration) through 2024 (founding, UCF license, I-Corps), 2025 (NSF STTR Phase I, MIT presentation), Feb 2026 (AR-coating validation), and a forward-looking 2026 milestone (prototype completion, pilot deployments). Each item uses a dot on a vertical rule; key milestones use the accent blue; the NSF award uses the accent orange; the final future milestone is visually neutral. Implements with pure CSS (no JS needed — uses existing scroll-reveal class). Respects existing dark editorial aesthetic.

Also updated About text to include the University of Utah (ECE department) collaboration — sourced from the `Miniature spectrometer_MIT.pptx` co-author list (T.M. Hayward, R. Menon) — not yet reflected in the body copy.
