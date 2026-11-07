# OCD Records — Productize Yourself Blueprint

> Living document. Each scheduled refinement updates this file.
> Inputs for the three bracketed fields were inferred from the current site
> (index.html, submit.html, licensing.html, artist.html, catalog.html).
> Override them in the "Inputs" block below to re-anchor the next refinement.

## Inputs (editable — drives the rest)

- **Expertise / transformation:** A&R curation + licensing-ready packaging for
  experimental electronic artists. The "obsession-becomes-art" filter that
  turns raw demos into release-grade, sync-licensable artifacts.
- **Current platforms:** ocdrecords.com (catalog, release, artist, submit,
  licensing, studios pages already shipped), plus whatever social accounts
  drive the existing submissions pipeline.
- **Time available to build:** ~10 hrs/week (default — adjust).

---

## Your Core Transformation

> I help **independent electronic artists** go from **"finished track, no
> label traction, no sync revenue"** to **"catalog-signed release with a
> licensing tier that earns while they sleep"** using the **OCD Signal Filter™**
> — a 7-point obsession-grade scoring rubric (sonic identity, arrangement
> discipline, mix tolerance, licensing fit, visual coherence, release
> readiness, catalog neighbor density) that decides what ships, how it's
> packaged, and which tier it enters.

The named mechanism is the **Signal Filter** — it is the proprietary IP,
not the label itself. The label is one application of the filter; the
product is the filter.

---

## 3 Product Formats

Scoring is 1–5 per axis, summed. Leverage = sells without me. Feasibility
= buildable in 30 days with ~10 hrs/wk. Margin = gross margin after
delivery costs.

| Format | Leverage | Feasibility | Margin | Total |
|---|---|---|---|---|
| **A. Signal Filter Scorecard (self-serve demo audit tool)** | 5 | 4 | 5 | **14** |
| **B. Release Operating System (digital product — templates, stems-to-license pipeline, Notion/PDF)** | 4 | 5 | 5 | **14** |
| **C. Catalog Collective (gated community + quarterly comp drop)** | 3 | 3 | 4 | **10** |

Rejected on sight:
- 1:1 A&R consulting (requires live presence — fails the test)
- Generic "how to run a label" course (no named framework — fails the rules)

**Winner:** Format A — **Signal Filter Scorecard**. Highest leverage
(fully automated), fastest to build on top of the existing site, and the
margin is near-100% once the rubric is encoded. It also feeds Format B
naturally: a low score produces a specific upsell to the Release OS.

---

## Winning Product Structure

- **Name:** **OCD Signal Filter™ — Instant Demo Audit**
- **Contents:**
  - Upload a track + 3 metadata fields (BPM, genre tag, intended use case).
  - Automated scoring across the 7 Signal Filter axes with a 1–5 per axis
    and a weighted total.
  - A one-page PDF verdict: **SIGNAL / NOISE / RE-RECORD**, with the two
    weakest axes called out and a specific remediation per axis.
  - A gated offer at the end: SIGNAL → submit to the catalog with a
    pre-filled submission (routes into submit.html). NOISE / RE-RECORD →
    buy the Release OS (Format B) at a one-click discount.
- **Delivery:** Web form on ocdrecords.com (`/signal-filter`), scoring
  runs server-side or via a serverless function; PDF generated and
  emailed. Zero human touch. Works at 3am.
- **What makes it irreplaceable:** The rubric is calibrated against the
  actual OCD catalog — every scoring axis is anchored to a named release
  on the site as a "5." Competitors can mimic a scorecard; they can't
  mimic the catalog it was trained on.
- **Price point:** **$29 one-time** (audit), **$149 one-time** (Release
  OS upsell). Rationale: $29 is below the "I need to think about it"
  threshold for a working artist; the Release OS price matches a single
  mastering session — a known, accepted spend in the target market.
  Target economics: 100 audits/mo × $29 = $2.9k passive, plus ~15%
  upsell to $149 = ~$2.2k. Roughly $5k/mo at zero live hours.

---

## Distribution Channel

**ocdrecords.com itself** — specifically the **submit.html** page. It
already receives demo traffic from artists who self-identify as a fit;
every one of them is a pre-qualified lead for the Signal Filter audit.
Add an above-the-fold CTA on `submit.html`: *"Not sure if you're a fit?
Run the Signal Filter first — $29, instant verdict."* That's the only
new distribution surface needed. No new channel, no cold audience.

Secondary, zero-lift: add a Signal Filter badge (SIGNAL / NOISE) to each
`release.html` catalog entry — every catalog page becomes a demo of the
rubric, every visitor is one click from buying an audit of their own
track.

---

## Launch Positioning Statement

> **OCD Signal Filter: in 90 seconds, know whether your track is catalog-grade,
> sync-licensable, or still a demo — scored against every release on
> ocdrecords.com.**

---

## Week 1 Build Roadmap

1. **Write the rubric.** Draft the 7 Signal Filter axes with a 1–5
   anchor per axis, each anchor citing a specific release from the
   current catalog. Deliverable: `signal-filter-rubric.md` in this repo.
2. **Build `/signal-filter` landing + form.** New HTML page in the
   existing site style (reuse nav, glass components, Archivo/Manrope
   type). Form fields: audio upload, BPM, genre tag, intended use.
   Stripe Checkout for $29. No scoring logic yet — collect submissions
   into a queue.
3. **Wire the submit.html CTA.** Add the "Not sure if you're a fit?"
   banner to `submit.html` pointing at `/signal-filter`. Ship it. This
   is the one distribution change — everything else is product build.

Once the queue has 10 real submissions, calibrate the automated scorer
against them before switching the delivery from manual-PDF to
fully-automated. Target: fully hands-off by end of week 4.

---

## Non-goals (reject list — do not drift)

- No live coaching tier at any price.
- No "mastermind" or cohort program.
- No new social channel. ocdrecords.com is the funnel.
- No scorecard that isn't anchored to a named release in the catalog —
  the catalog is the moat.
