# OCD Records — Productize Yourself Blueprint

> Applied to the OCD Records label, studios, and demo-submission funnel visible in this repo. Placeholders in the source template were filled from repo context (positioning, roster, studio spec sheet, submission page); update the assumptions block if any are wrong.

## Assumptions used to fill the template

- **Expertise / transformation offered:** OCD Records turns obsessive but formless independent producers into label-ready artists with a distinct sonic identity — the same craft the label already sells via signing, studios, and licensing.
- **Existing platforms:** the OCD Records website (index, catalog, artist, studios, licensing, submit) and the inbound demo funnel it collects; SoundCloud / Bandcamp / streaming references are already invited on the submit page.
- **Time available to build:** ~10 hrs/week of one engineer + one A&R (assumed for the 30-day feasibility window; adjust if wrong).

---

## Your Core Transformation

**I help obsessive independent producers go from bedroom demos that never quite sound like a finished record → label-ready releases with a signature sonic identity, using the Signal Chain Method (Intuition → Precision → Artifact → Transmission).**

The Signal Chain Method is the proprietary four-stage pipeline the OCD studios and A&R team already run on signed artists. Codifying it as a named framework is what converts a service into a product.

---

## 3 Product Formats

Each format was filtered against the rules: no live presence required, must carry a named framework, must ride existing OCD distribution.

| Format | Leverage (sells without you) | Feasibility (buildable in 30d) | Margin (>70%) | Score /30 |
|---|---|---|---|---|
| **A. Signal Chain Kit** — sample pack + preset bank + Ableton/Pro Tools template + embedded method PDF | 10 | 9 | 10 | **29** |
| **B. Signal Chain Masterclass** — recorded self-paced course (video + worked-example teardown of an existing Entropy release) | 8 | 6 | 9 | 23 |
| **C. Transmission Vault** — paid async community; monthly batched engineer-annotated feedback drops (never live) | 6 | 7 | 8 | 21 |

Rejected outright: 1:1 mixing/mastering retainers, live cohort courses, in-person studio workshops — all fail the "sells at 3 a.m. without me" test.

**Winner: A. Signal Chain Kit.** Highest on all three axes, and it is the only format that lets a buyer *use* the OCD sound the same night they buy it — a shorter time-to-value than either the course or the community.

---

## Winning Product Structure

### Name
**Signal Chain Kit vol. 01 — Entropy**
(Series named after existing catalog release ENTROPY-001, so every future kit — vol. 02 Neural Ghost, vol. 03 Cobalt Void — inherits roster equity.)

### Contents
- **Stems** (24-bit / 48kHz) from one released OCD catalog track, cleared for production use.
- **Preset bank** for Serum, Prophet-5 (soft), and the analog chain modeled from the Studios rig (SSL 4000G+ / Neve 8078 emulations).
- **Ableton Live 12 + Pro Tools session templates** pre-wired to the four Signal Chain busses (Intuition / Precision / Artifact / Transmission).
- **The Signal Chain Method** — a 30-page PDF + 4 short video teardowns (~8 min each) showing how the ENTROPY-001 session moved through each stage. This is the proprietary framework; the samples are the delivery vehicle.
- **A/B reference mix** — the same track before and after the Signal Chain, so buyers hear the transformation.
- **License stub** — non-exclusive production license; royalty-free for original releases.

### Delivery mechanism (no live presence)
- Sold via **Gumroad** (or Bandcamp digital item) as a single ZIP + hosted video links.
- Payment webhook → automated email with download + one-click "add me to the Transmission list" opt-in.
- Course video hosted unlisted on YouTube/Vimeo; PDF linked from Gumroad.
- **Zero human touch after the buy button** — this is the pass/fail on the 3 a.m. test.

### Price point
- **$79 launch tier** (first 100 buyers, "founding transmission" — social proof + testimonials).
- **$149 standard tier** thereafter.
- **$349 studio tier** — adds a one-off async written feedback pass on the buyer's Signal-Chain-processed track by an OCD engineer. Capped at 10/month to protect margin, and still not "live."
- Rationale: sample packs in this space anchor $30–$80; the embedded method + label brand justifies a 2–3× premium; the studio tier converts high-intent buyers without pulling engineers into a synchronous obligation.

### What makes it irreplaceable
- **Roster provenance:** these are the *actual stems* from an OCD catalog release, not sound-alikes.
- **Named methodology:** competitors sell samples; only OCD sells the Signal Chain that produced them.
- **Studio DNA:** presets model the SSL 4000G+ / Neve 8078 chain the label is already known for on the Studios page.
- **Series compounding:** vol. 01 sells vol. 02; every signed artist becomes a future kit.

---

## Distribution Channel (matches existing platform)

**The Submission Funnel** — the `/submit` page in this repo already collects the exact audience the Kit is built for: producers who admire the OCD sound enough to send WAVs.

Wire it up (no new channel required):
1. Every demo submission auto-responds with: "We review manually in 14 days. While you wait — this is the exact system we use on signed artists. Signal Chain Kit vol. 01: [link]."
2. Rejected demos (~95% of submissions) receive a tailored "here's the gap we heard — the Signal Chain Kit teaches the fix" follow-up.
3. Signed artists' release announcements on the catalog page carry a "Made with Signal Chain Kit vol. XX" credit that back-links.
4. The existing "Subscribe to frequencies" newsletter is the retention loop for vol. 02+.

This is the only channel where OCD already owns qualified inbound. Starting on TikTok / Reddit / Splice would violate the "do not start from zero" rule.

---

## Launch Positioning Statement

> **For obsessive independent producers whose demos never quite sound like a finished record — the Signal Chain Kit gives you the stems, presets, and four-stage method OCD Records runs on signed artists, so you can ship a label-grade track this weekend without ever booking a studio.**

---

## Week 1 Build Roadmap

1. **Pick the vol. 01 source track and clear its stems.** Choose one ENTROPY-series release with clean multitrack, get the artist to sign the non-exclusive sample license, export stems at 24/48. (Blocks everything else — do this Monday.)
2. **Record the Signal Chain teardown once.** Four ~8-minute screen recordings walking the chosen session through Intuition → Precision → Artifact → Transmission. One take, no edits, published unlisted. Draft the 30-page PDF from the video transcripts.
3. **Wire the funnel.** Create the Gumroad listing at the $79 founding tier, connect the payment webhook to an auto-delivery email, and add a single-line CTA + product card to `submit.html` (thank-you state) and `catalog.html` (nav strip). Ship it live behind the founding-tier price and start counting the first 100.

---

## What this blueprint deliberately does *not* do

- No 1:1 coaching, no live cohorts, no "book a call" CTAs — all fail the 3 a.m. test.
- No generic "learn electronic music production" course — the framework is named and proprietary, tied to actual catalog releases.
- No new-platform launch — distribution rides the existing site + submission inbox.
