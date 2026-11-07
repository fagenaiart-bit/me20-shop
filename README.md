# me20-shop

Live product data for **me20.studio/shop** (Glass UI kits): names, texts, prices, buy links and the waitlist link.

The site reads `shop.json` on every page request, so edits here show on the shop in about 1–2 minutes —
no Lovable publish needed. If the file can't be read, the site falls back to the copy bundled in the
main repo (`src/content/shop.fallback.json`).

No code lives here: everything in this file is already visible on the public shop page.

## Quick edits
- Price: `products[].price.personal` / `.commercial` (and `bundle.price`), in EUR.
- Start selling a kit: set `products[].buy.personal` / `.commercial` to the checkout links and `status` to `"available"`.
- Waitlist button: `waitlistUrl`.
- Texts are in `en` and `ua`.
