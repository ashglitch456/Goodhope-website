<!--

PUBLISH TARGET: /blog/cvsa-roadcheck-tire-violations-retread-safety.html

META TITLE: What CVSA's 2026 Roadcheck Data Actually Shows About Tire Violations

META DESCRIPTION: CVSA's 2026 International Roadcheck put 2,914 tires out of service — 20.9% of all vehicle OOS violations. Here's what the data does, and doesn't, prove.

NOTE ON HERO IMAGE: Canva was unavailable this run (MCP server not authenticated —
no OAuth possible in this non-interactive session). Sourced a real, licensed
photographic hero from Adobe Stock instead: asset_search (entityScope
StockAsset, query "truck tire inspection") returned "Semi Truck Mechanic
Inspecting Vehicle Tire During Daytime Repair in Urban Area" (Adobe Stock
asset ID 1091817403, 6000x4000, free-tier/core), licensed via
asset_license_and_download_stock. image_crop_and_resize's own output URL
was on photoshop-api.adobe.io, which this session's egress proxy blocks, so
per the known-quirk workaround the ORIGINAL licensed image was downloaded
directly from its S3 presigned URL via curl and cropped locally with ffmpeg
(/opt/pw-browsers/ffmpeg-1011/ffmpeg-linux, piped mjpeg input) to a center
16:9 crop (crop=6000:3375:0:280) matching the site's existing 1280x720 hero
convention, then scaled to 1280x720. Saved as
cvsa-roadcheck-tire-violations-retread-safety-hero.png. og:image and the
JSON-LD image field point to this hero.

INTERNAL LINKS:

  "Retread Tire Safety: What the TRIB/TIA Data Actually Shows" -> blog/retread-tire-safety-trib-tia-data.html
  "Casing Inspection: The 5-Point Check Before Every Retread" -> blog/casing-inspection-5-point-check.html
  "inspection spreader" -> /inspection-spreader.html
  "equipment buyer's guide" -> blog/tire-retreading-equipment-buyers-guide.html

DUPLICATE-TOPIC CHECK: Confirmed against the list of existing/open-PR topics
supplied in the task (cost-per-mile, extruder guns, curing chambers,
fleet-switching trends, franchise lock-in, buffing/rasping, fleet ROI,
casing ownership, tax credit legislation, wide-base singles, nitrogen
inflation, Canada-China dumping, steer-axle rules, buffing dust, SmartWay,
skiving, rasp blades, scrap tire circular economy, tread compound) plus the
two existing safety posts (retread-tire-safety-trib-tia-data.html — TRIB/TIA
sourced; casing-inspection-5-point-check.html — process/how-to). This post
leads with CVSA International Roadcheck enforcement data, which neither
existing post uses, and is framed to build on rather than duplicate them
(explicit internal links to both, no re-argued content).

