# tapcrate.dev

The TapCrate website: home page, app listings (ResDemand, Our Cashflow), support, privacy policy and terms of use.

Plain HTML and CSS with no build step. Hosted on Cloudflare (Workers static assets, configured in `wrangler.jsonc`): every push to `main` publishes the site. `.assetsignore` keeps repo files like this README off the live site.

- `index.html` home, apps, about, contact
- `support.html`, `privacy.html`, `terms.html`
- `style.css` shared styles
- `img/` app icons
- `_headers` security headers (CSP, HSTS, framing, referrer) applied to every page
