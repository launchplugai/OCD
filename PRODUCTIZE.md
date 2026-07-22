# OCD Records — Productize Yourself Blueprint

> Applied to OCD Records: the brand, the catalog, the submission funnel.
> Framework prompt scheduled 2026-07-22; user-info placeholders were empty,
> so this document infers the "expertise" from the live project — a
> curated underground record label whose current site already supports
> catalog browsing, artist profiles, releases, licensing, and submissions.

---

## Your Core Transformation

I help **obsessive underground music-makers** go from
**unheard tracks stuck on hard drives and ignored A&R inboxes**
→ to **catalog-signed artists earning sync/licensing revenue with a real brand identity**,
using the **OCD Signal → Signed → Synced** pipeline.

The three stages are the proprietary methodology:

1. **Signal** — an objective, label-grade verdict on a track (rubric-scored).
2. **Signed** — a curation path from top scores into the OCD catalog.
3. **Synced** — packaging catalog work for licensing / sync placement revenue.

---

## 3 Product Formats

| Format | What it is | Leverage (sells without me) | Feasibility (30 days) | Margin (>70%) | Score /15 |
|---|---|---|---|---|---|
| **Signal Score** (tool) | Self-serve web app that grades a submitted track against the OCD rubric and returns a written verdict + submission-ready package | 5 — pure SaaS, evaluator runs unattended | 4 — rubric + form + Stripe + LLM/audio-analysis backend; achievable, some engineering | 5 — software, ~90% margin | **14** |
| **Artist Vault** (digital product) | Static bundle: OCD's submission checklist, mix-reference pack, one-sheet template, licensing-ready metadata guide | 5 — file delivery, zero touch | 5 — writing + design only, ships in a week | 5 — one-time cost, ~95% margin | **15** |
| **Signed Circle** (community) | Paid tier for artists who scored above threshold: monthly A&R AMA recordings, private catalog previews, sync-brief drops | 3 — needs periodic new content, some curation | 3 — needs community platform + first cohort seeding | 4 — subscription, ~80% margin | **10** |

Feasibility-weighted winner: **Artist Vault**.
Moat-weighted winner: **Signal Score**.

**Winning choice: Signal Score.** Vault is easier but commoditizable in a week by any competitor. Signal Score is the defensible engine — it also becomes the top-of-funnel that filters into Vault upsell and Signed Circle later. It fails no rule: runs at 3 AM, uses a named framework (OCD Rubric v1), and rides the existing site.

---

## Winning Product Structure

- **Name:** **Signal Score by OCD** — powered by the **OCD Rubric v1** (10 weighted criteria across composition, sonic identity, mix integrity, release-readiness).
- **Contents:**
  - Upload flow accepting audio + genre tag + intent (release / license / feedback).
  - Automated evaluation returning:
    - A single 0–100 **Signal Score**.
    - Per-criterion breakdown with 1–2 sentence rationale each.
    - A written verdict (Reject / Refine / Ready-to-submit / Fast-track).
    - A generated **Submission Package** (one-sheet, metadata JSON, cover-art brief) when score ≥ 70.
  - Public "Signal Score" badge the artist can embed on socials / Bandcamp / SoundCloud.
- **Delivery:** Web app hosted at `ocdrecords.com/signal`. Stripe checkout, no human in the loop. Verdict emailed as PDF + dashboard link within 5 minutes. Free tier: 1 evaluation, watermarked. Paid: unlimited within plan.
- **Price point:**
  - **$29** per single-track evaluation (impulse-priced under the cost of a mixing session).
  - **$99 / month** unlimited (target: producers iterating on releases).
  - Rationale: sits below "pay a real A&R for feedback" ($200+) and above "free Discord critique" (worthless-signal); anchors OCD as the objective standard.
- **What makes it irreplaceable:** The rubric is *the same one* used to greenlight the OCD catalog. Every score is trainable evidence that OCD signs on — so passing the Score is not a vanity metric, it's a real submission shortlist ticket. Competitors can copy the tool; they cannot copy the label.

---

## Distribution Channel

**The existing OCD Records website — specifically the `/submit` page.**

Every artist already landing on `submit.html` today is the exact ICP. Instead of "fill this form and wait weeks," the CTA becomes "Get your Signal Score in 5 minutes — if you're above 70, you skip the queue." This converts existing (currently unmonetized) submission traffic into paid usage with zero new-channel risk. No new audience to build, no new algorithm to court.

Secondary organic amplifier: the shareable **Signal Score badge** — artists who score well post it, which drives inbound to the tool.

---

## Launch Positioning Statement

> **"Get a label-grade verdict on your track in 5 minutes — using the same rubric OCD Records uses to sign its catalog."**

---

## Week 1 Build Roadmap

1. **Lock the Rubric v1.** Write the 10 criteria + weights + scoring anchors in a single markdown file (`rubric.md`). This is the moat — no code until it exists.
2. **Ship the landing page + waitlist at `/signal`.** Static HTML in the existing OCD site style; Stripe payment link for a $29 "Founding Score" pre-order; capture email + genre.
3. **Wire the intake pipeline.** File upload (S3 or similar) → email trigger → manual scoring for the first 20 orders. Manual scoring is the on-ramp: it validates the rubric against real submissions before any automation, and every scored track becomes labeled training data for v2.
