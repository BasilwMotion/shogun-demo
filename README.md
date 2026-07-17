# Shogun Website Demo

Demo website for **Shogun Construction** — Specialist Mining Construction & Engineering (est. 1994, Parys, Free State, South Africa).

## Pages

- `index.html` — Homepage: history timeline, safety, growth roadmap, services overview, Google Maps, partner logo marquee
- `services.html` — Services & Products: interactive 3D models (mills, crushers, winders) that disassemble as you zoom out and reassemble as you zoom in (mouse wheel, pinch on touch, or the Take apart button), plus guided 3D walk-throughs of a cement plant and a concentrator plant
- `contact.html` — All phone numbers, email addresses, contact form and map

Static site — no build step. 3D powered by Three.js from CDN. Photos and logos are loaded from shogun.co.za. Fully responsive: no horizontal scroll on phones, header text never overlaps the menu button.

## Run locally

Open `index.html` in a browser, or:

```bash
npm run dev
```

## Deploy to Vercel

**Option A — GitHub + Vercel (recommended)**

```bash
git init
git add .
git commit -m "Shogun website demo"
gh repo create shogun-website-demo --public --source=. --push
# or create the repo on github.com and:
# git remote add origin https://github.com/<your-username>/shogun-website-demo.git
# git push -u origin main
```

Then go to [vercel.com/new](https://vercel.com/new), import the `shogun-website-demo` repo and click **Deploy**. No framework or build settings needed — Vercel serves it as a static site.

**Option B — Vercel CLI (no GitHub needed)**

```bash
npx vercel --prod
```
