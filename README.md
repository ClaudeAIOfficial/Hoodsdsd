# Business Cat — $BIZCAT

Scroll-driven 3D landing page for Business Cat, live on Robinhood Chain.
The cat walks through five department doors as you scroll — ORIGINS, FINANCE,
STRATEGY, ACQUISITIONS, BOARDROOM — with a coin-confetti finale on the top floor.

Single self-contained file: the 3D model is procedural (three.js r128 via CDN),
the face logo is embedded as base64. No build step, no dependencies.

## Run locally

Open `index.html` in a browser. That's it.

## Deploy on GitHub Pages

1. Push this repo to GitHub.
2. Settings → Pages → Source: `main` branch, root folder.
3. Site goes live at `https://<user>.github.io/<repo>/`.

## Before launch

- **Contract address** — replace the placeholder inside the `#caText` element in `index.html`.
- **Chart link** — the 📈 links (menu + boardroom card) still point to `#`; set your Dexscreener URL.
- **Step 3 of How to Buy** — name the actual DEX once known.

## Tuning

Everything lives in the `CONFIG` object at the top of the inline script:
door positions, walk speed, scroll easing, colors. `FACE_SPIN` (near the held
coin) rotates the minted face if it reads tilted in your browser.

`assets/` holds the original artwork and the extracted face logo for socials.
