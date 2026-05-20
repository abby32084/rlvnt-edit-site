# Replit Deployment Prompt — The RLVNT Edit Site

## How to use this

You have two paths. Pick whichever is faster for you.

---

## Path A — Drop-in deploy (fastest, ~5 minutes)

1. Go to replit.com → **Create Repl** → choose **Static HTML, CSS, JS** template
2. Name it: `rlvnt-edit-site`
3. Delete the placeholder `index.html` and `style.css` Replit auto-creates
4. Drag the entire contents of `~/1982-Media/rlvnt-edit-site/` into the file panel:
   - `index.html`
   - `styles.css`
   - `disclosure.html`
   - `privacy.html`
   - `terms.html`
   - `images/` folder
   - `README.md`
5. Hit **Run** → preview at the `.replit.app` URL
6. Settings → Domains → add `rlvntedit.com` (point DNS A/CNAME per Replit's instructions)
7. Done. Use `https://rlvntedit.com` as the promotional website in every affiliate application.

---

## Path B — Replit Agent prompt (if you'd rather have Replit build it from scratch with iteration capability)

Paste this exact prompt into a new **Replit Agent** session:

```
Build a static editorial landing page for "The RLVNT Edit" — an editorial
curation property of 1982 Media LLC. This is the public-facing site that
will serve as our promotional URL on affiliate program applications (AWIN,
Impact, CJ Affiliate, Partnerize), so it must read as a real, professional
editorial publication — NOT a "coming soon" placeholder.

DEPLOYMENT
- Single static site, no backend. HTML + CSS only. No JavaScript framework.
- Pages: index.html (landing), disclosure.html, privacy.html, terms.html.
- Will deploy to rlvntedit.com via Replit's custom domain feature.

BRAND (locked — do not invent variations)
- Customer-facing name: The RLVNT Edit
- Typographic mark: "THE RLVNT EDIT" with "THE" set as Playfair Display italic in burgundy, "RLVNT EDIT" set as Playfair Display 600-weight, letter-spaced 0.18em
- Holding company referenced in footer + about: 1982 Media LLC
- Sister brand mentioned once in About: RLVNT MEDIA (B2B services)
- Operator: Abby Buchmiller, founder/editor

PALETTE (Old Money — locked)
- Cream #F0EEE5 (primary background, 70% of page)
- Cream-2 #E5E1D3 (alternating section background for rhythm)
- Ink #2C2622 (primary text, 22% — also used for one dark "How We Operate" section)
- Burgundy #5B1A1F (accent, 8% — eyebrows, emphasis, hover states)
- Taupe #B5B0A6 (subtle borders/dividers)
- Moss #5F6A4F (reserved, not used in this build)

TYPOGRAPHY
- Headlines: Playfair Display (load 400/500/600/700 + italic 400/600 from Google Fonts)
- Body: Inter (load 300/400/500/600 from Google Fonts)
- Section eyebrows: Inter 500 weight, small caps, letter-spacing 0.22em, burgundy
- Italic emphasis inside headlines: burgundy

REFERENCE AESTHETIC
- Wirecutter × The Strategist × Kinfolk × Cereal Magazine
- Slow editorial, generous whitespace, single-column where appropriate
- Two-column for "philosophy" + "how we operate" + "about" sections (label on left, body on right)
- One dark section ("How We Operate") on cream-inverted ink background

PAGE STRUCTURE (index.html)

1. STICKY TOP BAR
   - Mark on left (THE RLVNT EDIT)
   - Nav links: Philosophy / What We Cover / How We Operate / About / "Read on Pinterest →" (CTA button, dark)

2. HERO (cream background, ~80vh)
   - Eyebrow: "Vol. I · Issue 001 · An editorial property of 1982 Media LLC"
   - Headline (Playfair, 5xl): "One considered purchase / over ten impulsive ones." (second line italic + burgundy)
   - Lede: "The RLVNT Edit is an editorial standard for high-end home and lifestyle objects worth keeping — premium outdoor, mattresses, home gym, kitchen, and considered decor. We write about the things after we've lived with them. We're not first. We're considered."
   - Primary CTA button: "Read the current Edit on Pinterest →" → https://pinterest.com/RlvntEdit
   - Secondary text: "Long-form web edition · Q3 2026"

3. PHILOSOPHY (two-column, cream)
   - Left: eyebrow "The Philosophy" + h2 "We earn our recommendation, or we don't make one."
   - Right: 3-4 paragraphs articulating the slow-editorial mission
   - Pull quote at end: "We're not first. We're considered." (Playfair italic, burgundy)

4. WHAT THE EDIT ISN'T (cream-2 background, centered)
   - Eyebrow: "What The Edit Isn't"
   - Grid of 5 items each prefixed with × in burgundy:
     - "A listicle."
     - "An affiliate farm."
     - "A daily content treadmill."
     - "A brand-partnership ad vehicle."
     - "A review of things we haven't lived with."

5. WHAT WE COVER (cream)
   - Eyebrow + h2: "Five categories. One bar."
   - Grid of 5 coverage cards:
     - 01 Premium Outdoor & Hosting
     - 02 Mattresses & Rest (covered: Saatva · Glacier)
     - 03 Home Gym (in development)
     - 04 Premium Kitchen (in development)
     - 05 Considered Home Decor (in development)
   - Each card: serif-italic numeral, h3 category name, short paragraph, small-caps burgundy "Currently covering: [brands]" line

6. HOW WE OPERATE (dark — ink background, cream text)
   - Eyebrow: "How We Operate"
   - h2: "AI as the production layer. / Human editorial taste as the output standard." (second line italic)
   - Right column: 1-2 paragraphs + stack list
     - Higgsfield Soul Location — moody editorial scene generation
     - Custom HTML/CSS + Playwright — pin design consistency at scale
     - Zernio — multi-platform distribution layer
     - Claude (Anthropic) — strategy iteration, voice consistency
     - Human curatorial judgment — on every product, every pin, every list
   - Pull quote: "Volume *and* quality — not volume *versus* quality."

7. CURRENT EDIT / PINTEREST (cream, centered)
   - Eyebrow: "The Current Edit"
   - h2: "Read on Pinterest."
   - Short lede about the 40+ pins / 5 boards
   - CTA: "pinterest.com/RlvntEdit →"

8. ABOUT (cream-2, two-column)
   - Left: eyebrow "About" + h2 "An editorial property of 1982 Media LLC."
   - Right: 2 paragraphs introducing Abby Buchmiller (founder/editor, previously co-founded a $250M+ solar services company with 500+ employees, two decades of operating instinct, etc.)
   - Family block listing: 1982 Media LLC, RLVNT MEDIA, The RLVNT Edit, Abby Buchmiller (abbybuchmiller.com)

9. FOOTER (ink background, cream text, 4 columns)
   - Col 1: Mark + tagline
   - Col 2: Contact (abby@rlvnt.media + pinterest link)
   - Col 3: Legal (Affiliate Disclosure, Privacy, Terms)
   - Col 4: Family (1982 Media LLC, RLVNT MEDIA, Abby Buchmiller)
   - Bottom bar: copyright + the affiliate disclosure paragraph

LEGAL PAGES
Build out three legal pages with the same topbar + footer chrome. Content should be production-ready FTC-compliant copy:
- disclosure.html — affiliate disclosure (mentions Amazon Associates, Partnerize, Impact, CJ, AWIN, direct merchants; affirms editorial independence from commission rates)
- privacy.html — minimum viable privacy policy (aggregate analytics, voluntary email collection, third-party services list, GDPR/CCPA contact line)
- terms.html — minimum viable terms of use (editorial-content disclaimer, affiliate-relationships pointer to disclosure, IP, external links, limitation of liability)

ACCESSIBILITY + SEO
- Semantic HTML5 elements (header, section, article, footer)
- All images need alt text
- Open Graph + Twitter card meta tags on index.html
- Sensible page titles + meta descriptions on each page
- Mobile-responsive (single-column under 820px width)

NO
- No JavaScript framework
- No build step
- No tracking pixels beyond standard analytics (we'll add Plausible/Fathom later)
- No "coming soon" or "notify me at launch" framing — this site goes live as a real publication
- No animations beyond subtle hover transitions
```

---

## After deploy

Once `rlvntedit.com` is live (whichever path you used):

1. Update all affiliate application bios to reference `rlvntedit.com` instead of `abbybuchmiller.com` as the primary promotional URL
2. Add the site URL to your Pinterest profile bio
3. Add a `rlvntedit.com` mention in the engine's `CLAUDE.md` identity-stack reference
4. Send the URL to me for a once-over before pasting into any application
