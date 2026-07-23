# Nanny Weekend Instructions

Single static page: `index.html`. No build step, no dependencies.

## Deploying to Vercel

1. In the Vercel dashboard, **Add New → Project**, import this repo (`jahhornung-ops/wtf`).
2. Set **Root Directory** to `nanny-weekend`.
3. Framework Preset: **Other** (static site) — no build command needed.
4. Deploy. Vercel will give you a URL like `wtf-nanny-weekend.vercel.app`.

The page is unlisted (`noindex`) and gated behind a password prompt (see below) since it
contains house-access and away-schedule details. It is not real security — just a basic
deterrent against a random visitor with the link. Share the URL and password with Maya
directly (text/verbally), not in any public place.

## Password

Set in chat when this was generated — check with the person who deployed it if you don't
have it. To change it: pick a new password, compute its SHA-256 hex digest, and replace
`CORRECT_HASH` in `index.html`'s script. E.g. in a terminal:

```
printf '%s' 'your-new-password' | sha256sum
```

## Before sharing the link

Fill in the blank fields in the "Contacts" section (phone numbers, address, pediatrician,
vet, WiFi) — those weren't in the original instructions and are left as placeholders.
