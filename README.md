# Site — techhelp.now

Static HTML/CSS. No build step.

- `index.html`, `styles.css` — the page
- `img/tech-table.jpg` (+ `-900` for phones) — hero illustration
- `print/` — flyer, rate card, tent card, director one-pager. Open in a browser, click the dotted blanks, print.

## Where it runs

GitHub Pages, repo `Rshafrir/techhelp`, branch `main`, custom domain `techhelp.now` (Porkbun A/AAAA → GitHub; `www` CNAME → `rshafrir.github.io`).
Email `hello@techhelp.now` forwards via Porkbun to Ron's Gmail.

## Deploy

```bash
# working clone lives at /tmp/techhelp-site; if missing:
#   gh repo clone Rshafrir/techhelp /tmp/techhelp-site
rsync -a --exclude .git --exclude CNAME --exclude .nojekyll --exclude .github site/ /tmp/techhelp-site/
cd /tmp/techhelp-site && git add -A && git commit -m "Update site" && git push
```

Live within about a minute. Cache is 10 minutes; add `?v=2` to force a fresh load.

## Before printing anything

- [ ] Phone number: `index.html` (search "hello@techhelp.now" — add the phone beside it) and the `phone` blanks in `print/`
- [ ] Stripe payment link when created

## Local preview

```bash
cd site && python3 -m http.server 8080 --bind 127.0.0.1
```
