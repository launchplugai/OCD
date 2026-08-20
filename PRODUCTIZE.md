# OCD Records — Productize Yourself Blueprint

> **Note on interpretation.** The stored prompt that generated this doc had unfilled placeholders
> (`[WHAT DO YOU HELP PEOPLE DO OR BECOME]`, `[LIST - EVEN SMALL]`, `[HOURS/WEEK]`). Rather than
> return an empty template, this blueprint applies the framework to the only concrete "you" visible
> in the repo — **OCD Records**, the boutique label/licensing site currently shipping in `main`. If
> the intent was a personal blueprint for the site owner, swap the inputs and re-run.

---

## Your Core Transformation

OCD Records helps **brands, sync supervisors, and content teams** go from
**hunting through generic royalty-free libraries that make their work sound like everyone else's**
to **shipping with a distinctive, label-grade sonic identity that raises the perceived tier of the
entire piece** — using the **Neural Precision Method™** (the label's stated bridge between human
intuition and neural precision, applied as a repeatable curation + clearance protocol).

---

## 3 Product Formats

Scoring on 1–10. **Leverage** = sells and delivers without a live human. **Feasibility** = shippable
in 30 days with current assets. **Margin** = gross margin above 70% at steady state.

| # | Format | Description | Leverage | Feasibility | Margin | Score |
|---|---|---|---|---|---|---|
| 1 | **Subscription (community/access)** | *Transmission Pass* — monthly all-you-can-license access to a rotating curated pool from the OCD catalog, pre-cleared, delivered via a members' feed. | 10 | 9 | 9 | **28** |
| 2 | **Digital product (pack)** | *Sonic Identity Kit* — downloadable stems + preset library + written playbook teaching a brand's in-house team to build a recognizable sonic identity using the Neural Precision Method. | 8 | 9 | 10 | 27 |
| 3 | **Tool (SaaS)** | *OCD Sound Match* — brief-in / catalog-out matcher: paste a mood/reference URL, get ranked, pre-cleared tracks with instant checkout. | 10 | 5 | 8 | 23 |

**Rejected on the "no live presence" test:** custom scoring, artist A&R packages, in-studio
sessions — all require the founder or a specialist in the room and cannot ship at 3am. They stay
on the Enterprise tier where hourly economics work.

---

## Winning Product: Transmission Pass

### Why it wins
Uses the catalog that already exists as inventory (no new production risk), converts one-shot
per-track buyers into recurring revenue, and matches the brand voice — "Join Transmission" is
already sitting unclaimed in the site footer.

### Name and proprietary mechanism
**Transmission Pass**, powered by the **Neural Precision Method™** — a three-lens curation protocol
the catalog is filtered through every cycle:

1. **Signal** — sonic signature strong enough to be identified within 4 bars.
2. **Frame** — arrangement clean enough to sit under dialogue or voiceover without EQ surgery.
3. **Clearance** — publishing and master rights pre-consolidated so no lawyer touches it.

Every track shipped inside the Pass carries a Neural Precision certificate stamped with those three
checks — this is what makes the Pass irreplaceable versus generic subscription libraries (Artlist,
Musicbed, Epidemic). Competitors sell volume; OCD sells a curated, editorially-defended pool.

### Contents (what a subscriber gets)
- **Monthly Drop** — 8–12 new pre-cleared tracks each cycle, chosen by the Neural Precision panel,
  released as a batch on the first Tuesday.
- **Full Rolling Vault** — access to every prior drop for the duration of the subscription (~100
  tracks by month 12).
- **Stems + Instrumentals** included for every track.
- **License certificate PDF** auto-generated per download, project-scoped, embedded metadata.
- **Members' Transmission feed** — a private RSS/Notion page with liner notes, tempo/key metadata,
  and "cleared for" flags (broadcast/social/podcast/gaming).
- **First-look rights** — 72-hour window on unreleased catalog before it hits the public store.

### Delivery mechanism (works at 3am)
- Stripe subscription checkout on the site → provisions a member account.
- Members feed served as a static, per-user-signed page (S3 or Cloudflare R2 with signed URLs).
  New drops published by dropping files in a folder — a scheduled build regenerates the feed.
