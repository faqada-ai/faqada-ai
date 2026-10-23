# FAQADA — CANONICAL BRAND KIT

Status: CANONICAL — compiled Oct 22, 2026 from Mark Rosario's locked brand
standards (MEMORY.md locked creative standards, reaffirmed in the Oct 19, 2026
redesign plan §5 and the Oct 21, 2026 phased-split build handoff) and adopted
as the single brand source at Mark's direction on Oct 23, 2026. Where older
documents disagree with this kit, this kit governs. Machine-readable version:
`brand-tokens.json`. Assets: `assets/`. Canonical home:
`~/workspace/user/brand/faqada-brand-kit/`; mirrored in the Faqada GitHub repo
under `brand/`.

---

## 1. Name, voice of the brand

- **Brand name: Faqada.** The wordmark reads "Faqada" — never "Faqada
  Marketing." *Faqada Marketing LLC* is the legal entity; use it only in legal,
  billing, contract, and footer contexts.
- **Pronunciation: fa-KA-da** (stress on the middle syllable). In TTS/voiceover,
  keep the visible spelling "Faqada."
- **Tagline: "Build with direction."** (period included)
- **Descriptor:** "The business platform for network marketers."
- **Four pillars: Opportunity · Skills · Systems · People.**
- Founder: Mark Rosario. Brand surfaces: faqada.com (authority/revenue hub),
  mark.faqada.com (founder one-pager), app.faqada.com (member platform).
- Copy posture: ambitious in headlines, specific in explanations. Describe real
  actions (practice a skill, plan a follow-up, support a team member). Never
  imply guaranteed income, automatic growth, or fabricated urgency.

## 2. Logo

- **Single master:** angled "F" + "Faqada" wordmark in the cyan→blue→violet
  identity gradient. Official file: `assets/logo/faqada-logo-official.png`
  (transparent PNG, measured 1139×281 px). Source of truth:
  `~/workspace/user/brand/faqada-logo-official.png`.
- **Rules — no exceptions:**
  - Use the official file bytes. Scale only. Never retype the wordmark as
    text, never recolor, redraw, re-space, or rotate it.
  - An all-white variant exists for dark surfaces (per the locked standard);
    no standalone white-variant file is in the local brand folder yet — known
    gap, request it rather than recreating it.
  - Never place text or graphics over the logo. Never stretch or crop it.
  - On mark.faqada.com the Faqada logo appears small in header/footer as the
    company mark. There is **no personal logo** for Mark — do not design one;
    his name is set in Space Grotesk beside his photo.

## 3. Color palette (locked)

| Token    | Hex       | Role                                                        |
|----------|-----------|-------------------------------------------------------------|
| Cobalt   | `#173BB7` | Primary action, links, active states                       |
| Chalk    | `#F7F1E8` | Reading surfaces, warm section band, headlines on dark     |
| Charcoal | `#20252C` | Body type, dark surfaces, dark AI band, footer             |
| Mist     | `#D9DFE9` | Secondary surfaces, borders, dividers, table rules, sublines |
| White    | `#FFFFFF` | Neutral primary surface (pages, cards, app content) — a surface, not a brand color |

No other hex values are authorized. Near-whites like `#FAFAFA`/`#F9F9F9` are
not tokens — one white, one Mist, one Chalk.

### The identity gradient — restricted

`#00E3FF → #087BFC → #714BFF` (cyan → blue → violet).

- **Identity moments ONLY:** the logo, the header rule, section dividers, the
  dark AI band accent, and hero numbers in video stat cards.
- **NEVER** on buttons, body text, form controls, links, or card backgrounds.
- Blue `#087BFC` on its own is a gradient stop, **not** a primary/action color.
  The action color is Cobalt `#173BB7`. (Several legacy systems use #087BFC as
  primary — that is drift, see the audit.)

## 4. Typography (locked)

- **Display: Space Grotesk, weight 700** — headlines, numbers, card titles,
  chapter labels, video headlines and captions.
- **Body: DM Sans, weight 400** (500 for emphasis) — body text, interface,
  sublines, small print.
