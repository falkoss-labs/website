# falkOSS labs – website

One static page for **falkOSS labs** at <https://labs.falkoss.org>: no build step, no framework, no external
resources, no cookies, no tracking. Same look as [falkoss.org](https://falkoss.org) (`falkoss/website`).

| Path | What |
|---|---|
| `index.html`, `style.css`, `404.html` | the page (English) |
| `assets/` | icons, lockup, mark, social preview – **copies** of `web-labs/` from [falkoss/brand](https://github.com/falkoss/brand) (CC BY-ND 4.0) |

Imprint and privacy policy are falkoss.org's – same operator, one place to keep them current.

Preview locally:

```sh
python3 -m http.server 8011
```

## Publishing

GitHub Pages via `.github/workflows/pages.yml` on every push to `main`. One-time setup:

1. Repo → Settings → Pages → Source: **GitHub Actions**; Custom domain: `labs.falkoss.org`; then **Enforce HTTPS**.
2. DNS at IONOS: `CNAME labs` → `falkoss-labs.github.io` (no A/AAAA records for `labs`).

Licence: the site's code is **AGPL-3.0-or-later** (`LICENSE`); the files in `assets/` are under CC BY-ND 4.0, and the
brand itself (logo, name, marks) is not covered by any licence – see falkoss/brand.
