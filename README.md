# Site — techhelp.now

Static HTML/CSS. No build step.

- `index.html`, `home.css` — one-viewport home (brand, one line, email CTA)
- `prices.html`, `prices.css` — full price list
- `img/tech-table-hero.jpg` — clubhouse / phone-in-hands photo
- `print/` — flyer, rate card, tent card, director one-pager. Open in a browser, click the dotted blanks, print.

## Where it runs

GitHub Pages, repo `Rshafrir/techhelp`, branch `main`, custom domain `techhelp.now` (Porkbun A/AAAA → GitHub; `www` CNAME → `rshafrir.github.io`).
Email `hello@techhelp.now` forwards via Porkbun to Ron's Gmail.

## Deploy

Push to `main`. The Pages workflow deploys the repo root. Live within about a minute. Cache is about 10 minutes; add `?v=2` to force a fresh load.

## Before printing anything

- [ ] Phone number: add beside `hello@techhelp.now` on the print blanks in `print/`
- [ ] Stripe payment link when created

## Local preview

```bash
python3 -m http.server 8080 --bind 127.0.0.1
```
