# Shearography, X-Ray, and NDT: How the Industry Actually Inspects a Casing Before It's Retread

Pillar: A (Product/equipment education)
Published: 2026-09-17

## Premise
Our existing post `casing-inspection-5-point-check.html` covers the manual visual/tactile
5-point check every shop should run. This post goes one layer deeper: the non-destructive
testing (NDT) technology — shearography, X-ray, ultrasound — that large retreaders and
TRIB-certified plants use to catch internal defects (like belt separations) that a trained
eye and hand cannot detect. Framed honestly: this is high-end plant-scale equipment, not
something Good Hope sells or claims independent shops need to buy. The point is education
+ context, closing with why rigorous visual/tactile inspection (our inspection spreader,
the 5-point check) remains the right foundation for independent and mid-size shops, with
NDT as the upgrade path at larger scale.

## Sources (verified via web search, September 17, 2026)
1. Shearography mechanism (vacuum-induced deformation, laser interferometry) — Smithers,
   "Tire Shearography" (smithers.com/industries/transportation/tire-wheel/tire-testing/tire-shearography)
2. ZEISS Optotechnik INTACT 1360-X shearography system — detects separations, blisters,
   undercuring; full bead-to-bead scan in ~55 seconds including load/unload; catches
   foreign-material inclusions X-ray can miss — optotechnik.zeiss.com/en/products/tire-testing-intact/retreading;
   corroborated by Metrology News, "Gone In 55 Seconds — High Speed Optical Tire Inspection
   System launched" (metrology.news)
3. Belt separations are typically hidden inside the belt package and not detectable by
   visual/tactile inspection alone; retreaders (e.g., Marangoni) use shearography to find
   them — McCarthy Tire Service, "Retreading" (mccarthytire.com/commercial-vehicle-services/retreading);
   corroborated by Commercial Carrier Journal, "Retreads unwrapped" (ccjdigital.com/business/article/14900267/retreads-unwrapped)
4. X-ray/radiography capability and limits — real-time, high sensitivity to foreign
   material and porosity; sensitivity depends on material density, so subtler bonding
   irregularities can be harder to catch than with shearography — general industry
   synthesis corroborated across Tire Review (tirereview.com) and USPTO patent
   documentation on tire NDT methods
5. TRIB-certified retreaders use shearography or X-ray on every casing before retreading
   as a certification requirement — Heavy Vehicle Inspection, "Retread Tire Safety
   Inspection Checklist for Commercial Fleets" (heavyvehicleinspection.com/blog/post/retreaded-tire-safety-inspection-checklist)
6. Michelin Retread Technologies' Casing Integrity Analyzer (CIA) — proprietary
   shearography + software, deployed in 100% of MRT plants; quote from Tom Brennan,
   president of Michelin Retread Technologies — business.michelinman.com/michelin-retread-technologies
7. Michelin TreadVision launch (March 2026) — AI-powered automated classification of
   Casing Integrity Analysis (shearography) results for more consistent, objective quality
   control — michelinmedia.com press release; corroborated by Trucks, Parts, Service
   (truckpartsandservice.com), Retreading Business (retreadingbusiness.com), and
   Aftermarket News (aftermarketnews.com)

## Duplicate check
Searched `blog/` for existing NDT/shearography/X-ray content — none found.
`casing-inspection-5-point-check.html` covers manual inspection only; this post is
explicitly framed as the complementary "what's above that" piece and cross-links to it.
No open PRs at time of writing duplicate this topic.

## Hero image
Canva was unavailable this run (requires OAuth authorization that can't be completed in
a non-interactive session). Fell back to Adobe Stock per the sourcing order: licensed a
real photograph (Adobe Stock asset 1091817403, "Semi Truck Mechanic Inspecting Vehicle
Tire During Daytime Repair in Urban Area", Nikon D850 photo) via asset_license_and_download_stock,
cropped to the site's 1280x720 hero ratio with image_crop_and_resize (subject-aware),
downloaded via the known photoshop-api.adobe.io egress-block workaround (re-crop the
original S3 download locally with ffmpeg using the tool's returned crop coordinates).
