# BFG Sudoku — public site

Public static pages for **BFG Sudoku** App Store / TestFlight fields:

| Page | Path | Purpose |
|---|---|---|
| Home | [`index.html`](index.html) | Short product blurb |
| Support | [`support.html`](support.html) | Support contact |
| Privacy | [`privacy.html`](privacy.html) | Privacy Policy |
| Accueil (FR) | [`index-fr.html`](index-fr.html) | Blurb French (Canada) |
| Assistance (FR) | [`support-fr.html`](support-fr.html) | Support FR — App Store FR Support URL |
| Confidentialité (FR) | [`privacy-fr.html`](privacy-fr.html) | Privacy FR — App Store FR Privacy URL |

**Support email:** bfgames.support@gmail.com

## Published URLs (GitHub Pages)

After Pages is enabled from the `main` branch root:

- Home: https://vh3.github.io/bfg-sudoku-site/
- Support: https://vh3.github.io/bfg-sudoku-site/support.html
- Privacy: https://vh3.github.io/bfg-sudoku-site/privacy.html
- Accueil (FR): https://vh3.github.io/bfg-sudoku-site/index-fr.html
- Assistance (FR): https://vh3.github.io/bfg-sudoku-site/support-fr.html
- Confidentialité (FR): https://vh3.github.io/bfg-sudoku-site/privacy-fr.html

These URLs are the App Store Connect Support URL and Privacy Policy URL sources. The private iOS source repository must not be used for those fields.

## Enable GitHub Pages

1. Repo Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main` / `/ (root)`
4. Save, wait for the site to become live

Or via CLI (owner):

```bash
gh api -X POST repos/vh3/bfg-sudoku-site/pages \
  -f build_type=legacy \
  -f source[branch]=main \
  -f source[path]=/
```

## Local preview

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8080
```
