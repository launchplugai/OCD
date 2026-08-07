# Productize Yourself — OCD Records Blueprint

> Note on placeholders: the source prompt shipped with `[WHAT YOU HELP PEOPLE DO]`,
> `[LIST PLATFORMS]`, and `[HOURS/WEEK]` left blank. This document infers them
> from the assets already live in this repository (label site with catalog,
> tiered licensing, artist profiles, and a submission funnel) rather than
> stalling on missing input. Update the "Inferred inputs" block below if the
> real numbers diverge and re-run.

## Inferred inputs

- **Expertise / transformation offered.** Turning uncompromising, obsessive
  independent producers into a licensable, royalty-generating catalog through
  OCD Records' "human intuition + neural precision" pipeline.
- **Existing platforms / audiences.** The live label surface itself:
  `index.html` (brand), `catalog.html` (48+ releases browser),
  `artist.html` (roster profiles), `release.html` (per-release deep pages),
  `studios.html` (booking), `licensing.html` (Standard $299 / Premium $799 /
  Enterprise custom), `submit.html` (open artist submission funnel).
- **Time available to build.** Assumed 10 hrs/week solo — the 30-day roadmap
  below fits inside that envelope.

---

## Your Core Transformation

**I help obsessive independent producers go from "unheard SoundCloud dumps" to
"tracks earning license checks in film, ad, and sync catalogs" using the
Signal-to-Artifact Protocol (S.A.P.) — the same intake, curation, and
neural-mastering pipeline that powers the OCD Records roster.**

The name is deliberate: the site already anchors its brand on "audio isn't
just signal — it's a physical artifact." S.A.P. names the four-stage move
from raw signal to a monetizable artifact:

1. **Signal capture** — stems + metadata intake at spec.
2. **Artifact audit** — sync-readiness scoring (loudness, structure,
   stem separation, brief-fit, clearance risk).
3. **Neural finish** — mastering + variant generation (30s/60s cut-downs,
   stinger, alt mixes) tuned to sync-brief conventions.
4. **Placement** — routing into the OCD catalog under the tier the artifact
   qualifies for (Standard / Premium / Enterprise).

Everything below productizes that protocol so the label collects revenue
while nobody's online.

---

## 3 Product Formats (scored)

Scores are 1–5. **Leverage** = sells without me (5 = fully async).
**Feasibility** = shippable in 30 days at 10 hrs/week. **Margin** = > 70%
gross after tooling + payout to contributors.

| Format | What it is | Leverage | Feasibility | Margin | Total |
|---|---|---|---|---|---|
| **A. The S.A.P. Playbook** (digital product) | $79 downloadable kit: the protocol as a PDF, a Reaper/Logic template pack, a metadata schema, a brief-fit rubric, and 5 sync-ready reference stems. | 5 | 5 | 5 (95%+) | **15** |
| **B. Artifact Score** (tool) | Web app on the existing site: producers upload a WAV, get a 0–100 sync-readiness score, category verdict (Standard / Premium / Enterprise / reject), and a stem-prep checklist. Freemium — 1 free scan, $19/scan or $49/mo unlimited. Auto-routes qualifying tracks into `submit.html`. | 5 | 4 | 5 (~90% after inference cost) | **14** |
| **C. The Roster** (community + rev-share) | Members-only pipeline: accepted producers get catalog placement + 50/50 rev-share on licenses closed. $0 up-front, $299 annual "artifact fee" for the mastering + placement slot. | 4 | 2 (needs A2R ops, contracts, payouts, cure-list of buyers) | 3 (~55% after payouts) | **9** |

**Reject:** any "1:1 mixing consult" or "live sync-brief workshop" formats —
they collapse the moment I stop being online. The prompt's own rule says
kill them.

**Winner:** Format A (The S.A.P. Playbook) *ships first*, because it seeds
demand for Format B without needing infra. Then Format B (Artifact Score)
becomes the durable engine — highest lifetime margin and it feeds
`submit.html` for free. Format C is the 2027 story, not the 30-day story.

---

## Winning Product Structure — The S.A.P. Playbook

- **Name.** *Signal-to-Artifact Protocol — The OCD Records Playbook v1.*
  The proprietary mechanism (S.A.P.) is the buyable thing, not "another
  music course."