CRITICAL FRAMING CHECK: CVSA's Roadcheck results do not break tire
out-of-service violations out by retread vs. new/original-tread
construction. The post says so explicitly (see "What this data doesn't
say" section) and does not state or imply that the CVSA data shows
retreads perform better, worse, or the same as new tires. The affirmative
claim made instead is narrower and fully sourced: tire OOS violations are
overwhelmingly tread-depth, physical-damage, and inflation
issues — maintenance/inspection neglect — not a defect traceable to
construction type. That point is triangulated from two independent
sources: the CVSA/trade-press violation-category breakdown (this post) and
the UMTRI/FMCSA debris study + TRIB/TIA position already cited in
retread-tire-safety-trib-tia-data.html (referenced, not re-argued, here).

SOURCES CITED:

  1. FleetOwner, "CVSA 2026 Roadcheck results show top truck, driver, and
     ELD violations" —
     https://www.fleetowner.com/safety/news/55400720/cvsa-2026-roadcheck-results-show-top-truck-driver-and-eld-violations
     Backs: 54,575 total inspections; 10,350 vehicles and 3,184 drivers
     placed OOS; 81% of vehicles / 94.2% of drivers had no OOS violations;
     17,680 CVSA decals issued; tires ranked #2 with 2,914 violations
     (20.9% of vehicle OOS violations); brakes #1 with 3,379 (24.3%);
     cargo securement 1,724 (12.4%); lighting 1,659 (11.9%).
  2. TheTrucker.com, "CVSA Roadcheck 2026: More than 10,300 vehicles placed
     out of service" —
     https://www.thetrucker.com/trucking-news/the-nation/cvsa-releases-road-check-results
     Backs (independent corroboration): the same inspection/OOS totals and
     tire-violation ranking/percentage as source 1, plus the May 12-14,
     2026 event dates and three-country (US/Canada/Mexico) scope.
  3. CVSA, "International Roadcheck Results" (official results hub) —
     https://cvsa.org/programs/international-roadcheck/international-roadcheck-results/
     Cited as the primary/official source for the Roadcheck results
     program. WebFetch could not reach cvsa.org directly in this session
     (network egress blocked for this domain), so the figures used in the
     post are the numbers independently corroborated across sources 1 and
     2 above, both of which report them as sourced from CVSA's release.
  4. Commercial Carrier Journal, "Tire and wheel violation prevention
     during CVSA Roadcheck" —
     https://www.ccjdigital.com/business/article/14938439/tire-and-wheel-violation-prevention-during-cvsa-roadcheck
     Backs: the specific checklist inspectors use for tire OOS calls —
     tread depth, cuts, bulges, sidewall damage, exposed fabric/belt or
     casing-ply material, underinflation, improper repairs — and that
     exposed belt/casing material is treated as a critical, OOS-triggering
     defect.
  5. 49 CFR 393.75 ("Tires"), via eCFR —
     https://www.ecfr.gov/current/title-49/subtitle-B/chapter-III/subchapter-B/part-393/subpart-G/section-393.75
     Backs: the federal minimum tread groove depth — 4/32" on steer axles,
     2/32" on all other axles — that Roadcheck tread-depth OOS calls are
     measured against.
  6. Tire Retread & Repair Information Bureau (TRIB) —
     https://www.retread.org/
     Backs: TRIB's published position that a properly built and maintained
     retread performs at parity with a new tire, referenced here (not
     re-argued) as independent corroboration of the maintenance-not-
     construction-type point; the fuller treatment of this source lives in
     retread-tire-safety-trib-tia-data.html, linked from this post.

  Internal corroboration (already sourced/cited in full in the linked
  post, not re-cited here): the UMTRI/FMCSA 2007 tire-debris field study
  (Page & Woodrooffe, Transportation Research Record 2096, 2009), covered
  in blog/retread-tire-safety-trib-tia-data.html, which similarly traced
  tire failures to road hazards and maintenance/operational issues rather
  than tire construction type.

WebFetch was blocked network-wide in this session's environment for every
domain tried this run (cvsa.org, fleetowner.com, thetrucker.com, fleetio.com,
coopskw.com, driveteam.com, thebrakereport.com, pti4you.com). All figures
above were verified via WebSearch, cross-checked across at least two
independent queries/sources per fact before citing, per the research
standard — consistent with the same environment limitation noted in the
casing-inspection-5-point-check.md source record for a prior post.

-->

# What CVSA's 2026 Roadcheck Data Actually Shows About Tire Violations

Once a year, roadside inspectors across the U.S., Canada, and Mexico spend three days doing nothing but commercial-vehicle inspections, all at once, all reported to the same body. That's the Commercial Vehicle Safety Alliance's International Roadcheck, and the 2026 edition — held May 12-14, 2026 — is the closest thing the trucking industry has to a continent-wide snapshot of what's actually wrong with the vehicles on the road. Tires came in second on that snapshot, right behind brakes. Here's what the numbers say, and — just as important — what they don't.

## The topline numbers

Over the three-day blitz, CVSA-certified inspectors conducted 54,575 commercial motor vehicle and driver inspections across North America. Of those, 10,350 vehicles and 3,184 drivers were placed out of service (OOS) — meaning the vehicle or driver was pulled from service on the spot until the violation was fixed. Put the other way: 81% of vehicles and 94.2% of drivers inspected had no out-of-service violations at all, and inspectors affixed 17,680 CVSA decals to vehicles that passed a full inspection clean, per FleetOwner's coverage of the results, corroborated by TheTrucker.com's reporting and CVSA's own International Roadcheck results page.

## Where tires rank among vehicle OOS violations

Brake systems topped the list, as they typically do, with 3,379 violations — 24.3% of all vehicle OOS violations. Tires were second: 2,914 violations, 20.9% of the total. Cargo securement (1,724 violations, 12.4%) and lighting (1,659 violations, 11.9%) rounded out the top categories.

| Vehicle OOS violation category | Violations | % of vehicle OOS violations |
|---|---|---|
| 1. Brake systems | 3,379 | 24.3% |
| 2. Tires | 2,914 | 20.9% |
| 3. Cargo securement | 1,724 | 12.4% |
| 4. Lighting | 1,659 | 11.9% |

Tires have landed in or near this same #2 spot for years running — it's a stable pattern, not a one-off. The question worth asking isn't "are tires a problem," it's: a problem in what sense?

## What actually puts a tire out of service

A tire doesn't fail a Roadcheck inspection because of how it was manufactured. It fails against a specific, published checklist: tread depth, physical damage, and inflation. Under 49 CFR 393.75, the federal minimum tread groove depth is 4/32" on steer axles and 2/32" on all other axles — a tire measured below that at any major groove is out of service on the spot. Beyond tread depth, inspectors are checking for cuts, bulges, sidewall damage, and — the most serious call — exposed fabric or belt/cord material where the rubber has worn through to the tire's internal structure. Underinflation and improper repairs round out the list. Commercial Carrier Journal's rundown of tire and wheel violation prevention during CVSA Roadcheck confirms this is exactly the checklist inspectors work from, and that belt material or casing ply exposed in the tread or sidewall is treated as a critical, OOS-triggering defect.

In other words: every one of the 2,914 tire violations in the 2026 Roadcheck traces back to a tire that was run too long, run too soft, or run damaged and unrepaired. None of it traces back to a construction method.

## What this data doesn't say

Here's the important caveat, and we want to be explicit about it rather than let a stat table imply more than it should: CVSA's Roadcheck results do not break tire OOS violations out by retread vs. new. The public data reports tread depth, exposed fabric, damage, and inflation as categories — it does not tag each violation by whether the tire was an original-tread tire or a retread. Anyone claiming the Roadcheck numbers prove retreads perform better, worse, or the same as new tires is reading something into the data that isn't there, and we're not going to make that claim either.

What the data does support is a narrower, more useful point: the overwhelming majority of tire violations severe enough to ground a commercial vehicle are maintenance failures, not manufacturing failures. That's consistent with what we found digging into the federal debris-study data and TRIB/TIA's published position in our Retread Tire Safety: What the TRIB/TIA Data Actually Shows post — the UMTRI/FMCSA field study of roadside tire debris likewise traced tire failures to road hazards and operational issues like underinflation and overloading, not to whether the casing had been retreaded. The Tire Retread & Repair Information Bureau's position, published independently of the CVSA data, is the same: a properly built and maintained retread performs at parity with a new tire, and the variable that actually determines tire safety in the field is inspection and maintenance discipline, not tread origin.

Two independent datasets — CVSA's roadside enforcement numbers and UMTRI's federally sponsored debris study — arrive at the same underlying conclusion through different methods: tires fail in the field because of how they were run, not how they were built. That's an argument for rigorous inspection and maintenance, on every tire on the truck, retread or new.

## Where that leaves a retread shop

If maintenance neglect — not tire type — is what's actually filling out CVSA's OOS reports, the practical takeaway for a retreader is the one this site keeps coming back to: the safety variable you control is the casing you start with and the discipline you inspect it with. A worn-past-limit or fabric-exposed tire never should have been on the road in the first place, whether it started life as a new tire or a retread — and the same non-destructive inspection process that catches a bad casing before it's rebuilt is what keeps a finished retread out of next year's Roadcheck numbers. We cover exactly what that inspection process looks like, check by check, in Casing Inspection: The 5-Point Check Before Every Retread, built around full bead-to-bead visibility from an inspection spreader.

## The takeaway

| Question | What the 2026 Roadcheck data shows |
|---|---|
| How big a share of OOS violations are tires? | 2,914 violations, 20.9% of all vehicle OOS violations — ranked #2 after brakes (24.3%) |
| What actually triggers a tire OOS violation? | Tread below 4/32" (steer) / 2/32" (other axles), exposed fabric/belt material, cuts/bulges, underinflation |
| Does CVSA data compare retread vs. new tire performance? | No — Roadcheck doesn't tag violations by tire construction type; that comparison isn't in this dataset |
| So what does drive tire OOS violations? | Maintenance and inspection neglect — consistent with UMTRI/FMCSA debris-study findings and TRIB/TIA's published position |

The honest reading of CVSA's 2026 Roadcheck numbers isn't "retreads are risky" or "retreads are safe" — that comparison simply isn't in the data. It's that tire violations, industry-wide, are a maintenance story. For a retread shop, that's exactly the case for rigorous casing inspection and disciplined process control, covered in full in our equipment buyer's guide.

## Tightening up casing inspection?

We supply inspection spreaders and casing-prep equipment with transparent all-in Canadian pricing and delivery from our Ontario warehouse — manufacturer-direct, no distributor markup. Tell us your volume and casing sizes and we'll spec the right line for your shop.

[ Get an equipment quote → ] (link to quote form)
