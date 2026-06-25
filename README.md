# Pen and Ink

A single landing page for **Pen and Ink** — a studio for *architecture · interiors · urbanism*.
A full-screen, auto-looping **pen-and-ink** slideshow of selected work. Monochromatic, no scroll,
no dropdowns: a quiet product showcase, not a marketing page.

**Open:** [`index.html`](index.html)

## What it is

- **One page only.** No other routes, no scrolling — everything lives in a single viewport.
- **Full-screen slideshow on loop.** Six interiors cross-fade automatically (~5s each) and loop
  forever; click the dots or use ← / → to move manually.
- **Pen & ink.** Each interior is rendered as a fine-line monochrome sketch (pre-processed with
  Pillow → [`assets/ink/`](assets/ink/)) and blended (`multiply`) onto the paper so the lines
  sit directly on the texture.
- **Background.** White with a very light grey paper grain (subtle SVG noise).
- **Minimal chrome.** Wordmark top-left; "Selected Work" + an **Enquire** link top-right
  (no dropdown menus). Caption bottom-left (project · type · year); progress dots bottom-right.
- **Loader.** A brief monochrome "VISHKAR" mark with a drawn line, then the show begins.

## Regenerating the ink images

Source photos live in [`assets/`](assets/) (`v-*.jpg`). The pen-and-ink versions are produced by
`ink.py` (grayscale → denoise → contour lines → light tonal wash → `multiply`). Re-run it to
re-process or add images, then point new `<img>` tags at `assets/ink/<name>.jpg`.

## To do (account actions — see hand-off notes)

- **Make the GitHub repo private** (repo Settings → General → Danger Zone → Change visibility).
- **Register the website Gmail.** The page currently links `penandink.studio@gmail.com` as the
  Enquire address — this needs to be created/confirmed.