- Files in this kit (verified with fontTools):
  - `assets/fonts/SpaceGrotesk-Bold.ttf` — internal name "Space Grotesk
    Bold", OS/2 weight **700**. ✔
  - `assets/fonts/DMSans-Regular.ttf` — "DM Sans Regular", weight **400**. ✔
- ⚠️ **FONT FILE TRAP (fixed on the main machine Oct 23, 2026):**
  `~/.fonts/SpaceGrotesk-Bold.ttf` was **mislabeled** — its internal identity
  was *Space Grotesk Light, weight 300*, and it silently corrupted shipped
  graphics (rendered "Bold" was Light — see audit). On Oct 23, 2026 the file
  was replaced with verified Bold 700 bytes and the Light face renamed to
  `SpaceGrotesk-Light.ttf`. Copies on other machines may still be wrong:
  verify any Space Grotesk file's internal name and OS/2 weight before
  trusting its filename.
- **DotGothic16 is retired** (Oct 22, 2026). It was the reference creator's
  typeface, never Faqada's. Do not use it in any Faqada material.

## 5. Video & social application (current standard)

Faqada short-form follows Ajay's (@thevibefounder) **format and methods** with
**Faqada identity** — the format is borrowed, the look is ours:

- Split-screen: host on camera in the bottom ~half; evidence panel on a dark
  field in the top ~half; a new visual beat every 2–4s; the host never
  disappears for long; every spoken claim gets its visual.
- Dark field: **charcoal-cobalt gradient `#0A1120 → #152036`** (Charcoal
  family) — not purple-navy.
- Type in video: Space Grotesk Bold throughout — chapter labels (chapter
  number in cyan `#00E3FF`, words in Mist), headlines in Chalk, caption pill
  (solid deep-navy pill, Space Grotesk Bold white) riding the seam between
  panel and host.
- Designed cards (stat/stack/end cards): brand field, Space Grotesk Bold,
  Chalk headlines, Mist sublines (DM Sans), cyan accents; the identity
  gradient is permitted on hero numbers and the logo only.
- Script grammar: hook in ≤1.5s, short spoken sentences, ~215–249 WPM, no
  dead air, close on one comment CTA. Runtime 35–60s.
- Master: 1080×1920 @30fps, **−14 LUFS integrated, true peak ≤ −0.5 dBTP**,
  deliberate cover (host face + headline) — never the platform default frame.

## 6. Retired / not-the-brand (do not use)

- **Apricot — anywhere.** No apricot exists in the locked palette. A September
  2026 "Cobalt & Apricot" application palette (incl. `#F0C5AB`, `#8B4C36`)
  survives in one superseded repo document. It is not the brand.
- **"Full-Spectrum 2.0"** (repo `brand/2026/`): Inter typography,
  Midnight/Deep Navy palette, tagline "Train smarter. Build faster. Scale
  with AI.", extra logo variants. Not the locked brand; do not pull assets
  or tokens from it.
- **"Clear Blue" Twitter theme** (V2 app): Open Sans, `#087BFC` primary,
  flattened gradient. A documented interim app theme; the Oct 19, 2026 plan
  scopes restoring the locked tokens (RD-01). Do not treat it as brand.
- **Inter / Open Sans** as brand typefaces. Not Faqada's.
- Any logo that is typed, recolored, redrawn, or carries a tagline lockup.

## 7. Do / Don't

**Do**
- Start every design from the tokens in `brand-tokens.json`.
- Use the official logo file; keep the gradient for identity moments.
- Set headlines in Space Grotesk 700, body in DM Sans 400.
- Write "Faqada" (fa-KA-da), tagline "Build with direction."

**Don't**
- Don't invent hex values, near-whites, or new logo variants.
- Don't use DotGothic16, Inter, Open Sans, apricot, or #087BFC as a primary.
- Don't put the gradient on buttons, text, controls, or card backgrounds.
- Don't render "Faqada Marketing" as the brand name or wordmark.
- Don't trust a font file's filename — verify its internal weight.

---

*Compiled by audit, Oct 22, 2026; adopted as canonical at Mark Rosario's
direction, Oct 23, 2026.*
