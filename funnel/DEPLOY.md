# Deploy the Monstro funnel to Vercel (preview)

Everything is committed — no files need to be recreated. Pull the branch and deploy `funnel/`.

- **Repo:** `jahhornung-ops/wtf`
- **Branch:** `claude/jolly-einstein-w8bhw9`
- **Deploy directory:** `funnel/` (static HTML, no build step, Root Directory = `funnel`)

## Steps

```bash
# 1. Get the branch
git fetch origin claude/jolly-einstein-w8bhw9
git checkout claude/jolly-einstein-w8bhw9

# 2. Deploy funnel/ as a PREVIEW
cd funnel
npx vercel deploy --yes
#   - If not already authenticated, add:  --token="$VERCEL_TOKEN"
#   - To target the EXISTING project first:
#       npx vercel link --yes --project <PROJECT_NAME> [--scope <TEAM>]
#       npx vercel deploy --yes

# 3. Vercel prints a preview URL — that's the shareable link.
```

## What's in `funnel/`

- `landing.html`, `vsl.html`, `booking.html`, `thank-you.html` — the 4 funnel pages
- `assets/brand.css` — shared design system (Poppins/Roboto, Monstro palette)
- `ads/` — 4 static 1080×1080 ad creatives + `index.html` contact sheet; `ads/exports/*.png` are the rendered images
- `vercel.json` — already configured: clean URLs + redirect `/` → `/landing.html`
- `previews/` — full-page screenshots; `README.md` — full documentation

## Don't change

- Copy follows `monstro-messaging-framework-v3.md` (Market Ownership positioning). Don't rewrite it.
- Still placeholdered (intentional — live site blocks downloads): logo, Brian Dietz headshot, Carlos photo, VSL video embed, Calendly booking widget, privacy/terms links.
- Carlos Leal's real case video is already embedded on `vsl.html` and `thank-you.html`.
