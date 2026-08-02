# Productize Yourself — OCD Records Blueprint

> Applied to the OCD Records label, using the site as the source of truth for what
> the brand already does (catalog, sync licensing tiers, studio rental, artist
> submissions). This is a strategy draft, not a shipped plan — review, then decide
> what to move into `index.html` / a new page.

Scheduled note: the source prompt was a generic "Productize Yourself" template
with placeholders for personal expertise, audience, and time budget. Those weren't
filled in, so this document treats **OCD Records the label** as the entity being
productized rather than fabricating personal details.

---

## Your Core Transformation

**OCD Records helps sync buyers and independent creators go from _"I can't
find a track that sounds obsessed, weird, and legally clearable"_ to _"I
licensed the right sound in under 10 minutes"_ using the OCD **Signal
Protocol** — a pre-cleared, tier-priced catalog of experimental releases with
one-click sync rights.**

The transformation already exists implicitly in `licensing.html` (Standard /
Extended / Exclusive tiers, "Frequency Rights / Sync Protocol", 24–48h response
window). It just isn't packaged as a self-serve product yet — every deal
appears to route through a human response window, which is the exact bottleneck
this exercise is meant to remove.

---

## 3 Product Formats

| Format | Leverage | Feasibility | Margin | Score |
|---|---|---|---|---|
| **A. Signal Vault** — creator-tier sync subscription (self-serve, auto-clearing licenses against the full OCD catalog) | 9 — sells and delivers overnight; recurring | 8 — catalog + Stripe + gated download + license PDF generator, buildable in 30 days | 9 — pure digital, >85% margin after Stripe/CDN | **26 / 30** |
| **B. Obsession Kits** — proprietary stem/loop/preset packs derived from label releases (Neural Ghost, Cobalt Void, etc.), branded per artist | 8 — one-time digital, sells while asleep | 7 — needs artist rev-share agreements + stem prep per release | 8 — >80% after payout split | **23 / 30** |
| **C. Transmission Circle** — paid community for aspiring sync artists, taught the OCD submission/production standard | 5 — retention needs live energy (Q&As, feedback) | 6 — Circle/Discord + monthly drop | 7 — decent, but bounded by seats | **18 / 30** |

**Rule check:** Format C brushes the "requires live presence" fail line and is
deprioritized for that reason. A and B both pass — A wins on leverage and margin.

---

## Winning Product Structure

### Name: **Signal Vault** (powered by the Signal Protocol)

Uses OCD's existing "Signal Chain / Frequency Rights" language so the branding
extends what's already on the site — not a bolt-on.

### Contents

- **The Vault** — the entire current catalog (Entropy 001 and all future
  releases), streamable and downloadable in WAV + MP3.
- **One-click auto-clearing sync license** at the subscriber's tier —
  the license PDF is generated with the buyer's project name / channel / usage
  scope at download time. No human in the loop for standard use.
- **Stems on demand** for tracks marked "stems available" (higher tier).
- **Monthly drop** — one new release added to the Vault each month; this is
  what turns it from a one-time sale into a subscription.
- **Signal Protocol license** — the proprietary document that codifies "what
  you can and can't do with an OCD track without emailing us." This is the
  irreplaceable piece: no other underground label has it standardized.

### Delivery

1. Buyer hits a `pricing.html` page (new, replaces the tiers table on
   `licensing.html` for the self-serve segment; enterprise/exclusive stays
   there and stays human-touched).
2. Stripe Checkout → webhook creates account on gated portal.
3. Portal = static Vault index + signed CDN URLs for each track, and a
   `POST /license` endpoint that stamps a PDF with the buyer's project info.
4. Nothing in the loop touches a human until the buyer wants Exclusive or
   custom composition — those stay on the existing 24–48h response track.

### Price Point

- **Creator — $29/mo** — social + YouTube up to 500k impressions per track,
  aligned with the existing Standard tier.
- **Studio — $99/mo** — up to 3 productions/mo, matches Extended tier.
- **Founding Signal — $290/yr** — first 100 subscribers, lifetime price lock.

Rationale: prices anchor to the tier language already on `licensing.html` so
the self-serve product doesn't undercut current human-negotiated deals. The
annual founding tier funds the 30-day build.

### What Makes It Irreplaceable

- **Curation** — the roster (Neural Ghost, Cobalt Void, Static Pulse, Lithium
  Soul, Elite Force) is the moat; no library-style competitor sounds like
  this.
- **The Signal Protocol license document** — the codified, tiered, pre-cleared
  contract IS the product. Competitors sell tracks; OCD sells "clear a weird
  track in one click."

---

## Distribution Channel

**The existing `catalog.html` + release pages.** Every release detail page
(`release.html`, `ocd/03-release-details-entropy-001.html`) is already a
landing page — add a persistent "License this track — from $29/mo" CTA into
the release template and every existing artist link into OCD becomes a Vault
funnel. This matches the "distribution must match your current platform" rule:
the label already publishes releases and pushes them out — Vault just gives
each release a conversion action.

Secondary: the artist submission funnel on `submit.html` — artists who submit
get notified when their work joins the Vault, which converts them into
promoters.

Do **not** open a new channel (no new TikTok, no cold outreach). The existing
release cadence is the channel.

---

## Launch Positioning Statement

> **OCD Signal Vault — one subscription, every OCD release, one-click cleared
> for your project. The obsessed sounds you can't find anywhere else, licensed
> before your edit is done rendering.**

---

## Week 1 Build Roadmap

1. **Draft `pricing.html`** — three tiers (Creator / Studio / Founding
   Signal) using the existing site chrome (Tailwind, Archivo, glass panels).
   No backend yet — the page validates the offer.
2. **Codify the Signal Protocol license** — take the language already scattered
   in `licensing.html` (Standard/Extended/Exclusive) and consolidate into a
   single templated PDF-ready document with `{{project}}` / `{{buyer}}` /
   `{{tier}}` merge fields. This is the artifact everything else depends on.
3. **Instrument the release template** — add a single "License from $29/mo →"
   CTA block to `release.html` and `ocd/03-release-details-entropy-001.html`,
   linking to `pricing.html`. This proves the funnel converts before any
   Stripe / portal work is done.

Weeks 2–4 (out of scope for this doc but sequenced): Stripe + webhook, gated
portal (static site + signed URLs is enough), license-stamping endpoint,
first monthly drop announcement.
