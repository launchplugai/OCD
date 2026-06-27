# OCD Records — Productize Yourself Blueprint

> Source expertise inferred from this repository: an AI-native music label
> (Neural Ghost roster, tiered sync licensing, studio rental, branded
> release templates). The fields in the original prompt
> ([WHAT DO YOU HELP PEOPLE DO OR BECOME], [PLATFORMS], [HOURS/WEEK]) were
> left blank; this blueprint is grounded in what the repo actually does and
> the assets that already exist on disk.

---

## Your Core Transformation

**I help bedroom AI musicians go from an unreleased folder of generated tracks
to a branded, license-ready catalog generating monthly sync revenue —
using the Entropy Engine™ (Signal → Artifact → License).**

The Entropy Engine maps 1:1 onto the three pillars already shipped on this
site:

| Phase    | What it produces           | Lives on              |
|----------|----------------------------|-----------------------|
| Signal   | Raw obsessive output       | `submit.html` mindset |
| Artifact | Branded artist + release   | `artist.html`, `release.html`, `catalog.html` |
| License  | Tiered, contracted revenue | `licensing.html` (Standard / Premium / Enterprise) |

This is not a generic course. The framework is the literal pipeline OCD
Records uses to ship Neural Ghost, and the deliverable hands that pipeline
to the buyer.

---

## 3 Product Formats

Scored 1–5. Score = average. Rule check: any format requiring live
presence is rejected before scoring.

| Format                                      | Leverage | Feasibility (30d) | Margin | Score |
|---------------------------------------------|----------|-------------------|--------|-------|
| **A. Entropy Engine Toolkit** (digital pack: HTML site templates, licensing contract pack, brand kit, prompt library, release checklist) | 5 | 5 | 5 (~95%) | **5.0** |
| **B. Catalog Auto-Builder** (SaaS — feed it tracks, it spins up artist + release + catalog pages from the OCD templates) | 5 | 2 (auth, hosting, payments, support) | 4 (~80%, infra cost) | 3.7 |
| **C. Sync Licensing Marketplace** (curated drop where buyers license AI tracks; revenue share) | 4 | 2 (cold-start liquidity, legal) | 3 (rev share + ops) | 3.0 |
| ~~D. 1:1 label consulting~~                 | —        | —                 | —      | **REJECTED** — requires live presence |
| ~~E. Cohort-based course~~                  | —        | —                 | —      | **REJECTED** — live calls fail the 3am test |

**Winner: A — Entropy Engine Toolkit.** B is the year-two product; the
toolkit funds and validates demand for it.

---

## Winning Product Structure

**Name:** **Entropy Engine™ — The AI Label-in-a-Box**

**Contents (what ships in the .zip):**

1. **The OCD Method playbook** (PDF, ~40 pp) — the Signal → Artifact →
   License framework with the actual decision rules used to sign Neural
   Ghost.
2. **Site template pack** — copies of `index.html`, `artist.html`,
   `release.html`, `catalog.html`, `licensing.html`, `submit.html` with
   tokens for label name, colors, fonts. Drop in, deploy on Netlify in
   under an hour.
3. **Licensing contract pack** — Standard / Premium / Enterprise tier
   contracts mirroring `licensing.html`, with attorney-review checklist.
4. **Brand identity starter** — the OCD type system (Archivo + Manrope +
   JetBrains Mono), color tokens (`--crimson`, `--electric-blue`), noise
   texture, glass utility classes.
5. **AI-music prompt library** — 50 production prompts for the major
   generators, organized by mood/BPM/use-case (sync-licensing oriented).
6. **Release packaging checklist** — artwork specs, metadata, DSP
   distribution, ISRC, the whole punch-list.
7. **Catalog auto-builder script** — Node CLI that takes a folder of
   tracks + a JSON of metadata and emits a deployable static catalog using
   the templates. (This is the seed for product B.)

**Delivery:** Lemon Squeezy (handles VAT) → instant download +
license-keyed GitHub repo invite for the script. Zero human in the loop.

**Price points:**
- **Lite — $97**: playbook + site templates + prompt library
- **Standard — $497**: everything above + licensing contract pack + brand kit
- **Founder — $1,497** (first 50 only): everything + auto-builder script +
  private Discord (peer-run, not founder-staffed — rule-compliant)

Rationale: $497 anchors against "one paralegal hour to draft your own
licensing tier" ($300+) and "one designer day to brand a label" ($1k+).
Founder tier captures the early-adopter premium without obligating the
operator to show up.

**What makes it irreplaceable:** It is the literal codebase of a working
AI label. Generic "AI music course" sellers cannot ship `licensing.html`
with three working tiers. The moat is the artifacts, not the information.

---

## Distribution Channel

**Existing OCD Records site → new `/method.html` page.**

The site already has the audience surface (catalog, artist profiles,
licensing CTA). Add `method.html` to the nav, frame it as "How we built
this label — get the box," and route checkout through Lemon Squeezy.
Cross-link from `submit.html` ("Not ready to submit? Build your own
label"). No new channel, no audience cold-start, no platform risk.

Secondary: the existing `launchplugai` GitHub org. Publish the
auto-builder script as a public repo with a paywalled
`/templates/premium` folder gated by license key — that's where dev-shaped
buyers find it.

---

## Launch Positioning Statement

> **"OCD Records ships Neural Ghost using the same six files in this
> box — clone the label that's already working."**

---

## Week 1 Build Roadmap

1. **Carve `method.html` from `index.html`.** Above-fold: positioning
   sentence + three-tier price ladder. Below-fold: contents grid (the
   seven items above), social proof from existing catalog stats, FAQ.
   Reuse the `glass-dark`, `hero-glow`, and `font-display` patterns
   already in the site so it ships in-brand same-day.
2. **Bundle the v0 .zip.** Tokenize the six existing HTML files
   (`{{LABEL_NAME}}`, `{{PRIMARY_COLOR}}`, etc.), export the licensing tiers
   as Markdown contracts, write the playbook outline (~20 pp is fine for
   v0). Upload to Lemon Squeezy, wire the webhook.
3. **Ship the launch email + one tweet thread.** Subject: *"We open-sourced
   our label."* Body: positioning sentence, what's inside, founder-tier cap
   at 50. Thread: one tweet per Entropy Engine phase, screenshots from
   `catalog.html`, link to `method.html`. Distribution: existing
   `launchplugai` audience, no new accounts.

---

*Generated by a scheduled routine on 2026-06-27. Refine the inferred
expertise statement, then iterate.*
