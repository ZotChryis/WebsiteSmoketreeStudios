# Smoketree Studios Website

Static site for [Smoketree Studios](https://www.smoketreestudios.com) — an indie game label.

## Structure

- `index.html` — the live site (V6 "Rainier": parallax forest hero, animated sign logo)
- `designs/` — earlier design candidates kept for reference
- `assets/logo-anim.mp4` — web-optimized animated logo (cropped, muted, fade-out trimmed)
- `assets/logo-still.png` — static logo frame (poster, about)
- `assets/logo-mark.png` — transparent-background logo mark (navbar)
- `assets/sasquatch.png` — sasquatch silhouette (parallax cameo)
- `SmoketreeStudiosLogoAnim.mp4` — original full-res animated logo
- `CNAME` — custom domain for GitHub Pages

## Games

| Game | Platform | Link |
|------|----------|------|
| Lil Laundry Lane | Steam (coming soon) | https://store.steampowered.com/app/4729080/ |
| DungeonSweeper | Steam + Android | https://store.steampowered.com/app/4109840/ |
| RunVR | Steam VR | https://store.steampowered.com/app/542570/ |
| Caketomino | Steam VR | https://store.steampowered.com/app/517770/ |
| Alchehistory | Android | https://play.google.com/store/apps/details?id=com.SmoketreeStudios.Trees.Alchehistory |
| SLicense to Dye | Android | https://play.google.com/store/apps/details?id=com.SmoketreeStudios.SLicensetoDye |

## Deploy

GitHub Pages: Settings → Pages → Deploy from branch → `main`, root (`/`).

DNS (Squarespace, for the custom domain):
- `CNAME` record: `www` → `zotchryis.github.io`
- `A` records on apex (`@`): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- Then in repo Settings → Pages set custom domain `www.smoketreestudios.com` and enable "Enforce HTTPS" once the cert issues.

Note: asset paths in the HTML are root-relative (`/assets/...`), which assumes the site is served at the domain root (custom domain or `username.github.io`). If previewing locally, serve with any static server from the repo root.
