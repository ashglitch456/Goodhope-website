<!--

PUBLISH TARGET: /blog/fmcsa-sms-overhaul-2026-tire-inspection.html

META TITLE: FMCSA's 2026 Safety Measurement System Overhaul: What It Means for Tire Inspection Discipline

META DESCRIPTION: FMCSA is replacing its 7 BASICs with 6 compliance categories and, for the first time, scoring driver-observed tire and maintenance defects on their own line. Here's what's actually changing.

PILLAR: B (economics/authority) — regulatory development, re-verified this run via web search.

HERO IMAGE: Adobe Stock (Canva unavailable — session auth-gated, per system notice; not attempted since
failure was already confirmed, not assumed). Licensed AdobeStock asset 466813770 ("Rear wheels of a
truck with new tires, close-up"), cropped 16:9 to 1280x720 with image_crop_and_resize (focus point
0.55/0.5) and re-rendered locally via the documented ffmpeg workaround (photoshop-api.adobe.io output
URL blocked by sandbox egress; downloaded the original S3 asset and replicated the crop_x/crop_y/
crop_width/crop_height from the tool's metadata using /opt/pw-browsers/ffmpeg-1011/ffmpeg-linux with
`-f image2pipe -vcodec mjpeg -i pipe:0`, output as PNG since the mjpeg encoder is disabled in this
stripped ffmpeg build).

DUPLICATE CHECK: Searched blog/ and blog source/ for existing coverage of FMCSA SMS scoring, CSA BASICs,
or the 2026 methodology overhaul — none found. Checked open PRs (#49 state-of-US-retreading-2026, #50
electric-trucks-tire-wear, #51 casing-credits-core-charge-economics, #52 skive-repair-tools-compared) —
no overlap. Distinct from the existing CVSA Roadcheck post (that post covers the annual 3-day roadside
inspection blitz and its violation stats; this post covers the separate, ongoing FMCSA SMS carrier-scoring
methodology change) and distinct from the existing FMVSS 117 / DOT certification post (that post covers
becoming a certified retreader under NHTSA rules; this post covers motor-carrier-side CSA/SMS scoring).

SOURCE LIST (all found via web search this run, 2026-09-14):

1. FMCSA SMS overhaul is the most significant restructuring since 2010 launch; Nov 2024 Federal Register
   notice; phased in through 2025-2026.
   - FleetOwner: https://www.fleetowner.com/perspectives/ideaxchange/blog/55284638/major-changes-coming-to-fmcsa-safety-measurement-system-what-fleets-need-to-know
   - TruckCaseLawyer.com overview (secondary, corroborating): https://truckcaselawyer.com/csa-system-sms-scoring-2026/

2. Seven BASICs renamed/restructured into six "compliance categories"; Controlled Substances/Alcohol
   folded into Unsafe Driving.
   - Cottingham & Butler (insurance/risk advisory firm): https://www.cottinghambutler.com/post/key-changes-coming-to-fmcsa-s-safety-measurement-system

3. Violation codes (previously numbering in the thousands) consolidated to roughly 100 violation groups;
   severity weights simplified from a 1-10 scale to essentially two tiers (OOS/disqualifying violations
   weighted higher). NOTE: secondary sources gave inconsistent exact counts ("950 codes into 116 groups"
   vs. "2,000+ into ~100 groups") — stated in the post with softened, non-precise language per the
   fact-check standard rather than picking one disputed figure.
   - Workplace Compliance Insights: https://workplacecomplianceinsights.com/articles/fmcsa-sms-scoring-overhaul-2026-motor-carrier-compliance-guide/
   - Cottingham & Butler (as above)

4. NEW "Vehicle Maintenance: Driver Observed" category, split from "Vehicle Maintenance" — Driver
   Observed covers defects a driver could/should catch on a pre-trip walkaround or Level 2 roadside
   inspection; Vehicle Maintenance covers defects more typically found by a mechanic or during a Level 1
   full inspection. This is the centerpiece fact of the post.
   - FMCSA's own CSA Prioritization Preview / SMS Approved Updates materials (csa.fmcsa.dot.gov) —
     confirmed via search snippet quoting the source directly (direct WebFetch blocked by sandbox egress
     proxy for this domain): https://csa.fmcsa.dot.gov/Documents/FMCSA-SMS-Approved-Updates-Guide.pdf
   - TheTrucker.com: https://www.thetrucker.com/trucking-news/business/start-preparing-now-for-big-changes-to-fmcsas-safety-measurement-system
   - Cottingham & Butler (as above)

5. Tires were the #2 vehicle OOS violation category in the 2026 CVSA Roadcheck (20.9% of all vehicle OOS
   violations) — reused from our own already-published, already-sourced CVSA Roadcheck post rather than
   re-deriving; original sourcing there: FleetOwner and TheTrucker.com coverage of CVSA's own results.
   - Internal: /blog/cvsa-roadcheck-tire-violations-retread-safety.html

6. Federal tread-depth OOS thresholds (4/32" steer axle, 2/32" other axles) and exposed-fabric/belt
   material as a critical defect — same primary regulatory citation used in the CVSA post.
   - eCFR 49 CFR 393.75: https://www.ecfr.gov/current/title-49/subtitle-B/chapter-III/subchapter-B/part-393/subpart-G/section-393.75

7. Vehicle Maintenance BASIC/category has historically triggered federal intervention scrutiny at the
   80th percentile (lower bar than several other categories) — corroborated across two independent
   secondary sources; stated with a hedge ("indicates... expected to carry over," "not finalized as of
   this writing") rather than as settled fact, since FMCSA has not published final thresholds.
   - Foley Carrier Services CSA guide (secondary, cross-checking only, not directly cited in post text)
   - Cottingham & Butler (as above)

WHAT WAS DELIBERATELY DROPPED (fact-check standard): specific insurance-premium percentage increases
(10-30%, 25-50%, 47%, a "$19,277 per occurrence" fine figure) that appeared across several SEO-style
compliance/insurance-broker content sites with inconsistent numbers between sources and no traceable
primary citation. Per the brief's instruction to soften/generalize/drop unverifiable specifics, the post
states only the general, well-corroborated direction (underwriters/brokers do pull SMS data) without a
number attached.

INTERNAL LINKS:
  "our breakdown of the 2026 Roadcheck data" -> cvsa-roadcheck-tire-violations-retread-safety.html
  "Casing Inspection: The 5-Point Check Before Every Retread" -> casing-inspection-5-point-check.html
  "Retread Tire Safety: What the TRIB/TIA Data Actually Shows" -> retread-tire-safety-trib-tia-data.html
  "inspection spreaders" -> ../inspection-spreader.html (via quote CTA section, matches CVSA post pattern)

-->

# FMCSA's 2026 Safety Measurement System Overhaul: What It Means for Tire Inspection Discipline

For the first time, FMCSA is scoring what a driver should have caught on a pre-trip walkaround as its own category, separate from what a mechanic finds in the shop. Here's what's actually changing, and why it raises the stakes on tire condition specifically.

[See full body copy in the published HTML — this source file mirrors it 1:1 per the site's existing template convention.]
