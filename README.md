# Tsar Bomba

> Overkill is the strategy.

One-page site for team **Tsar Bomba** at Lebanon CTF 2026 (Beirut, Oct 24).

Plain static HTML: no build step, no dependencies.

## Files

- `index.html` — the whole site (styles + script inline)
- `favicon.svg` — tab icon
- `_headers` — Cloudflare Pages security/caching headers

## Deploy (Cloudflare Pages)

1. Cloudflare dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
2. Pick this repo.
3. Build settings: Framework preset **None**, build command **empty**, output directory **`/`**.
4. **Save and Deploy**.
5. Project → **Custom domains** → add your domain/subdomain.

Every push to `main` redeploys automatically.

## Edit

- Countdown target: `const target = ...` near the bottom of `index.html`.
- Doctrine lines and spec sheet are plain HTML in the middle of the file.
