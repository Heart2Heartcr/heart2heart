# Heart to Heart — Website

This repo is the public website for **Heart to Heart**, a private, non-medical in-home
care business on Costa Rica's Central Pacific coast. It's built as a favor for the
owner, Felicia, who is **not technical**. She'll eventually make small text edits
herself, so the code must stay simple, readable, and boring in the best way.

---

## ⚠️ Read this first — deploy hygiene

This repo (`Heart2Heartcr/heart2heart`, at `~/Projects/heart2heart`) is served by Netlify
at the **repo root** and deploys on **every push to `main`** — anything committed is
instantly public.

The site is built from source materials that live **outside this repo**, in
`~/Downloads/Heart to Heart/`. That folder also holds the owner's **client PII, financial
records, legal documents, and HR files** (intake forms, emergency contact forms, care
plans, etc.).

- **Never** copy those source materials into this repo. Only finished website assets
  (HTML/CSS/JS, brand images meant to be public) belong here.
- Before any commit, confirm no `.docx`, client form, or financial/legal PDF is staged.
- Keep the repo flat and root-served: `index.html` at the root, one `.html` file per page.

---

## Stack

- Plain **HTML + CSS + minimal vanilla JS**. No framework, no build step, no
  `node_modules`, no bundler.
- Netlify serves the repo root directly. A page is a real `.html` file.
- **Mobile-first.** Most visitors are on phones, at night, worried — an adult child
  researching care for a parent, or a retiree on the coast. Design for the small screen
  first, enhance up.
- Fonts: **Lora** and **Lato** from Google Fonts (both free, SIL OFL). Load only the
  weights in use: Lora 400/500/600, Lato 300/400/700.
- Keep it editable by a non-technical owner: semantic HTML, plain text content that's
  easy to find and change, generous comments near editable copy, no clever abstractions.

---

## What the business is

Private, non-medical **in-home care** — planned under clinical guidance, delivered by
BLS-certified caregivers, and communicated to families with unusual discipline.

Positioning, in one sentence:
> Heart to Heart is private, non-medical in-home care on Costa Rica's Central Pacific
> coast — planned under clinical guidance, delivered by BLS-certified caregivers, and
> communicated to families with a discipline most agencies do not attempt.

The three defensible differentiators — everything on the site supports one of these:
1. **Clinical guidance** — care planning and caregiver training guided by a Registered
   Respiratory Therapist (RRT).
2. **Certified caregivers** — BLS-certified, advanced emergency response training.
3. **Communication** — honest, regular updates to families (the thing families actually
   complain about with other agencies).

### 🚨 Hard compliance rule (outranks every style rule)

Heart to Heart provides **non-medical** care. Nothing on the site may imply nursing,
medical treatment, diagnosis, or clinical judgment about a condition. Caregivers
**observe, document, and report** — they do not assess, treat, manage, or nurse. The RRT
provides **"guidance"** and **"oversight"** on planning/training only — never
"supervision of care" or "medical direction," and she does not provide clinical care to
clients. No stethoscopes, scrubs, clipboards, or hospital imagery (aesthetic *and*
compliance problem).

## Who it serves (four audiences)

The whole site is built around self-segmentation into these four:
1. **Retirees living in Costa Rica** — keep living the retirement they came for.
2. **Adult children living abroad** — the actual decision-makers/bill-payers, not
   physically present. Highest-value audience for paid/referral traffic. They want the
   truth about how their parent really is, without having to ask.
3. **Local Costa Rican families** — nearby but stretched; supplement family involvement,
   don't replace it. (Reduce guilt.)
4. **Healthcare & referral partners** (hospitals, clinics, discharge planners) — B2B,
   more direct/credential-forward tone. Kept one click away, never cluttering the
   family-facing nav.

## Services (5 categories)

