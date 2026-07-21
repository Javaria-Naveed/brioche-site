# Brioche — project context

## What this is
Single-file static website (index.html) for Brioche, a home donut brand in Karachi run by Javaria (Jo). Cold-fermented brioche donuts, 20+ hours dough to donut, fried fresh per preorder. Instagram: @brioche_pakistan. Separate brand from her cookie bakery, Jo & Co. (joandcobakes.com) — don't mix the two.

## Current model
- Daily evening batches sold at Kings Towers, Play Area, 7pm pickup/delivery.
- Preorders via WhatsApp: the site's "Order" buttons open wa.me with the order pre-filled. No backend, no payments online.
- This is a proving ground: she's building an audience and sales track record to pitch for a donut stall at IBA Karachi (campus grants category exclusivity — no second donut stall allowed).

## Pricing (structure-based, may be revised)
- Mini, not filled: Rs. 180
- Mini, filled: Rs. 200
- Regular, not filled: Rs. 350 (preorder-only for now)
- Regular, filled: Rs. 390 (preorder-only for now)
- Box discounts: 2 donuts = 5% off, 4+ = 10% off (auto-applied in cart)

## Current flavours
- Milk Chocolate & Sprinkles (glazed)
- Dark Chocolate (glazed)
- Nutella-filled, rolled in sugar

## How the site works
- Everything lives in index.html. The CONFIG object at the bottom (in <script>) holds: WhatsApp number, pickup location/time, order cutoff (2pm for same-evening), discounts, and the daily menu array. Daily menu changes = edit CONFIG only.
- Photos go in images/hero.jpg and images/baker.jpg; a CSS-drawn donut fallback shows if absent.
- Design: warm cream/amber/espresso palette, Fraunces + Hanken Grotesk, styled as a sibling of joandbakes.com (editorial voice, generous space). Keep that character in any edits.
- Hosted on Vercel (free tier), deployed via CLI. Repo should auto-deploy on push once linked.

## Owner preferences
- Honest, critical feedback over reassurance. Minimal-complexity, direct solutions. No paid services. Plain human voice in copy, no em-dashes, no AI-sounding phrasing.

## Likely upcoming work
- Daily menu/flavour rotation edits, adding a "only N tonight" scarcity note, enabling regular-size donuts in the picker, adding real photos, order-count tracking, eventually IBA-stall-related pages.
