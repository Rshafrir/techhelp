# Site — techhelp.now

Static one-page card site. Files: `index.html`, `styles.css`.

## Deploy (Porkbun)

Simplest path:

1. In Porkbun → techhelp.now → **DNS** / hosting, or upload via **URL Forwarding** only if you temporarily point elsewhere.
2. Preferred: host on **Cloudflare Pages**, **Netlify**, or **Porkbun site builder** if you use it — upload this `site/` folder.
3. Point DNS:
   - `A` / `CNAME` for `@` and `www` to the host (follow host’s docs)
4. Email: Porkbun → **Email forwarding**: `hello@techhelp.now` → your Gmail (or similar).

## Before public

- [ ] Replace “Add your phone number here” in `index.html` with real number
- [ ] Add Stripe payment link when created
- [ ] Confirm `hello@` forwarding works (send a test)

## Local preview

```bash
cd site && python3 -m http.server 8080
```

Open http://localhost:8080
