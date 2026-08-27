<!--
TOPIC QUEUE — Good Hope Retreaders blog
The daily routine pops the FIRST unchecked topic each run, writes it, and
checks it off (changes "- [ ]" to "- [x]") in the same PR. Ash/marketing adds
new topics here as they're researched — the routine should never invent a
topic that isn't in this list or in the "already-pending" set the routine
checks for in the repo itself.

Each entry: topic, target keyword + real volume/difficulty (source and date),
and the real, citable fact/trend/source the post should be built around.

HARD RULE — every post ships with a real in-article hero image:
Every post MUST include an in-article hero <img>, not just an og:image
fallback pointing at a reused/generic site image.

HARD RULE — hero images must be realistic, not flat icon/vector graphics
(per Ash's explicit instruction, Aug 2026):
The hero must look like a real, photographic (or photo-real 3D-render)
image — actual tires, casings, equipment, warehouse/shop scenes — dark
moody industrial lighting with an orange accent, the way
retreads-vs-new-tires-cost-per-mile-real.png looks. Do NOT ship a flat
vector/icon graphic (text + thin-line icons on a solid background) as the
hero — that style is retired; posts like casing-inspection-5-point-check-
hero.png and electric-vs-steam-curing-chamber-hero.png predate this rule
and should be treated as needing a realistic-image refresh when convenient,
not as the pattern to copy.

Images must also be topically related to the specific post, not a generic
reused site photo swapped in as a placeholder — e.g. this post (fleets
switching to retreads) uses a real photo of commercial trailer tires plus
a real fleet-truck-on-highway photo, not the site's generic default tread
close-up used elsewhere. Prefer more than one real, relevant photo per
post where the content supports it (a hero plus one supporting in-article
image), rather than a single reused stock shot.

Sourcing order:
1. Canva (primary) — ask for a realistic/photographic result explicitly in
   the prompt, not an icon/vector poster.
2. If Canva fails (quota, etc.), try Adobe Stock (asset_search,
   entityScope StockAsset). Note (learned Aug 26 2026): this account DOES
   have a working free-tier stock entitlement — an earlier run wrongly
   assumed it had none after one narrow query (with contentType/orientation
   /pricing filters combined) returned zero results. If a filtered query
   returns zero, retry with a broader, simpler query (e.g. "semi truck
   tires") before concluding Adobe Stock is unavailable. License with
   asset_license_and_download_stock, then crop/resize with
   image_crop_and_resize (subject-aware focus).
   Known egress quirk: image_crop_and_resize's output URL is hosted on
   photoshop-api.adobe.io, which the sandbox's outbound proxy blocks for
   direct curl/WebFetch download. Workaround: download the ORIGINAL
   licensed image from its S3 presigned URL (asset_license_and_download_
   stock's downloadUrl — that host is not blocked) with curl, then
   replicate the same crop locally using the crop_x/crop_y/crop_width/
   crop_height values from image_crop_and_resize's metadata, via
   `/opt/pw-browsers/ffmpeg-*/ffmpeg-linux` (note: this stripped ffmpeg
   build needs `-f image2pipe -vcodec mjpeg -i pipe:0` piped input, not a
   plain file path, to decode a JPEG).
3. If both Canva and Adobe Stock genuinely fail (verified, not assumed),
   do NOT fall back to a self-authored flat SVG/icon graphic — that
   violates the realism rule above. Instead: publish the post with the
   existing product/site photography as a temporary og:image only, clearly
   flag in the PR description that the bespoke realistic hero is still
   needed, and note which tool(s) failed and why. A human will supply or
   approve the real image before merge. Do not invent a photo-real image by
   hand-coding SVG shapes to look like a photo.
-->

## Pending (already drafted content, not yet in the repo — do these first if missing)

- [x] **Retreads vs. New Tires: What the Cost-Per-Mile Numbers Actually Show**
      Keyword: "retread tires vs new tires" (~50/mo, Semrush US, Aug 2026)
      Anchor fact: retreading runs 35-45% below new-tire cost per lifecycle
      (industry-standard figure); TRIB/TIA publish data showing retread
      failure rates track construction/maintenance quality, not the retread
      process itself.

- [x] **Extruder Guns for Tire Repair: A Buyer's Guide**
      Keyword: "extruder gun" (~90/mo, Semrush US, Aug 2026; Shamrock ranks
      only #25 for this term — winnable)
      Anchor fact: OTR repair typically needs 750W-class guns vs. 400W-class
      for passenger/light-truck — real spec differentiator, not filler.

- [x] **Pre-Cure vs. Mould-Cure Retreading: Which Process Fits Your Shop**
      Keyword: "tire retreading equipment" / "tire retread machine"
      (~20/mo each, Semrush US, Aug 2026)
      Anchor fact: pre-cure dominates independent/mid-size shops because of
      lower capital cost and off-the-shelf tread pattern interchangeability.

## Next up (researched Aug 11, 2026 — real data, not guesses)

- [x] **Retread Tire Safety: What the TRIB/TIA Data Actually Shows**
      Keyword: "retread tire safety" (20/mo, competition 0.05 — low difficulty,
      Ubersuggest US, Aug 11 2026)
      Research angle: directly disarms the "retreads fail on the highway"
      myth with real published failure-rate data from TRIB (Tire Retread &
      Repair Information Bureau) and TIA — cite their actual published
      positions, don't paraphrase from memory. This is named as priority
      objection-handling content in the marketing manual (Section 9).

- [x] **Casing Inspection: The 5-Point Check Before Every Retread**
      Keyword: "tire casing inspection" (low/no measured search volume — this
      is an authority-building piece, not a volume play; still worth doing
      because it's foundational to the cost-per-retread story every other
      post leans on)
      Research angle: what actually disqualifies a casing (structural damage
      types, age, prior repair history) — needs real technical sourcing
      (TRIB/TIA/retread.org process documentation), not invented detail.

- [x] **Why More Fleets Are Switching to Retreads: The Cost & Circular Economy
      Case in 2026**
      Not a keyword play — a trend/news-hook piece.
      Research angle: cite current market growth data (Future Market Insights
      projects the global retread market growing at a steady mid-single-digit
      CAGR through the early 2030s; TechSci Research separately projects
      ~4.28% CAGR through 2031) — pull the actual current figures and report
      names via web research at write-time rather than reusing these numbers
      verbatim, since they should be re-verified as current when the post is
      written. Tie to fleet cost-per-mile pressure and the sustainability
      angle (no new casing manufactured per retread cycle).

## Researched Aug 27, 2026 — 18-topic batch to sustain daily posting
(All facts below were web-researched this date via parallel research passes.
Re-verify each is still current at write-time per the routine's research
standard — treat what's here as a strong starting anchor, not a substitute
for a fresh check. Topics flagged NEEDS SOFTER FRAMING have no single
named-authority (TRIB/TIA) source and must be written with the caveat
intact, not upgraded into a harder claim than the source supports.)

- [ ] **Buffing Machines & Blades: Getting Buffing Texture and Radius Right**
      Keyword: "tire retread buffing texture standard" (no measured volume
      this round — Ubersuggest daily quota was exhausted; re-check when
      quota resets)
      Anchor fact: TIA/TRIB's Tread Rubber & Tire Repair Materials
      Manufacturers' Group (TRMG) publishes RP-01-01 "Tire Profiling for
      Retreading" on tireindustry.org, setting buff radius/crown-width by
      tire size — e.g. Double Coin's published TBR retread spec sheet calls
      for a 26" buff radius (7"/178mm max width) on a 215/75R17.5. Cite the
      RP-01-01 doc and the manufacturer spec sheet directly.

- [ ] **How Ontario's Tire Recycling Regulations Shape the Retread Business
      Case**
      Keyword: "Ontario tire recycling regulations" (no measured volume
      this round)
      Anchor fact: Effective Jan 1 2025, RPRA-administered amendments to
      Ontario's Tires Regulation (under the RRCEA) cut the tire management
      requirement from 85% to 65% (60% for large tires) through 2029,
      rising to 70%/60% from 2030. Source: RPRA, "Summary of recent
      amendments to Ontario's Tires Regulation," March 2025 — verify no
      further amendment has landed before publishing.

- [ ] **Curing Envelopes Explained: Inner vs. Outer, and Why Vacuum
      Integrity Matters**
      Keyword: "curing envelope tire retreading vacuum" (no measured
      volume this round)
      Anchor fact: in pre-cure/envelope retreading, a vacuum is drawn
      between the inner/outer envelopes and the tire before autoclave cure
      specifically to prevent trapped air/steam pockets that cause
      incomplete cushion-gum cure and bond failure — sourced from
      retreading-apparatus patent literature (US6261409, US5007978).
      Cross-check against TRIB's own mold-cure-vs-pre-cure process page at
      write time if it's reachable.

- [ ] **Preventing Zipper Failures and Casing Separation: The Equipment
      Side of Retread Safety**
      Keyword: "tire zipper rupture retreading inspection" (no measured
      volume this round)
      Anchor fact: USTMA's Tire Information Service Bulletin TISB Vol. 33
      directs retreaders to reject any casing with upper-sidewall
      ripples/bulges/porosity/softness and to use non-destructive testing
      (shearography, x-ray) plus a post-cure pressure test before a casing
      re-enters service. Source: ustires.org, TISB 33 PDF. Differentiate
      this from the existing retread-tire-safety-trib-tia-data and
      casing-inspection-5-point-check posts by focusing specifically on
      inspection equipment/technology — cross-link both rather than
      re-covering the same ground.

- [ ] **Bonding Cement & Cushion Gum: What the Application Standard
      Actually Requires**
      Keyword: "cushion gum application retreading" (no measured volume
      this round)
      Anchor fact: TIA's TRMG maintains a named recommended practice,
      "Classification and Application of Cushion Gum" (tireindustry.org),
      governing cushion-gum grade and application procedure. Cite the
      standard's existence/title as the authority hook — do NOT state a
      specific cure time/temperature number, since none was verifiable
      from a public non-paywalled source this round; point readers to
      manufacturer cure charts instead.

- [ ] **OTR Retreading: Why Mining and Construction Fleets Are a Different
      Market**
      Keyword: "OTR tire retreading mining" (no measured volume this
      round)
      Anchor fact: a single giant mining tire (e.g. 59/80R63 for
      ultra-class haul trucks) costs roughly $35,000-$42,000 new (Modern
      Tire Dealer, "Big Horn Tire" feature) — an order of magnitude past
      truck/bus tire economics. Global Market Insights' OTR Tire Market
      report notes mining/industrial fleets increasingly retread
      specifically to stretch casing life given that cost.

- [ ] **Skiving Stations: Why Repair Prep Determines Bond Strength**
      Keyword: "tire skive repair procedure standard" (no measured volume
      this round)
      Anchor fact: TIA-aligned repair training standards cap puncture
      repairs at 1/4" (6mm), require two-piece repairs above a 25° injury
      angle, and specify a cupped "Y"-type 90° skive through steel belts
      for crown repairs. Cite TechTireRepairs' and PREMA's published
      training guides plus TIA/tireindustry.org glossary material.

- [ ] **Retreading Regulations in Canada: What CVSA Roadside Inspection
      Actually Requires**
      Keyword: "CVSA out of service criteria retread tires Canada" (no
      measured volume this round)
      Anchor fact: CVSA's 2025 International Roadcheck made tires the
      year's inspection focus — 2,899 tire-related out-of-service
      violations, 21.4% of all vehicle OOS violations (cvsa.org, May
      2025); CVSA's North American OOS Criteria set steer-axle tread
      depth at 2/32" vs 1/32" elsewhere. IMPORTANT CAVEAT: the "no
      retreads on steer axles" rule is a US FMCSR rule (49 CFR 393.75),
      NOT a Transport Canada rule — Transport Canada's framework (SOR/2013
      -198, TSD 120) governs manufacture/import, and Ontario roadside
      enforcement runs through O.Reg 199/07 plus the CVSA standard. The
      post must reflect this precisely and never claim Transport Canada
      bans retreads on steer axles.

- [ ] **White Oxide Stones & Finishing Abrasives: Meeting the Industry
      Buff-Texture Standard**
      Keyword: "tire buffing texture standards" (no measured volume this
      round)
      Anchor fact: TRMG's RP-01/02-23 ("BTS6") defines six
      industry-approved buff-texture classifications used across
      retread/repair, jointly hosted by TRIB and TIA (tireindustry.org) —
      corroborated by Tire Review and Tire Business 2020 coverage of the
      standard's update. (Note: the Buffing Machines & Blades post above
      leans on RP-01-01 buff-radius specs — keep these two posts'
      citations distinct rather than both centering on BTS6.)

- [ ] **Small Consumables That Make or Break a Retread: Flaps, Stems, and
      Seals**
      Keyword: "tire flap failure retread" (no measured volume this
      round)
      Anchor fact: OSHA's "Servicing Multi-Piece and Single-Piece Rim
      Wheels" (OSHA 3584) states rim-wheel-servicing hazards are "greatly
      increased" on multi-piece rims and tires inflated to 45+ psi, with
      failures capable of causing fatal injury (29 CFR 1910.177/
      1917.44(o)). Build the post around this verified safety-compliance
      angle — a TRIB-specific casing-rejection failure-rate stat was
      searched for but not found publicly this round, so don't invent one.

- [ ] **Camelback Tread Rubber: Compound and Tread Pattern Selection for
      Precure Retreading**
      Keyword: "camelback tread rubber precure retreading" (no measured
      volume this round)
      Anchor fact: pre-cure remains the dominant retread process — Future
      Market Insights' "Retread Tire Market" report and Market.us both
      track pre-cure's continued majority share of the process segment,
      though exact share figures vary by vendor (one cites ~68%, another
      ~61%). Cite one specific named report and its stated figure — don't
      average conflicting vendor numbers into a single "consensus" claim.

- [ ] **Retread Warranty Basics: What Voids Coverage and What Doesn't**
      Keyword: "retread tire warranty" (no measured volume this round)
      Anchor fact: Bandag/Bridgestone's current Limited Lifetime National
      Warranty covers workmanship/material defects for the life of the
      tread but caps casing-defect coverage at just two years, separate
      from lifetime tread coverage (commercial.bridgestone.com PDF).
      Frame as "what a major retreader's actual current warranty document
      says," not as TIA-authored policy — no single TIA warranty fact
      sheet was found.

- [ ] **Dust Collection & Shop Air Quality: Combustible Dust Compliance
      for Retreaders**
      Keyword: "combustible dust tire buffing NFPA" (no measured volume
      this round)
      Anchor fact: OSHA's Combustible Dust National Emphasis Program (CPL
      03-00-006) flags rubber buffing/grinding dust as a fire/
      deflagration hazard under NFPA 654 guidance — a dust layer just
      1/32" thick over 5% of a room's surfaces can fuel a secondary
      explosion. CCOHS provides the parallel Canadian housekeeping
      guidance (wet methods/approved vacuums only, no dry sweeping or
      compressed air).

