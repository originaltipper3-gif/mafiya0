# Toss Mafiya — Telegram Channel Landing Page

A mobile-first landing page for the Toss Mafiya Telegram channel. It shows the channel's branding and highlights, runs a 15-second countdown with circular and linear progress indicators, and then sends visitors to the channel automatically. Visitors can also join right away with the main button, the fallback link, or the sticky bottom bar.

## Technologies

- Plain HTML in a single file (`index.html`) with no build step
- Tailwind CSS (Play CDN), Font Awesome 6, and Google Fonts (Outfit, Rajdhani)
- A small inline script for the countdown and redirect
- Hosted on Netlify, which serves the repository root as static files

## Running locally

Open `index.html` in a browser, or serve the folder with any static server, e.g.:

```bash
npx serve .
```

## Customizing

- **Telegram link:** change `targetTelegramUrl` in the script at the bottom of `index.html`, and the `href` on the three join links.
- **Countdown length:** change `totalSeconds` in the script, and the initial `15` shown in the markup.
