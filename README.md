# The RLVNT Edit — Site

Static editorial landing page for **The RLVNT Edit** (rlvntedit.com), an editorial property of 1982 Media LLC.

## Purpose

This site exists to:

1. Serve as the credible, professional landing URL paste-able into affiliate program applications (AWIN, Impact, CJ, Partnerize, etc.) to demonstrate legitimacy of The RLVNT Edit as a real editorial publication.
2. House the publication's editorial mission, what we cover, how we operate, and the operator's background.
3. Carry the legal surface (FTC affiliate disclosure, privacy policy, terms of use) that affiliate networks require to approve a publisher.
4. Direct readers to the active Pinterest channel where The Edit currently publishes (`pinterest.com/RlvntEdit`).
5. Eventually become the long-form web edition of The Edit (Q3 2026).

## Brand stack (locked — do not drift)

- **Customer-facing brand:** The RLVNT Edit (typographic mark: `THE RLVNT EDIT`)
- **Sister B2B brand:** RLVNT MEDIA (not this site)
- **Holding company:** 1982 Media LLC
- **Old Money palette:** Cream `#F0EEE5`, Cream-2 `#E5E1D3`, Ink `#2C2622`, Burgundy `#5B1A1F`, Taupe `#B5B0A6`, Moss `#5F6A4F`
- **Recommended ratio:** 70% cream backgrounds / 22% ink text / 8% burgundy accent
- **Typography:** Playfair Display (serif headlines, italic emphasis) + Inter (sans body)
- **Aesthetic reference:** Wirecutter × The Strategist × Kinfolk × Cereal Magazine. Slow editorial. Generous whitespace. Single-column long-form when appropriate.

## File structure

```
rlvnt-edit-site/
├── index.html        — landing page (hero, philosophy, coverage, about, footer)
├── disclosure.html   — FTC affiliate disclosure
├── privacy.html      — privacy policy
├── terms.html        — terms of use
├── styles.css        — all styles, brand-locked
├── images/           — brand assets (favicons, lockup, OG share image)
└── README.md         — this file
```

## Deploy

### Replit
1. Create a new Static HTML repl
2. Drag the contents of this folder in
3. Run → page serves at the auto-generated `.replit.app` URL
4. Custom domain: in repl settings, point `rlvntedit.com` to the deployment

### Vercel / Netlify / GitHub Pages
This is a static site — drop the folder into any static host. No build step.

## Edit guidance

When updating copy or adding sections:

- Headlines: Playfair Display, 500 weight, italic burgundy for emphasis
- Body: Inter, 400 weight, ink color
- Section eyebrows: small caps, burgundy, letter-spaced
- Pull quotes: Playfair italic, burgundy, left burgundy hairline rule
- Never use red — use burgundy `#5B1A1F`
- Cream sections alternate with cream-2 for subtle rhythm
- One dark (ink) section per page max — currently "How We Operate"

## Reference: canonical brand docs

The full brand pack and decision history lives in the affiliate engine repo:

- `~/1982-Media/rlvnt-pinterest-affiliate-engine/docs/brand_assets/Brand Tokens.md` — palette + type tokens
- `~/1982-Media/rlvnt-pinterest-affiliate-engine/docs/decision_log.md` — Decisions #43, #44 (rebrand)
- `~/1982-Media/rlvnt-pinterest-affiliate-engine/docs/affiliate_apps_round_2.md` — current positioning copy

## Status

- Built: 2026-05-17
- Live URL: pending Replit deploy + DNS for `rlvntedit.com`
- Owner: Abby Buchmiller (`abby@rlvnt.media`)