- License PDF generated on download via a stateless serverless function (project name is the only
  runtime input; the certificate template + Neural Precision seal are pre-baked).
- Support is asynchronous: a `hello@ocd` inbox with a 48-hour SLA published on the page. No live
  chat, no calls in the loop.

### Price point
- **$149 / month** or **$1,290 / year** (~28% annual discount).
- Rationale: sits above Artlist Pro (~$16.60/mo) and Musicbed Personal (~$21.99/mo) but well
  below one Standard License ($299 per track). One track licensed per month already breaks even
  versus per-track pricing, so any active brand converts. The premium price is the positioning —
  buying Transmission signals the same taste OCD's brand is built on.
- Team seat add-on: **+$79/mo** per additional user.

### What makes it irreplaceable
- **Curation defensibility.** The Neural Precision Method™ is a named, auditable filter competitors
  can't copy without the label's ear.
- **Pre-cleared for real-world use.** Most subscription libraries hedge on broadcast, sync, and
  paid social. Transmission's certificate is explicit and enumerated.
- **Scarcity by design.** Cap the Pass at (e.g.) 500 seats. Waitlist over that. Scarcity is on-brand
  for a boutique label and forces price integrity.
- **Artist economics.** Publish the revenue-share formula openly (e.g., 50% of Pass revenue pooled
  and distributed by monthly stream/download weight). This turns the roster into distribution — every
  artist has a reason to promote the Pass to their own audience.

---

## Distribution Channel (matches current platform)

**The existing OCD Records site + the already-live "Join Transmission" newsletter capture in the
footer of every page.** No new platform required.

Concrete sequencing:
1. Re-point the footer's "Join Transmission" form from newsletter-only to a **waitlist for the Pass**
   with a stated launch date. Every page on the current site already sends traffic into this capture
   — that funnel is currently unmonetized.
2. Add a **fourth licensing tier** on `licensing.html` (or a lateral "Subscribe" card) titled
   *Transmission Pass* alongside Standard/Premium/Enterprise. This is the highest-intent surface on
   the site and it currently offers no recurring option.
3. Publish a **Neural Precision Method™** explainer page (`transmission.html`) as the destination
   for the waitlist and the tier CTA — this is the story page that justifies the price.

No cold audience-building required — the site's own inbound traffic and the roster artists' existing
social channels are the launch engine.

---

## Launch Positioning Statement

> **Transmission Pass gives brands and creators one flat monthly rate for pre-cleared, label-grade
> underground music — curated through the Neural Precision Method™, delivered without lawyers,
> sync fees, or waiting.**

---

## Week 1 Build Roadmap

1. **Ship `transmission.html`** — a single landing page containing: the positioning sentence, the
   three-lens Neural Precision Method™ explanation, sample drop preview (3 tracks from the existing
   catalog), pricing card, and email waitlist form. Reuse the existing site's design tokens (glass
   cards, red-600 accent, font-display) so it feels native.
2. **Re-wire the "Join Transmission" footer form** across all pages to POST to the same waitlist
   endpoint as the new landing page. Add a `?src=footer` param so waitlist source is tracked.
3. **Draft the Transmission Charter** — a short public document at `/transmission-charter.md` (or
   an inline section on `transmission.html`) that names the three lenses, the drop cadence, the
   seat cap, the clearance scope, and the artist revenue-share formula. Publishing the charter
   before taking a single dollar is what makes the mechanism credible and non-generic; it is also
   the anchor sync supervisors and legal review will ask for on day one.

Everything else — Stripe integration, member-only feed, license PDF generation, back-catalog
tagging — is Week 2+ and does not block starting the waitlist.

---

## Framework Compliance Check

- ✅ Requires no live presence to deliver (fulfillment is drops + static member feed + auto-PDF).
- ✅ Includes a named, proprietary methodology (**Neural Precision Method™**) — not a generic pool.
- ✅ Distribution runs on the platform that already exists (OCD site + Join Transmission footer),
  not a channel launched from zero.
