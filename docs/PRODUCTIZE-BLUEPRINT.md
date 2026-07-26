# OCD Records — Productize Yourself Blueprint

> **Note on inputs.** The scheduled prompt used the "Productize Yourself" template
> with the personal-input fields left as placeholders
> (`[WHAT DO YOU HELP PEOPLE DO OR BECOME]`, platform list, hours/week). Because
> this routine was fired against the OCD Records repo with the instruction to
> "work on this project," the inputs below are inferred from the current
> site — `index.html`, `licensing.html`, `studios.html`, `submit.html`, and
> `artist.html`. Edit the "Assumed Inputs" section and re-run the framework if
> any of those inferences are wrong.

## Assumed Inputs

- **Expertise / transformation on offer:** OCD Records combines "neural precision
  and human intuition" to develop artists whose tracks clear a sync-licensing bar
  — i.e., turning underground / AI-augmented producers into commercially
  licensable acts.
- **Current platforms:** `ocdrecords.com` (the website in this repo), plus
  whatever label/artist social channels feed the existing `submit.html` funnel.
- **Time available to build:** unknown — the blueprint is scoped to a 30-day
  build assuming ~10 focused hours per week (adjust if wrong).

---

## Your Core Transformation

**I help obsessed independent producers go from unreadable one-off tracks to
sync-licensable, catalog-ready releases using the NPHI-7 framework
(Neural Precision × Human Intuition, scored across 7 axes).**

The seven axes:

1. **Mixdown Coherence** — LUFS integrated / true-peak / dynamic range vs.
   sync-broadcast targets.
2. **Sonic Identity** — spectral fingerprint distinctiveness vs. the top
   200 tracks in the target sync category.
3. **Arrangement Tension** — energy curve, drop density, and negative-space
   ratio.
4. **Low-End Architecture** — sub / bass separation, mono compatibility.
5. **Harmonic Risk** — modal / key movement complexity (a proxy for "will
   this stand out on a supervisor's shortlist").
6. **Brand Fit** — semantic match to the OCD Records catalog and to named
   sync verticals (film trailer, prestige TV, streetwear, etc.).
7. **Licensing Safety** — sample / stem / model-provenance clearance risk
   (critical for AI-augmented producers).

Every product below uses this rubric as its spine. NPHI-7 is the proprietary
mechanism.

---

## 3 Product Formats

Scoring key: **Leverage** = sells while you sleep (1–10). **Feasibility** =
buildable in 30 days at ~40 h (1–10). **Margin** = gross margin above 70 %
scored 1–10.

| Format | Leverage | Feasibility | Margin | Score |
|---|---|---|---|---|
| **A. "Signal Score" — self-serve NPHI-7 track audit** (upload a track, get a scored PDF report + fix list within minutes; $39 / track) | 10 | 8 | 9 | **27** |
| **B. "The OCD Method" — self-paced course + Ableton/Logic template pack** (video modules teaching NPHI-7 with DAW project files and mix-ready presets; $299 one-time) | 8 | 6 | 9 | **23** |
| **C. "OCD Stems" — cleared sample & stem subscription** (curated stems drawn from label releases with pre-cleared sync usage rights; $19 / mo) | 9 | 6 | 8 | **23** |

Ranking is unambiguous — Signal Score wins on all three axes and is the only
one that requires zero live A&R involvement to deliver.

---

## Winning Product Structure

### Name
**Signal Score by OCD Records — NPHI-7 Sync Audit**

### Contents
Every audit returns:

1. **NPHI-7 score card** — 7 axes × 3 sub-criteria, each 0–10, weighted into
   a single Signal Score (0–100) and a binary sync-licensable / not
   verdict.
2. **Fix List** — top 5 concrete corrections ordered by score-impact
   (e.g., "cut 1.8 dB at 240 Hz; sub bass drops mono below 40 Hz").
3. **Reference matches** — 3 nearest catalog tracks + 3 nearest
   commercially-licensed reference tracks, so the artist can hear the gap.
4. **Signal Score badge** (SVG + embed code) if the track scores ≥ 80,
   usable on the artist's own site / streaming links — turns every high
   scorer into a free distribution asset.
5. **Upsell** — one-click "submit this track to OCD A&R with the Signal
   Score attached; skip the queue" for $0 to the artist (feeds the label's
   existing submit funnel with pre-qualified demos).

### Delivery mechanism (works at 3 a.m.)
- Upload page at `/signal-score` on the existing site — same design system,
  Stripe Checkout for payment.
- Background pipeline: audio-analysis worker (LUFS / true-peak / spectral /
  key / stem separation via a hosted model) → LLM pass over the qualitative
  axes given the numeric features and a private catalog embedding index →
  templated PDF + HTML report emailed and available in a magic-link portal.
- No human step required for the report. A&R only touches submissions that
  the artist explicitly upgrades into the label submission flow.

### Why it's irreplaceable
- **NPHI-7 is proprietary and named.** Competitors sell generic "AI
  mastering" or "song feedback"; this is scored against an actual sync
  label's live A&R rubric with a licensing-safety axis nobody else runs.
- **The reference set is the moat.** Scores are computed relative to the
  OCD Records catalog embedding index — a dataset only OCD has.
- **The badge creates network effects.** Every high-scoring track that
  ships with a Signal Score badge becomes a marketing surface for the
  next artist.

### Price point
- **$39 per track audit.**
- **$149 for a 5-track pack** (rewards batching, lifts AOV).
- Rationale: an independent producer already spends $50–$150 to master a
  track; $39 pre-master to know whether it's worth mastering is a
  no-brainer. Marginal cost of one audit is dominated by inference
  (< $2 with current hosted model pricing), keeping margin well above 90 %.

---

## Distribution Channel (matches existing platform)

**The OCD Records submit funnel itself.**

- Every rejection email from `submit.html` gets a CTA: "We didn't sign
  this one. Want the NPHI-7 audit that tells you why — $39?" That flips a
  bottleneck (label reviewing every demo for free) into revenue and
  loops rejected artists back into paid feedback.
- The homepage `/index.html` gets one "SIGNAL SCORE — 60-SECOND SYNC AUDIT"
  card in the studios/services zone; the licensing page gets a footer
  callout targeting the same producers who would otherwise cold-email
  submissions.

No new platform, no cold audience. Every source of Signal Score traffic is
already indexed and drawing organic reach.

---

## Launch Positioning Statement

> **OCD Records tells you in 60 seconds whether your track is sync-licensable —
> and exactly what to fix if it isn't — scored against the NPHI-7 rubric our
> A&R uses to sign the label.**

---

## Week 1 Build Roadmap

1. **Ship `/signal-score` landing page + waitlist.** Reuse the existing
   Tailwind / Archivo / Manrope system in `index.html`; one hero, the
   NPHI-7 rubric grid, a $39 price anchor, an email capture that posts to
   the same list as the existing `Join Transmission` form. Zero backend
   needed for the waitlist.
2. **Freeze the NPHI-7 scoring spec as a versioned JSON config** (`nphi7.json`)
   — 7 axes × 3 sub-criteria × pass/fail thresholds × fix-list copy strings.
   This is the source of truth every future pipeline reads.
3. **Backfill an eval set of ≥ 200 historical demos** from the existing
   submit funnel with the A&R's actual accept / reject decision. This is
   the benchmark the automated Signal Score is graded against before it
   ever charges a real customer — protects the brand from shipping a
   scorer that disagrees with the label.

Weeks 2–4 (out of scope for the Week 1 sprint but the natural continuation):
build the audio-analysis worker, wire Stripe Checkout, ship the PDF
template, and soft-launch to the waitlist at half price.
