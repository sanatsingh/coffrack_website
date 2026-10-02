# Coffrack website

The public website for [Coffrack](https://coffrack.in), a calm, design-led
coffee companion for people who brew at home.

Plain HTML and CSS with no build step, no scripts, no cookies and no
analytics.

| File | What it is |
|---|---|
| `index.html` | Home page: what the app does |
| `privacy/index.html` | Privacy policy, served at `/privacy` |
| `tos/index.html` | Terms of use, served at `/tos` |
| `styles.css` | Styles; colours, radii and type mirror the app's design tokens |
| `assets/logo/` | Coffrack logo (SVG and PNG) |
| `assets/fonts/` | Inter, served locally, with its licence (SIL Open Font License 1.1) |

## Preview locally

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Hosting

Served at <https://coffrack.in> by Cloudflare Pages, connected to this
repository: every push to `main` deploys, and other branches get preview
URLs. There is no build step; the output directory is the repository root.
All links are relative, so the pages also work opened straight from disk.
