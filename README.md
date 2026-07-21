# Brioche — website

A single-file site. No build step, no paid services. Orders open WhatsApp with the order pre-filled.

## Put it live on Vercel (free)
1. Go to vercel.com and sign in with GitHub/Google.
2. Click **Add New → Project → deploy from folder** (or drag this whole `brioche` folder into the Vercel dashboard).
3. Vercel detects it as a static site. Click **Deploy**. Done — you get a free `*.vercel.app` link.
4. Later, add your own domain (e.g. brioche.pk) under Project → Settings → Domains.

Alternative (fastest): install the CLI once with `npm i -g vercel`, then run `vercel` inside this folder.

## The two things to edit
Open `index.html` and find the **CONFIG** block near the bottom (inside `<script>`).

- `whatsapp`: your number, digits only, with country code. `0300 1234567` → `923001234567`.
- `menu`: tomorrow's flavours. Set `filled:true` for filled donuts (prices at Rs.200 mini).
- `pickup`, `pickupTime`, `orderCutoff`, `discounts`: change as needed.

That's the only block you touch day to day.

## Photos (optional — it looks finished without them)
Drop files into an `images/` folder next to index.html:
- `images/hero.jpg` — the top donut shot
- `images/baker.jpg` — you in the kitchen (Story section)

If a photo is missing, a drawn donut + warm gradient shows instead, so the site never looks broken.
