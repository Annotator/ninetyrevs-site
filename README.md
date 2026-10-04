# ninetyrevs-site

Public website of the Ninety Revs iPhone app, served by GitHub Pages at https://ninetyrevs.com.

| Path | Page |
| --- | --- |
| `/`, `/de/` | Landing page (English, German) |
| `/support/`, `/de/support/` | Support and FAQ |
| `/privacy/`, `/de/privacy/` | Privacy policy |

Plain HTML and one stylesheet (`assets/site.css`): no build step, no JavaScript, no cookies, no trackers and no
external fonts, scripts or CDNs. Adding any of these requires updating the privacy policy. English pages live at
unprefixed paths, German pages under `/de/`; every page links to its counterpart. Keep both languages in sync.

The privacy policy describes what the app actually does; update it together with app changes that add network
requests, data stored in the account, third-party services or permissions.

## Assets

Copied unchanged or resized from `Brand/` in the app repository (do not redraw the 90R mark):

- `assets/90r-black.svg`, `assets/90r-white.svg`: `Brand/90R/90R-black.svg`, `90R-white.svg`
- `assets/app-icon-384.png`, `apple-touch-icon.png` (180 px), `favicon.png` (64 px):
  `Brand/AppIcon/90R-topography-1024.png`, resized with `sips -Z`

## Preview and publishing

Open the HTML files directly or run `python3 -m http.server` in the repository root. GitHub Pages publishes the
`main` branch root; `CNAME` sets the custom domain.
