# OCD Records — Productize Yourself Blueprint

> A scalable product system for the OCD Records brand. Designed to convert
> the label's proprietary A&R and production expertise into an asset that
> sells at 3am without a live human on the line.

**Framing note.** The Productize Yourself prompt shipped with unfilled
placeholders (expertise, platforms, hours). No live operator was available
to fill them in, so the blueprint below is applied to the brand this
repository actually represents — **OCD Records**, the "curated label for
the obsessed creator." Swap in different inputs and the framework re-runs;
the mechanics don't change.

---

## Your Core Transformation

**I help obsessive bedroom producers go from "talented but generic and
unheard" to "signed-caliber sonic architect with a signature catalog and
sync-licensing income" — using the Signal Lock Protocol.**

The Signal Lock Protocol is the proprietary rubric OCD's A&R already uses
internally to decide which of the thousands of annual demo submissions
gets "Status: Active / Signal Locked" (the phrase that ships on every
artist profile page). Formalizing it turns an internal filter into a
product.

---

## 3 Product Formats

| Format | Leverage (sells without me, /10) | Feasibility (buildable in 30 days, /10) | Margin (/10) | Score |
|---|---|---|---|---|
| **A. Signal Lock Protocol — Field Manual** (self-serve PDF + audio pack + browser scoring tool) | 10 | 9 | 10 (~95%) | **29 / WIN** |
| **B. OCD Sample Vault** (monthly stem/preset drop from signed roster, subscription) | 9 | 7 (royalty splits, delivery infra) | 8 (~80% after splits) | 24 |
| **C. Sonic Architect Cohort** (6-week live course with A&R feedback) | 3 (requires live presence) | 6 | 7 | 16 — **REJECTED**, violates the live-presence rule |

Format C is included only to show the disqualification working. Any offer
that needs the founder on Zoom fails the 3am test and is out.

---

## Winning Product: Signal Lock Protocol — Field Manual

### Name
**Signal Lock Protocol™ — The OCD Records A&R Field Manual**
(The mechanism is named, trademarked in copy, and already surfaces
inside the site's existing "Status: Active / Signal Locked" language,
so it inherits authority instead of inventing it.)

### Contents
1. **The 7-Axis Signal Lock Rubric** — the exact scoring dimensions OCD
   A&R uses on demos (spectral density, arrangement entropy, low-end
   architecture, aesthetic coherence, mix "physicality," artist
   identity signal, catalog-fit trajectory). Each with pass/fail bands
   and reference tracks from the signed roster.
2. **The Rejection Ledger** — 20 anonymised real demo submissions with
   line-by-line A&R commentary and the specific reason each did not
   sign. Learning from rejections is impossible everywhere else on the
   internet.
3. **The Neural Ghost Deconstruction Pack** — stems + session
   screenshots + producer commentary for one flagship signed track,
   showing the rubric being satisfied in situ.
4. **Frequency Filter (browser tool)** — a self-serve web app the buyer
   uploads a WAV to. It runs the 7-axis rubric algorithmically (spectral
   analysis + presence/absence heuristics) and returns a Signal Lock
   score, per-axis gap analysis, and the two closest catalog reference
   tracks. This is the *irreplaceable* piece — the reference corpus is
   OCD's signed catalog, which no competitor can legally clone.
5. **The Resubmission Fast-Lane** — every buyer earns one guaranteed
   re-review of their next demo submission. Not a live consult;
   asynchronous, written, delivered within 30 days by the same A&R
   process — so the founder can be offline.

### Delivery Mechanism (no human in the loop)
- Gumroad or Lemon Squeezy → instant download of the Field Manual PDF +
  audio pack + private access link to the Frequency Filter tool.
- Frequency Filter hosted as a static single-page app (the site already
  runs on static HTML + petite-vue + Tailwind CDN; keeps the stack).
  Audio processing runs client-side via Web Audio API so there are no
  server costs per user.
- Resubmission Fast-Lane is a hidden form URL delivered post-purchase;
  submissions queue into the existing A&R inbox with a "SLP" tag.
  Response is a templated PDF the A&R fills once per demo — still not
  live, still async.

### What Makes It Irreplaceable
- **Reference corpus.** The Frequency Filter scores against OCD's
  signed catalog. Any imitator would need equivalent signed artists.
- **The Rejection Ledger.** Requires actually running a label with
  submission volume — no course creator can fabricate that.
- **Named A&R signal.** "Status: Signal Locked" is already brand-canon
  in the site; the product inherits the aesthetic authority instead of
  starting cold.

### Price Point
**$249 one-time.**
- Above the $99 course-price impulse tier — signals seriousness and
  filters tourists out of the Resubmission queue.
- Below the $497 cohort tier — no live delivery means no live pricing.
- At 95% margin ($236 net after gateway fees), 30 sales/month = **$7k
  MRR-equivalent** with zero incremental founder time.
- Rationale for one-time vs subscription: the transformation is
  binary (you get signed or you don't). Recurring pricing would erode
  trust. The Sample Vault (Format B) is the subscription follow-up
  once buyers convert.

---

## Distribution Channel

**The existing demo-submission funnel on `submit.html`.**

The site already runs a "Now Accepting Demos for 2025 Cycle" call — this
implies thousands of unsolicited producer submissions per year, of which
99%+ are rejected. That rejected 99% is the perfect pre-qualified
audience: they've already self-identified as "obsessive producer who
wants OCD's approval." No new channel to build, no cold traffic to buy.

**Mechanics:**
1. Rejected demos receive an automated reply: *"Not signed this cycle.
   Here's the exact rubric we scored you against, and how to close the
   gap before the next window opens — Signal Lock Protocol."*
2. Every artist page and the studios/licensing pages get one discreet
   "Signal Lock Protocol" link in the footer strip.
3. Instagram/Twitter/YouTube/SoundCloud (already wired into
   `footer.html`) drop one weekly Rejection Ledger snippet — anonymised
   demo teardown from the Field Manual, ending "full teardown in the
   Protocol." Native to the brand's existing content voice.

Zero new platforms. Every touch-point is an existing surface.

---

## Launch Positioning Statement

> **"For the bedroom producer whose tracks *sound right* but never get
> signed: the Signal Lock Protocol reverse-engineers exactly what OCD
> Records A&R listens for on demo day — turning your next submission
> into a catalog-worthy release, without a single hour of my calendar."**

Delivered in one line, it names the audience, the pain, the mechanism,
the outcome, and enforces the 3am test in the last clause.

---

## Week 1 Build Roadmap

1. **Codify the 7-Axis Rubric.** One 90-minute session with whoever
   currently makes the signing calls; write the axes, the bands, and
   the reference tracks. Ship as a plain doc first — the manual is
   downstream of this being right.
2. **Wire the rejection auto-reply.** Update `submit.html`'s form
   handler so any submission not marked "hold" triggers an email with
   the Signal Lock Protocol pre-sell link. This is the entire
   distribution engine; it has to be live before the product is.
3. **Prototype the Frequency Filter scoring UI.** Static HTML page,
   Web Audio API, one axis working end-to-end (spectral density is the
   easiest to demo). Ship a "coming soon" version that captures emails
   from anyone who tries it before purchase — the waitlist funds the
   remaining six axes and validates the demand before build cost
   compounds.

---

*Blueprint generated on the `claude/kind-edison-83nzjh` branch.*
