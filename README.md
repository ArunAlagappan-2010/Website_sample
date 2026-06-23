# Vishkar Interiors — Website Concepts

Six website directions for **Vishkar Interiors**, an interior-design studio. This round is about
**structure**, not paint: each concept has a genuinely different skeleton — where the nav sits,
which way the page scrolls, how content is positioned — plus its **own loading animation**.

Shared brief throughout: minimal, black-and-white, inspired by apple.com, **sleek dropdown
navigation** across all six menus (About Us · Services · Our Portfolio · Office · Careers ·
Contact Us), minimal copy, and **booking a consultation** as the primary action.

**Start here:** open [`index.html`](index.html).

## The six structures

| # | Concept | Nav position | Scroll | Loader |
|---|---------|--------------|--------|--------|
| 01 | [Centered Classic](concept-1-product/index.html) | Top-centre | Down ↓ | Logo letters stagger in |
| 02 | [Fixed Left Rail](concept-2-editorial/index.html) | Left vertical rail | Down ↓ | Line draws down, wipes left |
| 03 | [Split-Screen Diptych](concept-3-swiss-grid/index.html) | Top (over right pane) | Down ↓ (left pane fixed) | Two panels part apart |
| 04 | [Horizontal Scroll](concept-4-cinematic/index.html) | Top | **Sideways →** | Marker sweeps, wipes right |
| 05 | [Fullscreen Snap Deck](concept-5-studio/index.html) | Top + side dots | Down ↓ snap (100vh panels) | 0–100% counter on black |
| 06 | [Asymmetric Grid](concept-6-typographic/index.html) | **Top-right** | Down ↓ | Black block + counter, wipes up |

## How they differ structurally

- **01 Centered** — the familiar baseline: centred hero, vertical sections.
- **02 Left Rail** — navigation is a fixed vertical sidebar; content is offset to the right.
- **03 Split-Screen** — viewport split in two; the left image/booking pane stays put while the
  right scrolls, and the left image swaps to match each section.
- **04 Horizontal** — scrolling moves the page sideways, panel by panel (progress bar + pager).
- **05 Snap Deck** — one full-screen panel at a time with side-dot navigation; a slide-deck feel.
- **06 Asymmetric** — right-aligned nav over a broken, off-centre grid with oversized type.

## Shared across all six

- **Black & white**, Apple-minimal, deliberately sparse copy.
- **A different custom loading screen** on every page (see table above), each animating the
  Vishkar wordmark, then revealing the page in a way that matches the layout.
- **Sleek dropdown navigation** with all six menus — implemented differently per concept.
- **Booking-led** — a persistent "Book a Consultation" CTA + a working booking form that
  confirms on submit; sections funnel toward it.
- Full mobile fallbacks (horizontal scroll and snap deck collapse to normal vertical scroll).

## Notes

- Each concept is a **self-contained HTML file** — no build step. Just open it.
- Photography is from Unsplash (free to use), in [`assets/`](assets/) (`v-*.jpg`), so pages work
  offline. Replace with Vishkar's real project photography later.
- Reference studios (well-known interior designers) are listed in [`references.md`](references.md).
