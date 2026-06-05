# streetfinance.co.za

Single-page marketing site for **Streetlight Financial Services** at
[streetfinance.co.za](https://streetfinance.co.za).

## Hosting

- **Cloudflare Pages** project: `streetfinance` (production branch: `main`).
- Custom domain: `streetfinance.co.za` (apex) — DNS managed in the Cloudflare
  `streetfinance.co.za` zone.
- Every push to `main` triggers a production deploy. Pull requests get a
  preview deploy at `<commit>.streetfinance.pages.dev`.

## Local preview

It's one static file — open `index.html` in a browser, or:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

No build step, no dependencies. Google Fonts loaded over CDN; the brand logo
is inlined as base64.

## Editing

Make the change, push to `main`, and the new version is live within ~60s.
