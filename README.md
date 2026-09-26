# Tech Help · techhelp.now

Static HTML and CSS. No build step.

| Path | What it is |
| --- | --- |
| `index.html` | Home page for residents: the three ways to get help, what people bring, how to reach Ron |
| `directors/index.html` | Page for activity directors deciding whether to host a Tech Table |
| `assets/site.css` | Shared tokens, type, and components for every page and print sheet |
| `assets/icons.svg` | Icon sprite, used with `<use href="assets/icons.svg#name">` |
| `print/flyer.html` | Letter flyer for the bulletin board, with day, time, and room blanks |
| `print/tent-card.html` | Letter sheet that folds into a two-sided table card |
| `print/prices.html` | Two half-sheet price lists on one landscape Letter page |
| `print/director.html` | One-page leave-behind for an activity director |

Print sheets: open in a browser, click a dotted line to type, then use the Print button. Pages are sized for US Letter with no margins.

## Where it runs

GitHub Pages from `main` (`.github/workflows/pages.yml`), custom domain `techhelp.now` via `CNAME`. Email Ron at `ron@techhelp.now` (mailbox setup in progress).

## Before printing or going live

- [ ] Add a phone number beside `ron@techhelp.now` on the home page, the directors page, and the print sheets
- [ ] Add the Stripe payment link once it exists

## Local preview

```bash
python3 -m http.server 8080 --bind 127.0.0.1
```
