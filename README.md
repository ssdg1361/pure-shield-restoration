# Pure Shield Restoration — site

Hugo static site for Pure Shield Restoration (water / mold / fire damage restoration, Boca Raton + South Florida). Same pattern as the Vent Viper build: Hugo + GitHub Pages, auto-deployed via GitHub Actions on push to `main`.

- **Repo:** ssdg1361/pure-shield-restoration
- **Live URL (once Pages is on):** https://ssdg1361.github.io/pure-shield-restoration/
- **Phone on site:** (561) 583-6375
- **Stack:** Hugo extended 0.128.0, custom layouts + CSS, no theme.

## Local dev
```bash
hugo server -D       # preview at localhost:1313
hugo --minify        # build to ./public
```

## Deploy
Push to `main` → the `.github/workflows/deploy.yml` action builds and deploys to Pages.
First time only: in GitHub repo Settings → Pages → Source = **GitHub Actions**.

## TODO before going fully live
- Set the lead form endpoint in `layouts/index.html` (search `YOUR_FORM_ID`) to a real Formspree (or other) form, or swap for a call-only CTA.
- Swap the placeholder reviews for real Google reviews.
- Add an OG/share image at `static/images/og-image.png` + reference in `baseof.html`.
- Confirm phone number with Dan/owner (two numbers were floating around: 561-583-6375 vs 561-264-7034).
- Optional: point a custom domain (add `static/CNAME`).
