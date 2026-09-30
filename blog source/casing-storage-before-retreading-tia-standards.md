# Casing Storage Before Retreading: What TIA's Best-Practice Standards Actually Require

Pillar: A — process education, with a Pillar C (in-house operations) close
Published: 2026-09-18
Live post: `blog/casing-storage-before-retreading-tia-standards.html`

## Angle

No existing post covers casing/finished-tire storage (ozone, UV, humidity,
stacking) — `tread-rubber-cushion-gum-storage-shelf-life.html` is scoped
strictly to raw consumable materials (tread rubber, cushion gum shelf
life), not used casings or finished retreads. `casing-ownership-in-house-
retread-control.html` covers casing tracking/barcoding, not physical
storage conditions. Confirmed by reading both posts before writing.
Angle: storage is invisible until it isn't — a casing can pass every
inspection point and still degrade on the rack before it's ever buffed.
Light Pillar C tie-in at the end (storage becomes your own operational
responsibility once you run your own line, vs. happening on a vendor's
property) — kept factual and general, no franchise-naming or
monopoly-adjacent language, since that guardrail isn't really in play for
a storage-standards piece.

## Duplicate check

Checked `blog/` (44 posts including today's radial-run-out post) and the
two open PRs (#59 tariff, #60 NDT/shearography) plus this run's other new
post (#61, radial run-out/balance) before writing. Grepped for "casing
storage", "ozone crack", "store casings" — no matches. Grepped more
broadly for storage|warehous|ozone — the only real overlaps are the
consumables-shelf-life post (different subject: raw materials, not
casings) and passing mentions in cost-to-set-up (facility space, not
storage conditions).

## Sources used (verified 2026-09-18 via WebSearch; direct fetch of
tireindustry.org blocked by session egress policy)

1. Tire Industry Association, "Best Management Practices for Proper Tire
   Storage" — named, real TIA document (tireindustry.org); specific
   points relayed via WebSearch synthesis since direct fetch is
   egress-blocked from this session:
   - Store away from electric motors, battery chargers, welding
     equipment, and generators — this equipment generates ozone, which
     has a deteriorating effect on rubber.
   - Store on a pallet or rack, not directly on the ground.
   - Store upright in racks to prevent distortion; limit stack height
     and rotate flat-stacked stock.
   - Tires stored mounted on rims should be inflated to roughly 50% of
     normal operating pressure.
2. Temperature/humidity range (roughly below 77°F, above freezing;
   moderate humidity) and UV/sunlight as a cracking driver — corroborated
   independently by warehouse-racking industry publishers Mecalux /
   Interlake Mecalux and AR Racking, consistent with TIA's guidance
   rather than a single-source claim.
3. Moisture promoting mold/rust on steel belts and beads from the inside
   — general corroboration across the same warehouse-racking sources.
4. No chemical (solvent/fuel/lubricant/disinfectant) contact — same
   general tire-storage-guidance corroboration.

No specific fleet, customer, or dollar-savings example is used in this
post — kept to documented storage standards and general reasoning, per
the fact-check standard.

## Image

Canva unavailable this run (OAuth required, not authenticated). Adobe
Stock fallback: licensed asset 333522915 ("Large modern warehouse with
forklifts and stack of car tires", 6016×4016) via
`asset_license_and_download_stock` — first licensing attempt on a
different candidate (323748729) hit a transient upstream error, retried
successfully on this asset. Cropped to 16:9 via `image_crop_to_bounds`,
verified with `asset_inline_preview`, then downloaded the original S3
image directly and replicated the identical crop locally with
`/opt/pw-browsers/ffmpeg-*/ffmpeg-linux` (crop=6016:3384:0:316, scaled to
1280x720) since the tool's own output URL is on the egress-blocked
`photoshop-api.adobe.io` host. Genuine photograph (racked tire storage
aisle), not a vector/icon graphic; the warm light at the aisle's end
happens to match the site's dark-industrial-with-orange-accent look.
