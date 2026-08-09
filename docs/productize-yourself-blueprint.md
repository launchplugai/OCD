# OCD Records — Productize Yourself Blueprint

_A scalable-operator design applied to the label's demonstrated expertise: sonic
architecture, boutique electronic curation, studio engineering, and sync licensing.
Built to sell at 3am with nobody online._

> Note on inputs: the scheduled prompt's `INFORMATION ABOUT ME` fields were not
> filled in. This blueprint infers the operator's expertise, platforms, and
> constraints from the current site (index / catalog / release / artist /
> studios / licensing / submit pages). Swap the assumptions in **§ Inputs Used**
> when the operator wants a re-cut.

---

## Your Core Transformation

**I help serious independent electronic producers go from unfinished bedroom
demos to a release-grade, sync-licensable catalog track — using the Frequency
Protocol™: a 7-stage signal chain and delivery spec that meets OCD Records'
Tier-02 (Premium) licensing standard on the first submission.**

The transformation is measurable: the producer's file passes the same technical
gate the label applies to its own catalog (LUFS, true-peak, stereo image,
stem-splits, cue-point map, tag metadata). Pass = catalog-eligible. Fail = a
diff report telling them exactly which stage broke.

---

## 3 Product Formats

Scored 1–10 on each axis. Leverage = sells while founder sleeps. Feasibility =
shippable in 30 days with the existing site. Margin = gross margin after
delivery cost. Total = sum, ranked.

| # | Format | Leverage | Feasibility | Margin | Total |
|---|--------|----------|-------------|--------|-------|
| 1 | **Frequency Protocol Kit** — DAW template sessions (Ableton + Logic) preloaded with the OCD signature chain, plus a written spec and a reference-track A/B pack | 10 | 9 | 9 (~95%) | **28** |
| 2 | **Sync-Ready Auditor** — web tool: upload a WAV, get a Tier-02 pass/fail report against the label's licensing spec, with a fix list | 9 | 6 | 8 (~85% after infra) | **23** |
| 3 | **Sonic Architecture Cohort** — 6-week live course + Circle community | 3 (needs presence) | 7 | 6 (~65% after ops) | **16** |

Format 3 **fails Rule 1** (requires live presence). Rejected. Format 1 wins on
all three axes and is what an under-30-day build should ship.

---

## Winning Product Structure

- **Name:** **Frequency Protocol™ Kit — Tier-02 Edition**
  - Proprietary mechanism: the 7-stage Frequency Protocol (Source → Sculpt →
    Space → Sum → Stem → Stamp → Ship). Each stage has a named gate that maps
    1:1 to the label's Premium License technical spec — so passing the Kit
    means the track is literally submittable.
- **Contents (what buyers get in the zip):**
  1. `Frequency-Protocol.pdf` — 24-page playbook, one page per gate, with the
     numeric targets (integrated LUFS -14 ±0.5, true-peak ≤ -1.0 dBTP, stereo
     correlation floor, LR delta ceiling, tag schema).
  2. `Templates/Ableton.als` + `Templates/Logic.logicx` — session files with
     the signature bus chain, correctly gain-staged, color-coded per stage.
  3. `Reference/` — 4 A/B stem pairs from released catalog tracks (Elite
     Force, Neural Ghost, Cobalt Void, Static Pulse) with a `NOTES.md`
     explaining the specific decision at each gate.
  4. `Delivery/submission-checklist.pdf` — the exact filename convention,
     metadata schema, and stem-split spec used by the label's A&R queue.
  5. `Bonus/`— a one-time 15% licensing-fee credit voucher redeemable on the
     buyer's first accepted catalog track (converts customers into supply).
- **Delivery mechanism (no founder required):**
  - Sold from `/kit` on the existing OCD Records site. Gumroad or Lemon
    Squeezy checkout (Stripe on the back). On payment, webhook fires an
    automated email with a signed 72-hour S3 download URL. No manual step.
  - The `/submit` page gains a "Kit-verified?" checkbox — verified submissions
    jump the manual review queue from 14 days to 5. This makes the Kit
    _visibly_ preferential inside the funnel that already exists.
- **Price point:** **$149** one-time.
  - Rationale: below the impulse-buy ceiling for a working producer
    ($200), 10× a sample pack (positions as tooling, not content), and 1/3
    the cost of one Tier-02 sync license — so it pays back on a single
    placement. Margin at $149 with a ~$4 processing + ~$1 storage cost per
    unit ≈ **96%**.

**What makes it irreplaceable:** the Kit is a private-key match to the
label's licensing gate. Anyone can sell a mastering course; only OCD Records
can sell a Kit whose pass criteria _are_ the OCD Records submission spec, and
whose voucher redeems against the label's own catalog. Cloning it requires
running a label.

---

## Distribution Channel (existing surface, zero new platform)

The `/submit` page currently reads _"we review every submission manually
within 14 business days"_ — that funnel is the highest-intent traffic on the
site and it already assumes the visitor is a producer with a finished-ish
track. Add a single line above the submit form:

> Submissions that pass the Frequency Protocol are reviewed in 5 days, not 14.
> [Get the Kit →](#/kit)

Every rejected submission also triggers a diff email — _"here are the 3 gates
your track failed; the Kit fixes them"_ — turning the existing rejection
volume into the primary sales channel. Nothing new to launch. No new
platform, no new audience-building, no live presence.

---

## Launch Positioning Statement

> **The Frequency Protocol™ Kit turns a bedroom demo into a Tier-02
> sync-licensable track — using the exact spec OCD Records applies to its
> own catalog. Pass the gate, skip the queue.**

---

## Week 1 Build Roadmap

1. **Write the 7 gates as numeric pass/fail criteria** (one afternoon).
   Freeze the spec before touching any template. Deliverable:
   `Frequency-Protocol-spec-v1.md` — the source of truth every other artifact
   points back to.
2. **Cut the Ableton template from a known-good catalog session** (one day).
   Take the Entropy-001 session, strip its content down to the bus/routing,
   color-code by gate, save as `.als`. Logic port comes in week 2.
3. **Wire the checkout on a `/kit` page + submission-queue diff email**
   (one day). Gumroad product, webhook → S3 signed URL email, and a one-line
   change to `submit.html` linking to `/kit`. This is the smallest change
   that lets the funnel start selling before the Kit contents are 100%
   finished — pre-orders fund the last 20% of the build.

---

## Inputs Used (swap when re-cutting)

- **Expertise / transformation:** inferred from `licensing.html` (Tier
  01/02/03 spec, sync-license workflow), `studios.html` (engineering depth
  — Abbey Road, Berklee, Berlin mastering), `submit.html` (14-day manual A&R
  review), and the catalog releases (Entropy-001, Elite Force, Neural
  Ghost).
- **Current platforms:** the OCD Records website (index, catalog, release,
  artist, studios, licensing, submit). No external channels assumed.
- **Time to build:** assumed ~10 hrs/week for 4 weeks. Week-1 roadmap fits
  in ~3 focused days if concentrated.
