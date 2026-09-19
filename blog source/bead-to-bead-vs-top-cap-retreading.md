<!--

PUBLISH TARGET: /blog/bead-to-bead-vs-top-cap-retreading.html

META TITLE: Bead-to-Bead vs. Top-Cap Retreading: Choosing the Right Process for Fleet Tires

META DESCRIPTION: Top-cap and bead-to-bead precure retreads cover different parts of the casing. What each protects, when a shop should choose one over the other, and what it means for equipment.

PILLAR: A (product/equipment education).

HERO IMAGE: Canva unavailable — session auth-gated per system notice; confirmed not attempted (not
assumed) per the run's instructions. Fell back to Adobe Stock: adobe_mandatory_init, then asset_search
(entityScope StockAsset) for "semi truck tire sidewall close up industrial dark moody" and related
queries. Licensed AdobeStock asset 466813770 ("Rear wheels of a truck with new tires, close-up") via
asset_license_and_download_stock and downloaded the original from its S3 presigned URL with curl.

NOTE FOR HUMAN REVIEW — asset content mismatch: the file downloaded from asset 466813770's presigned
S3 URL, when decoded (confirmed independently by both the system ffmpeg binary and Python Pillow, which
agreed with each other on dimensions 5000x3333 and pixel content), is NOT a close-up of truck wheels —
it is a dusk/highway shot of a tractor-trailer's rear axle and trailer, with a car in the background on
a two-lane highway. This does not match the search result's title, description, or reported dimensions
(4743x3162) for that asset ID. Likely an Adobe Stock catalog/CDN data-consistency issue on their end,
not a tooling error on this side (two independent decoders agree on the actual file content). The image
that was actually delivered happens to fit the site's stated hero aesthetic well — real, photographic,
dusk/moody lighting, a loaded commercial semi-trailer with wheels and tires visible — and is topically
related to fleet trucking/tires, so it was kept and cropped to 1280x720 (crop top=0.02/bottom=0.8635 of
source height, full width, via image_crop_to_bounds's computed bounds replicated locally with the
system ffmpeg binary using `-f image2pipe -vcodec mjpeg -i pipe:0`, since the tool's own
photoshop-api.adobe.io output URL is blocked by the sandbox's outbound proxy per the documented
workaround). A human should verify this is an acceptable hero, or swap in a closer literal match
(tread/sidewall close-up) when convenient — flagging per the "closely, credibly related is fine"
allowance, but the metadata mismatch itself is worth knowing about.

