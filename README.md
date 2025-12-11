# SuMail Website

Landing page for the SuMail Chrome extension (summaries, translation, tone analysis, reply templates). Built with plain HTML/CSS/JS and ships with a KO/EN toggle.

## Highlights
- Hero: product tagline, primary CTA (Chrome Web Store), and key stats (paste/selection support, auto/manual templates, supported languages).
- Preview cards: demo blocks for summary, tone analysis, and reply template UI.
- Features & workflow: six feature cards plus a three-step “how it works”.
- Language toggle: `ko/en` switch updates all copy and persists preference in `localStorage`.
- Interactions: `IntersectionObserver` fade-up animations and forced scroll-to-top on refresh.

## Stack
- Static site only: `index.html`, `styles.css`, and a small inline script.
- Design: CSS custom properties for colors/radius/shadows; grid/flex layout with soft gradient background.
- Assets: PNG logos in `assets/`; `fonts/` ready for optional custom fonts.

## Run locally
1) Open `index.html` in your browser, or  
2) Serve with a tiny local server:
   ```bash
   python3 -m http.server 4000
   # visit http://localhost:4000
   ```

## File map
- `index.html` — markup and i18n script.
- `styles.css` — layout, type, and animation styles.
- `assets/` — SuMail logo images.
- `fonts/` — optional custom font directory.

## Customize
- Copy/i18n: edit the `I18N` object near the top of `index.html`. To add a language, add a key and call `applyLang` with it.
- Colors/styles: tweak the `:root` CSS variables in `styles.css` to match your branding.
- CTA links: replace the Chrome Web Store URLs in the hero and CTA sections with the real listing link.

## Deploy
No build or server required. Upload as-is to GitHub Pages, Netlify, Vercel, or any static host.
