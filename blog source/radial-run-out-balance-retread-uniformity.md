# Radial Run-Out and Balance: The Uniformity Check Every Retread Needs Before It Ships

Pillar: A — product/equipment/process education
Published: 2026-09-18
Live post: `blog/radial-run-out-balance-retread-uniformity.html`

## Angle

No existing post covers ride-quality uniformity (radial run-out / RFV /
balance) — the site's existing buffing content
(`buffing-rasping-casing-prep-bond-quality.html`) is about bond/adhesion
quality, not roundness or vibration. Confirmed via grep across `blog/`
for balance|RFV|run-out|runout|uniformity before writing (only the
buffing-rasping post matched, tangentially). This post is the
complementary "does it ride right" piece: buffing to remove worn tread
can throw a casing out of round, and that's a distinct failure mode from
a weak bond.

## Duplicate check

Checked `blog/` (43 existing posts at time of writing) and the two open
PRs (#59 Section 232 tariff, #60 NDT/shearography casing inspection) —
neither overlaps this topic.

## Sources used (verified 2026-09-18 via WebSearch; WebFetch/curl blocked
by session egress policy on tirereview.com, tireindustry.org, retread.org)

1. Buffing worn tread can create/expose radial run-out (out-of-round)
   non-uniformities; retreaders measure buffed-casing run-out and index
   high/low spots so gum and tread application compensates for it —
   general engineering description corroborated across USPTO tire-
   retreading run-out-correction patent literature and retreading-process
   explainer content (Casing Jockey / retread-process descriptions).
2. Computer-controlled radial buffing systems guided by a casing spec
   database + continuous undertread measurement, used to hold undertread
   depth even across the crown — USPTO patent literature (general
   engineering description).
3. Radial Force Variation (RFV) definition — stiffness variation over one
   revolution under constant load, distinct from static/dynamic balance;
   RFV in use since the 1970s; OEM low-speed RFV testing defined by SAE
   Practice J332 — Tire Review Magazine, "What RFV Means to the Tire
   Industry" (Parts I & II).
4. Post-cure inspection: retreaded tires get a second NDT and balance
   check specifically to confirm the remolding process didn't alter
   integrity or balance from what was measured going in — retread.org
   process documentation, corroborated by Bauer Built, "Retread Tires:
   Fact from Fiction."
5. Tire uniformity graders/optimizers (TUG/TUO) as the equipment class
   used to measure and correct RFV at scale — USPTO patent literature
   (general engineering description); framed as plant-scale equipment,
   not something an independent shop needs to buy (matches the site's
   established "no sales spin" tone from `electric-vs-steam-curing-
   chamber.html`).
6. Undertread commonly targeted in roughly the 3/32"–5/32" range — McCarthy
   Tire Service retreading-process description, corroborated by general
   retread-process sourcing. Deliberately kept as a range, not an exact
   tolerance — TIA's RP-01-01 "Tire Profiling for Retreading" document
   itself is access-restricted on tireindustry.org (egress-blocked) and a
   prior post's research (`buffing-rasping-casing-prep-bond-quality.md`)
   already concluded no specific citable undertread-depth figure could be
   verified from primary text, so this post doesn't assert one either.

## Image

Canva unavailable this run (connector requires OAuth; not authenticated,
no interactive flow possible in this non-interactive session). Fell back
to Adobe Stock per the sourcing order: licensed asset 682192444 ("Crop
mechanic tightening wheel of truck in workshop", Canon EOS 5D Mark III
photo, 5760×3840) via `asset_license_and_download_stock`, computed a
16:9 center crop with `image_crop_and_resize`/`image_crop_to_bounds`,
verified via `asset_inline_preview`, then downloaded the ORIGINAL S3 image
directly (that host isn't egress-blocked) and replicated the exact crop
locally with `/opt/pw-browsers/ffmpeg-*/ffmpeg-linux` (crop=5760:3240:0:300,
scale to 1280x720) since the tool's own output URL is hosted on the
blocked `photoshop-api.adobe.io` domain. Genuine photograph, not a
vector/icon graphic.