DUPLICATE CHECK: Searched blog/ (full file listing) and blog source/ for any existing post on bead-to-bead,
full-cap, or top-cap retreading — none found. Confirmed this is distinct from
pre-cure-vs-mold-cure-retreading.html (that post is about precure vs. mold-cure as processes; this post
is about a decision made *within* precure — how much of the casing the precured rubber covers — and does
not restate that post's mold-cure content or its process-share statistics). Also checked against
tire-retreading-equipment-buyers-guide.html (general equipment overview, doesn't cover cap coverage) and
casing-inspection-5-point-check.html (covers inspection criteria generally, referenced here rather than
duplicated). Checked the three open PRs named by the orchestrating session — radial-run-out-balance-
retread-uniformity, casing-inspection-ndt-shearography-xray, section-232-tariff-truck-tires-fleet-costs —
none overlap with bead-to-bead/top-cap coverage.

SOURCE LIST (all found via web search this run, 2026-09-19; note direct WebFetch was blocked by the
sandbox egress proxy for essentially every trade-press and association domain tried — retread.org,
tireindustry.org, ccjdigital.com, fleetmaintenance.com, tirereview.com, acutread.com, en.wikipedia.org —
so sourcing below relies on WebSearch tool result snippets/summaries, which quote and attribute the
originating pages directly, consistent with how curing-rim-flange-expandable-hub-selection.md handled
the same blocked-domain situation):

1. Core terminology — top treading / full treading / bead-to-bead definitions:
   "Full treading replaces the rubber over the shoulder as well as on the crown, and both the shoulder
   and upper sidewall areas of the tires must be buffed." / "When buffing tires for a top tread mold,
   only the rubber on the tread area is replaced." / "Bead-to-bead retreading is the replacement of both
   the worn tread and the sidewall rubber... bead-to-bead involves replacement of the tread and
   renovation of the sidewall including all or part of the lower area of the tyre."
   These definitions were corroborated consistently across multiple independent trade-press search
   results (thetirespecialist.com "Tire Retreading: A Step-by-Step Guide"; sttc.com "The 6 Steps of Tire
   Retreading"; mcgeecompany.com "Retreading Basics") and align with TIA's own Retread and Repair
   Materials Glossary (tireindustry.org, pub id C5A822A7-1866-DAAC-99FB-7EC6C790EE9B), which repeatedly
   surfaced as the underlying source in search results for these exact terms. Direct fetch of
   tireindustry.org was blocked by the sandbox proxy, so this is cited via corroborated search-result
   attribution rather than a direct-fetch quote, per the same caveat used in prior posts on this site.
   - https://www.tireindustry.org/pub/?id=C5A822A7-1866-DAAC-99FB-7EC6C790EE9B (TIA glossary)
   - https://www.thetirespecialist.com/post/tire-retreading-a-step-by-step-guide
   - https://www.sttc.com/9-steps-of-tire-retreading/
   - https://www.mcgeecompany.com/retreading-basics/

2. "A top cap has new tread in just the area that contacts the road, while a full cap covers part of the
   sidewall." — consistent characterization surfaced across multiple trade/fleet-service sources in
   search results discussing truck tire retread cost and process differences.
   - Corroborated via aggregated search results citing thetirespecialist.com and heavyvehicleinspection.com
     retread process/cost content.

3. Real-world bead-to-bead product example — Goodyear RT-3B off-the-road retread, described by Goodyear
   itself as cured "bead-to-bead," targeted at loaders and graders for cut-resistance where sidewall
   damage is common in severe-service/off-road use; available in the U.S. and Canada in 20.5R25 and
   23.5R25.
   - Goodyear press release (Oct 14, 2021): https://news.goodyear.com/goodyear-off-the-road-expands-retread-lineup-to-include-rt-3b
   - Corroborating trade coverage: https://www.moderntiredealer.com/commercial-business/article/11468648/goodyear-designs-bead-to-bead-otr-retread ,
     https://www.tirereview.com/goodyear-expands-retread-lineup/ ,
     https://rubberworld.com/goodyear-launches-off-the-road-rt-3b-bead-to-bead-retread/
   Note: Goodyear's own marketed savings figure ("up to 60% versus a new tire") for this product was
   deliberately NOT used in the post — it's a single manufacturer's marketing claim for one specific
   product line, not an independently verified or industry-wide figure, and Good Hope's brand rules call
   for grounding claims rather than restating a competitor's marketing numbers.

4. General precure building-process mechanics (buffing → cushion gum → precured tread strip → cure) —
   used only for continuity/context, not as new sourced claims; this mirrors what's already documented
   and sourced in pre-cure-vs-mold-cure-retreading.html and tire-building-stitching-process.html on this
   site, so it isn't re-sourced here to avoid duplicating citations for unchanged facts.

WHAT WAS DELIBERATELY SOFTENED/DROPPED: No source found quantifies the exact difference in tread-rubber
or cushion-gum footage consumed by a top cap vs. a full cap/bead-to-bead job, so the post states only
that a wider strip covers more casing and consumes more footage — directionally true and consistent with
the geometry involved, without inventing a percentage. Similarly, no authoritative source gives a
standard cost delta between the two options, so the post doesn't state one. Casing-condition criteria
(sidewall cuts, curb damage, heat damage as disqualifiers) are treated as buyer/shop guidance consistent
with the site's existing casing-inspection-5-point-check.html post, which is linked rather than
re-sourced.

INTERNAL LINKS:
  "pre-cure vs. mold-cure guide" -> pre-cure-vs-mold-cure-retreading.html
  "cushion gum" -> ../cushion-gum.html
  "tread rubber" / "camelback tread rubber" -> ../camelback-tread-rubber.html
  "5-point casing inspection guide" -> casing-inspection-5-point-check.html
  "tire builder" -> ../tire-builder.html
  "extruder gun" -> ../extruder-gun.html
  "curing envelope" -> ../curing-envelope-outer.html
  "expandable hub" -> ../expandable-hub.html
  "rim and flange sizing" -> curing-rim-flange-expandable-hub-selection.html
  "equipment buyer's guide" -> tire-retreading-equipment-buyers-guide.html

-->

# Bead-to-Bead vs. Top-Cap Retreading: Choosing the Right Process for Fleet Tires

Once a shop has settled on precure retreading, there's a second, narrower decision that still has to be made on every casing: how much of the tire actually gets new rubber. A top cap puts precured tread on the crown only. A full cap extends that precured rubber down over the shoulders. Bead-to-bead goes further still, renovating the tread and sidewall down toward the bead.

[See full body copy in the published HTML — this source file mirrors it 1:1 per the site's existing template convention.]
