# AGENTS.md

## Architecture

A static, single-page site with no build step. Everything lives in `index.html`: markup, a small `<style>` block for custom effects (glow, pulse, shimmer, glassmorphism), and an inline script for the countdown and redirect. `netlify.toml` publishes the repository root.

## Key files

- `index.html` — the whole page
- `netlify.toml` — sets the publish directory to `.`

## Conventions and decisions

- The page was supplied by the owner as a finished file and is deployed as-is. Keep edits small and don't add a framework or bundler unless asked.
- Styling uses Tailwind utility classes from the Tailwind Play CDN; custom CSS goes only in the inline `<style>` block.
- The Telegram invite URL shows up in four places (three `href`s plus `targetTelegramUrl` in the script). Keep them in sync.
- The countdown duration is set by `totalSeconds` in the script and also hard-coded as `15` in the initial markup. Update both together.