- **Contents.**
  1. `01_protocol.pdf` — the 4-stage S.A.P. explained with the same
     Archivo / mono type system as the site, so it reads as label canon.
  2. `02_intake_spec.md` — the exact stem-naming, sample-rate,
     LUFS-target, and metadata schema OCD accepts. (This becomes the
     `submit.html` spec, so it doubles as label documentation.)
  3. `03_artifact_audit.xlsx` — the scoring rubric behind Artifact Score.
     Shipping the rubric openly makes the tool trustworthy later.
  4. `04_reference_pack/` — 5 licensed stems (one per tier + one
     "rejected" example) so buyers hear what each score sounds like.
  5. `05_placement_playbook.pdf` — how the Standard / Premium / Enterprise
     tiers map to sync brief types (Standard = social / creator use,
     Premium = broadcast / theatrical, Enterprise = global campaign).
  6. `06_submit_fast_track.txt` — a one-time code that flags a submission
     through `submit.html` as "playbook buyer, pre-audited," moving it to
     the top of intake. This is the irreplaceable hook: only OCD can
     honor it, so no competitor can copy the playbook wholesale.
- **Delivery.** Static download via Gumroad or Lemon Squeezy behind a
  one-click checkout on a new `/playbook` page bolted onto the existing
  site (same nav, same aesthetic). Zero human touch — the fast-track code
  auto-generates on purchase.
- **Price point.** **$79 launch / $129 list.** Rationale: it's 26% of one
  Standard License ($299) and 10% of a Premium ($799). Any buyer who
  places even one track pays for the playbook 3–10×, so the perceived ROI
  is obvious. Under $100 clears the impulse threshold; over $50 signals
  it's not a lead magnet.
- **What makes it irreplaceable.** The fast-track submission code. The
  content can be copied; the routing into OCD's actual catalog cannot.

---

## Launch Positioning Statement

> **"OCD Records' Signal-to-Artifact Protocol turns your obsessive demos
> into license-ready artifacts — and drops you straight into the same
> intake queue our roster came through, without a gatekeeper email."**

Use it verbatim as the hero H1 on `/playbook` and as the pinned post
across the label's existing artist / catalog nav bar.

---

## Week 1 Build Roadmap (3 tasks, start immediately)

1. **Author `docs/sap-protocol-v1.md`** — the full 4-stage protocol
   written out, including the audit rubric. Everything else in the
   playbook is derived from this single document, so it must exist first.
2. **Ship `playbook.html`** — new page in the repo, styled with the
   existing `--crimson` / `--electric-blue` / `Archivo` / `JetBrains Mono`
   tokens so it inherits the label's look. Hard-code the positioning
   statement as the H1, a 6-item contents grid mirroring `licensing.html`,
   and a single Gumroad "Buy — $79" button. Add it to the nav in
   `index.html`, `catalog.html`, `artist.html`, `licensing.html`,
   `submit.html`.
3. **Wire fast-track codes into `submit.html`** — add a single optional
   input ("Playbook code — skip the queue"). Server-side (or a
   client-side Gumroad license-key check for MVP) flags matching
   submissions with a `fast_track: true` field. This is the mechanism
   that makes the playbook irreplaceable — build it in week 1 or the
   whole product loses its moat.

---

## Distribution channel that matches existing platform

The OCD Records **catalog and submission funnel is the channel** — it
already ranks (or will rank) for "sync-licensable electronic tracks" and
draws producers via `submit.html`. Every catalog page and every artist
profile gets a small "Producers: score your track" ribbon pointing to
`/artifact-score` (Format B) with the playbook as the upsell. That means
zero new-channel effort — no TikTok pivot, no cold outreach — the site
we've already built *is* the funnel.

---

## What ships in the next 30 days

- **Days 1–7.** Protocol doc, `playbook.html`, fast-track wiring, Gumroad
  listing live.
- **Days 8–14.** Record 5 reference stems (or license from the roster),
  export rubric as `.xlsx`, bundle the ZIP.
- **Days 15–21.** Launch. Post the positioning statement across every
  existing surface (site nav, artist bios, release pages). No new
  channels.
- **Days 22–30.** Begin Format B (Artifact Score) MVP: a single-page
  uploader that runs the rubric client-side (loudness + duration +
  structure detection via WebAudio) and issues the same fast-track code
  when the score clears the Standard threshold. This is when the system
  starts running at 3am without me.
