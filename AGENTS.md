# AGENTS.md

## Cursor Cloud specific instructions

This repository is a single, self-contained static personal resume website. There
is intentionally **no build system, no package manager, and no dependencies** — the
whole product is `index.html` (HTML + inline CSS/JS) plus `README.md`.

### Running the site (dev mode)
Serve the repo root with any static file server, e.g.:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000/`. There is no hot-reload; refresh the browser
after editing `index.html`.

### Build / Lint / Test
- **Build**: none — the file is served as-is.
- **Lint**: none configured.
- **Test**: none configured; verification is visual in a browser.

### Notes / gotchas
- All content lives inline in `index.html`; edit that file directly to change the
  resume. CSS variables at the top of the `<style>` block control theming.
- The floating pencil (✏️) button in the bottom-right links to an external GitHub
  edit URL (`github.com/yuan1618/resume-web/edit/main/index.html`). That repo may
  not exist, so the button can navigate to a GitHub 404 — this is expected and not
  a bug in this codebase.
