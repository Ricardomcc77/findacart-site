# FindACart holding page

Temporary static site for findacart.com until the full web app launches. Plain HTML and CSS, no build step, no JavaScript.

- `/` home, `/privacy`, `/terms`, `/support` (each folder has an `index.html`).
- Privacy and terms are converted from the web app's pages with the wording unchanged.
- Fonts are self-hosted (SIL Open Font License, files in `fonts/`).

Preview locally: `python3 -m http.server 8765` in this folder, then open http://127.0.0.1:8765.
