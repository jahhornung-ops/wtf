# Monstro — Market Ownership Funnel (Deliverable Pages + Ad Creatives)

Built by Academy of Advertising · June 2026. Copy source of truth: `../monstro-messaging-framework-v3.md` (Market Ownership positioning).

## What's here

```
funnel/
├── assets/brand.css        Shared brand system (Poppins/Roboto, Monstro palette)
├── landing.html            Landing page  — "One school in your city owns the search results. Is it yours?"
├── vsl.html                VSL page      — video sales letter (Brian Dietz, 7-min)
├── booking.html            Booking page  — "Your territory may still be available."
├── thank-you.html          Confirmation  — post-booking, with pre-call homework
├── ads/
│   ├── index.html          Contact sheet (previews all 4 ads)
│   ├── ad-1-search.html     "Do they find you first?"   (white / search bar)
│   ├── ad-2-renting.html    "Renting vs Owning"         (split compare)
│   ├── ad-3-agency.html     "On your 3rd agency?"       (dark)
│   ├── ad-4-carlos.html     "120 → 300+, ads off"       (social proof)
│   └── exports/            Rendered 1080×1080 ad PNGs (2160² @2x) — ready to upload
└── previews/              Full-page screenshots of each page (desktop + landing mobile)
```

## Funnel flow

Ad (image or video) → Survey (5-q pre-qualifier, see framework) → **landing.html** → **vsl.html** → **booking.html** → **thank-you.html**, then the email/SMS sequences in the framework doc.

## Brand system (extracted from mymonstro.com)

- **Fonts:** Poppins (headings), Roboto (body) — loaded via Google Fonts in `brand.css`.
- **Palette:** black `#000` buttons → indigo `#6366f1` hover · indigo-600 `#4f46e5` accent · red `#ef4444` highlight · slate-950 `#020617` dark sections · slate-100 `#f1f5f9` light sections · yellow `#facc15` stars · green `#22c55e` checks.
- All pages share `assets/brand.css` — edit once, every page updates.

## Real assets still to drop in

These are intentional placeholders (the live site blocks automated downloads):

1. **Logo** — text wordmark `MONSTRO` stands in. Replace with the real logo (`/_next/static/media/logo.0ef6d2b8.png`, 616×187) in each page header/footer and in the ads. Search the files for the `LOGO:` comment.
2. **Photos** — Brian Dietz headshot (booking + landing credibility), Carlos Leal photo (landing testimonial). Styled placeholders are marked with comments.
3. **VSL video** — `vsl.html` has a `.video-frame` placeholder with an embed comment. Drop in Brian's recorded VSL when ready.
4. **Booking widget** — `booking.html` has a Calendly-sized placeholder; insert the real booking iframe.
5. **Privacy / Terms links** — footer links are `#` stubs.

> Carlos Leal's real case-study video (`youtube.com/embed/HLFUfPlfsXg`) is already embedded on `vsl.html` and `thank-you.html`.

## Re-exporting the ad PNGs after edits

The ads are HTML so they stay editable. Each contains one `1080×1080 .ad-stage`. To export: open the file in a browser and screenshot the stage, or use a headless-Chromium element screenshot of `.ad-stage` (what produced `ads/exports/*.png` at 2× / 2160²).

## Notes

- Pages are responsive (360–1440px) and self-contained except the shared `brand.css` + Google Fonts.
- Copy follows the campaign guardrails: renting-vs-owning framing (never "stop running ads"), verified case-study numbers only, Brian Dietz as former gym owner / Army vet / BJJ black belt, "school/academy/dojo" terminology, one CTA per page, real territory exclusivity (no fake countdowns).