- [ ] **Choosing a Retread Equipment Supplier: An Evaluation Checklist**
      Keyword: "retread equipment supplier" (no measured volume this
      round)
      Anchor fact: precure retreading lines run roughly 20-30% lower
      capital cost than full mold-cure setups, which is why precure is
      projected to hold ~67% of the process-method market in 2026 even as
      mold-cure gains ground on a 5.88% CAGR from improved automated
      presses (The Business Research Company's "Tire Curing Press Market
      Report 2025," cross-checked against Mordor Intelligence). Cite as
      industry market analysis, not a trade-body standard; never name a
      specific competitor or cite private pricing.

- [ ] **Rasp Blade Design: Why Radial Casings Buff Differently Than
      Bias-Ply**
      Keyword: "rasp blade radial vs bias tire retread" (no measured
      volume this round)
      NEEDS SOFTER FRAMING — no TIA/TRIB document formally codifies rasp
      type by casing construction. The citable material is engineering
      rationale: rasp-blade patents (US6789982, WO2004024382A1) and
      manufacturer literature (B&J Rocket's channel-cooled "Super Cool"
      blades) explain that radial casings' steel-belt exposure during
      buffing generates more frictional heat than bias-ply, driving
      blade-geometry/cooling differences that protect bond quality. Write
      this as engineering rationale, never as an "official standard."

- [ ] **Preventive Maintenance Schedules for Curing Chambers and Buffing
      Machines**
      Keyword: "curing chamber preventive maintenance schedule" (no
      measured volume this round)
      NEEDS SOFTER FRAMING — no TRIB/TIA-published PM schedule specific to
      retread curing chambers/buffers was found. Usable substitutes:
      Melion Industry's published curing-chamber user instructions (daily
      door-seal cleaning, monthly locking-ring re-greasing, periodic
      pressure-bleed-valve checks) plus general manufacturing
      downtime-cost data (Aberdeen Research: ~$260K/hour average
      unplanned downtime across manufacturing). Disclose these as
      illustrative examples, not an industry-wide retread standard.