- **Daily Living Support** (Personalized Daily Living)
- **Companionship & Lifestyle Support** (Lifestyle & Wellness)
- **Memory & Cognitive Support** — dedicated deep-dive page (dementia/Alzheimer's)
- **Recovery & Transitional Support** — dedicated deep-dive page (post-hospital,
  post-illness); urgency-appropriate CTA ("Request a Same-Week Consultation")
- **Family Communication & Updates** (Family Peace of Mind)

---

## Site map

Primary nav is intentionally narrow (6 clusters) + a persistent CTA button. A quiet
utility bar sits above it (phone click-to-call · WhatsApp · "For Referral Partners").

- **Home**
- **About** (dropdown): About Heart to Heart · Meet Felicia · Our Care Philosophy · Why Choose Heart to Heart
- **Services** (dropdown): Services Overview · Memory & Cognitive Support · Recovery & Transitional Support
- **What Care Looks Like** (standalone — the site's most emotional/shareable page: Morning / Afternoon / Evening vignettes)
- **For Families** (dropdown): For Families Abroad · For Local Families
- **Resources** (Life in Costa Rica hub + articles)
- Persistent CTA button: **"Schedule a Complimentary Consultation"**

Full page list (16): Home · About · Meet Felicia · Our Care Philosophy · Services
Overview · Memory & Cognitive Support · Recovery & Transitional Support · What Care
Looks Like · For Families Abroad · For Local Families · Why Choose Heart to Heart · For
Healthcare & Referral Partners · Life in Costa Rica Resources (hub + articles) · FAQ ·
Contact · Privacy Policy / Terms.

Every path (header button, page CTAs, footer) leads to the **same** short inquiry form +
the **same** phone/WhatsApp options. Consistency > customization on the ask.

Suggested build order (start small, ship early): Home → Contact → About/Meet Felicia →
Services Overview → the two service deep-dives → What Care Looks Like → the two Families
pages → Why Choose → Referral Partners → FAQ → Resources.

---

## Brand: Coastal Luxe identity system

Feel: closer to a **Four Seasons / Auberge** property page than a home-care agency. Quiet
confidence, not urgency. Photography over icons. Full sentences over bullet-point task
lists. Generous white space. Nothing should feel "medical." Three instincts override
everything: **show a life, not a service** · **slow the page down** · **never rush the ask.**

### Colors (Coastal Luxe palette)

| Token | Hex | Use |
|---|---|---|
| Deep Harbor | `#0F3B4C` | Primary. Headlines, header/footer bands, the mark. |
| Harbor Deep | `#0A2B37` | Shadow tone. Footer sub-bands, hover states. |
| Tidewater | `#2C7A8C` | Secondary. Eyebrows, subheads, links, small emphasis on light. |
| Tidewater Light | `#7CA8B2` | Secondary text on dark grounds ONLY (fails contrast on light). |
| Seafoam Mist | `#DDE9EB` | Callout / info-block fill ("operational note"). |
| Warm Sand | `#EFE6D9` | Section rules, numerals, structural detail on light. |
| Sand Wash | `#F7F2EA` | Large tinted areas — alternating web sections. |
| Ivory | `#FCFAF7` | Page background. **Never pure white** — reads cold. |
| Coral Signal | `#C0574F` | Accent: heartmark bullets, primary buttons, single rules. **Ceiling 5% of any surface** — scarcity is its power. |
| Soft Gold | `#C2A462` | Rules under headings, band edges. Detail only, never fills. |
| Ink | `#232A2E` | Body copy on light. |
| Ink Mid | `#55636A` | Secondary / descriptive copy. |

Proportion target: ~60% ivory/sand, ~30% deep harbor, ~6% tidewater/mist, ~4% coral/gold.
If a layout feels cheap, it's almost always too much coral or too little ivory.

### Typography

- **Lora** (serif) carries the voice: every headline, the brand line, pull quotes.
  Never set body copy in Lora.
- **Lato** (sans) carries the information: body, eyebrows, labels, buttons. Never set a
  headline in Lato. This division of labour is the whole system.
- Web font stacks: `"Lora", Georgia, serif` and `"Lato", "Helvetica Neue", Arial, sans-serif`.
- Sentence case for headlines. Full caps only for eyebrows/labels, always with letter-spacing.
- Ragged right everywhere (never justified). Body measure 45–75 characters.

### Layout language

- One idea per horizontal band; alternate grounds (harbor / sand / ivory). A reader
  should skim the bands alone and follow the argument.
- Rules do the work borders would: a gold hairline under H2s, a sand hairline between
  list items. **No boxes, no drop shadows, no rounded cards.**
- Left-aligned by default; center only inside contained blocks (hero, contact panel).
- Section order house rule for every page: **Feeling → Understanding → Trust → Action.**
  Emotional/human content first, proof/credentials second, logistics (forms/FAQ) last.
- Mobile: header CTA becomes a sticky bottom bar with **Call · WhatsApp · Schedule**
  (thumb-reachable). Click-to-call and click-to-WhatsApp are primary conversion paths.

### The mark / logo

- The mark is the wave-and-heart symbol (`Print materials/Heart to Heart logo.png`).
  On light grounds use the Deep Harbor monochrome treatment; ivory/white reverse on dark.
- ⚠️ The current logo PNG carries the tagline **"Care that feels like family"** — this is
  **off-brand and retired.** The brand guide explicitly bans "we treat every client like
  family" language and the old line "Companion Care You Can Trust." **Do not put that
  tagline on the site.** Use the brand line instead (below). Ideally get a clean logo file
  without the tagline; the current file is a soft-edged raster.

### Brand line (three separate sentences, never a run-on)

> **Compassionate Care. Professional Standards. Peace of Mind.**
> ES: *Cuidado Compasivo. Estándares Profesionales. Tranquilidad.*

"Peace of Mind" always lands last. Separate the three with a small coral heartmark in
horizontal lockups. In Spanish use "Tranquilidad" (never "Paz Mental").

## Voice & tone

- **Specific, not sentimental.** "A change in appetite. A change in gait. A change in
  breathing." — not "we care deeply about your loved one."
- **Benefit before task.** Dignity before bathing. Independence before transportation.
  Confidence before medication reminders.
- **Short declaratives.** Confidence reads as short sentences; long hedged ones read as
  fear.
- **Warm through precision, not adjectives.** Cut "loving," "caring," "passionate."
- **Write about a person, not a patient.** "your mother," "the person," "our client" —
  never "the elderly," "sufferers," "victims of dementia."
- **Trust is cumulative, never asserted.** No page says "trust us"; specifics do the work.

**Do-not-use list:** companion care you can trust · loved ones · golden years · aging
gracefully · here to help · we treat every client like family · caring hearts · angels ·
second family · quality care at affordable rates · we go above and beyond.

## Photography

Until a real shoot is commissioned, **run layouts without photos** — they're designed to
stand alone, and empty photo boxes are worse than none. **No stock imagery** on hero,
covers, or key pages (fastest way to look cheap). When real photos exist: real homes on
this coast, available light, caregiver and client at the same eye level doing something
real, hands/doorways/shared tables. Never: stethoscopes/scrubs/clipboards, exaggerated
smiles/thumbs-up, or any photo taken during personal care. Signed written consent before
any client photo, always.

## Bilingual (future)

English first; a Spanish (Costa Rican, *usted*) version is planned. Keep copy in a
structure that's easy to duplicate per-language later. Company name stays "Heart to
Heart" in both; only the descriptor translates (IN-HOME CARE → CUIDADO EN EL HOGAR).

---

## Business facts (for footer / contact / SEO)

- **Name:** Heart to Heart
- **Type:** Service-area business (in-home; **no public street address** — caregivers go
  to the client)
- **Service area:** Garabito, Jacó, Playa Hermosa, Herradura, Punta Leona, Esterillos,
  Puntarenas, and surrounding Central Pacific communities
- **Phone / WhatsApp:** +506 8828-1934
- **Email:** heart2heartcr@gmail.com
- **Domain:** www.heart2heartcr.com
- **Google category:** Home Care Service
- **Founder:** Felicia
- Note the correct spelling **Garabito** (an earlier brochure had "Grarabito"); watch
  apostrophes on "Alzheimer's" / "Parkinson's."

---

## Source materials (outside the repo, in `~/Downloads/Heart to Heart/`, NOT for deploy)

- `Start Here/Heart-to-Heart-Brand-and-Production-Guide.pdf` — full brand system (colors,
  type, logo, voice, photography).
- `Start Here/H2H master messaging copy library.pdf` (and `.docx`) — **the definitive
  approved copy source**: 25 homepage headlines, 50 supporting headlines, CTAs, value
  props, services messaging, What Care Looks Like vignettes, founder story, FAQ (30 Qs),
  microcopy. Pull page copy from here — it's finished, not a starting point.
- `Website/H2H website strategy final.pdf` — the full UX blueprint this summary condenses
  (per-page goals, objections, layout concepts, conversion framework).
- `Print materials/Heart to Heart logo.png` — logo (see tagline warning above).
- `Google Business/…` — business info, service area, launch copy.