- [ ] **How Many Times Can a Truck Tire Casing Be Retreaded? Casing
      Life-Cycle Economics**
      Keyword: "how many times can a tire be retreaded" (no measured
      volume this round)
      Anchor fact: TRIB/retread.org states long-haul casings typically go
      2-3 retread cycles (short-haul/local casings 5+ with proper
      maintenance); two cycles roughly triples a casing's productive
      output vs. one, three cycles roughly quadruples it; retreads
      typically sell for 30-50% of a comparable new tire (as low as ~25%
      on a fleet-supplied casing); retreading saves the US trucking
      industry over $3B annually. Cite retread.org's "Learn More" page
      directly, corroborated by Bandag/Bridgestone's "Cost & Savings of
      Retread Tires" page. Differentiate from the existing
      retreads-vs-new-tires-cost-per-mile post (that one's about
      cost-per-mile comparison; this one's about cycle-count economics) —
      cross-link both.

- [ ] **The Retread Investment Case: What the Cost-Savings Data Actually
      Shows**
      Keyword: "retread equipment payback period ROI" (no measured volume
      this round)
      NEEDS SOFTER FRAMING — no trade-press or industry source gave a
      sourced, retread-equipment-specific payback-period figure (the
      "1-3 year payback" numbers that surface in search trace to generic
      equipment-ROI-calculator sites, not retread-specific research — do
      not cite those). What is well-sourced: USTMA states retreads
      typically cost 30-50% less than comparable new tires, and ~15M
      tires are retreaded annually in the US supporting ~51,000 jobs in a
      ~268,000-job tire ecosystem (ustires.org/tire-retreading); real
      named capex activity exists too (Bridgestone's ~$60M Abilene Bandag
      retread-plant expansion, per Tire Business capex coverage). Build
      the ROI case around these verified cost/scale figures, never an
      invented payback-period number.
