---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 168 items, 20 important content pieces were selected

---

**AI News**
1. [Meta FAIR and NYU study of 200+ MLLMs finds encoder pretraining optional, vision-only parameters required](#item-ai-news-1) ⭐️ 7.0/10

**Technology News**
1. [ULA&\#x27;s Vulcan rocket fails minutes after liftoff, destroying 40 Amazon satellites](#item-tech-news-1) ⭐️ 9.0/10
2. [Is bad news for Jensen Huang also bad news for the AI industry?](#item-tech-news-2) ⭐️ 7.0/10
3. [NVIDIA board faces 108,000-signature petition to reinstate Jensen Huang; Microsoft 365 recovers after 19-hour outage](#item-tech-news-3) ⭐️ 7.0/10

**Medical News**
1. [Tirzepatide Cuts BMI in Adolescents With Obesity in Phase III Trial](#item-medicine-news-1) ⭐️ 8.0/10

**Astronomy News**
1. [Dead Star Spinning Every 8 Minutes Emits Mysterious Radio Pulses](#item-astronomy-news-1) ⭐️ 7.0/10
2. [Euclid reveals record ~15,000 candidate strong gravitational lenses](#item-astronomy-news-2) ⭐️ 7.0/10
3. [Reanalysis finds no evidence for overmassive black hole in galaxy UHZ1](#item-astronomy-news-3) ⭐️ 7.0/10
4. [Simulations Offer Explanation for Uranus and Neptune&\#x27;s Tilted Magnetic Fields](#item-astronomy-news-4) ⭐️ 6.0/10

**Aerospace News**
1. [ULA&\#x27;s Vulcan rocket fails in flight, destroying 40 Amazon Leo satellites](#item-aerospace-news-1) ⭐️ 9.0/10

**Chemical Products and Polymer Markets**
1. [Sipchem Completes $169M Propylene and PP Expansion at Al Waha](#item-chem-products-1) ⭐️ 6.0/10

**Energy News**
1. [Darlington&\#x27;s First BWRX-300 SMR to Exceed C$7.7 Billion Budget and Miss 2030 Target](#item-energy-news-1) ⭐️ 6.0/10

**Oil and Gas Industry News**
1. [Kazakhstan Oil Output Falls Sharply After Drone Attacks Force Export Terminal Closure](#item-oil-gas-news-1) ⭐️ 7.0/10
2. [£2.1 billion Jackdaw gas field begins production in UK North Sea](#item-oil-gas-news-2) ⭐️ 7.0/10

**Literature News**
1. [M. John Harrison&\#x27;s &\#x27;The End of Everything&\#x27; Wins 2026 Booker Prize](#item-literature-news-1) ⭐️ 9.0/10
2. [Editors Reassess the Real Patricia Highsmith Ahead of Helen Mirren Film](#item-literature-news-2) ⭐️ 7.0/10
3. [New York Times Reviews Louise Kennedy&\#x27;s Novel &\#x27;Stations&\#x27;](#item-literature-news-3) ⭐️ 6.0/10
4. [Tiffany Watt Smith on Fleeting Friendships and the Russian Poputchik](#item-literature-news-4) ⭐️ 5.0/10
5. [Literary Agents Turn Themselves Into the Product via Newsletters](#item-literature-news-5) ⭐️ 5.0/10
6. [AO3 Comes Back Online After More Than Two Weeks of Downtime](#item-literature-news-6) ⭐️ 4.0/10

---

## AI News

<a id="item-ai-news-1"></a>
### [Meta FAIR and NYU study of 200+ MLLMs finds encoder pretraining optional, vision-only parameters required](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 7.0/10

Researchers from Meta FAIR and NYU trained more than 200 multimodal LLMs from scratch under a shared compute budget to test which parts of a standard vision encoder actually matter. Their findings: separate encoder pretraining is optional — encoders pretrained with contrastive, self-supervised, and captioning objectives at best tie a from-scratch encoder at matched compute, and extending MetaCLIP pretraining 6.5x raised ImageNet linear-probe accuracy from 80.4% to 84.4% without improving VQA. Vision-only parameters are required — encoder-free models trail at every backbone size from 0.6B to 6.4B and need roughly 3x the compute to catch up, while allocating those parameters to the LLM improves text performance but not VQA. Placement before the LLM is also optional: an in-fusion design adding zero-initialized vision-only weights to the LLM&\#x27;s first 8 layers matches a separate encoder from 1.7B to 6.4B scale with about 13% lower time to first token, and at 1.7B reaches 45.0 VQA versus 44.4 for a separate encoder \(42.3 when text shares the parameters, 35.1 when placed in the last 8 layers\). Evaluations use 16 Cambrian VQA benchmarks at 448 px and 12 language benchmarks; details rest on the authors&\#x27; paper and self-reported results, and the post includes an author disclosure.

reddit · r/MachineLearning · /u/trungh98 · Nov 15, 17:38

**「Background」** Multimodal LLMs have conventionally used a separately pretrained vision encoder \(e.g., a contrastively trained model like MetaCLIP\) whose parameters are shared only with vision tokens and whose outputs are injected before the LLM. Because published models differ in data and compute budgets, labs have recently reached conflicting conclusions — Gemma 4 12B dropped its encoder, Kimi K3 trains one from scratch, and Inkling 2 Small reintroduced an encoder — leaving the design question unsettled. The standard encoder bundle conflates three separable choices: separate pretraining, vision-only parameters, and placement relative to the LLM, which is what this study isolates.

**「Why it matters」** For practitioners designing multimodal models, the results suggest the pretraining budget for a separate vision encoder \(e.g., a contrastive CLIP-style model\) can be redirected to multimodal training without loss at matched compute, provided vision tokens retain dedicated parameters. The in-fusion result also offers a concrete latency benefit — about 13% lower time to first token at parity quality from 1.7B to 6.4B — though the study covers 0.6B–6.4B backbones and 448 px evaluation, so extrapolation to larger or higher-resolution systems is unverified.

**Tags**: `#multimodal`, `#vision-encoders`, `#ablation-study`, `#model-training`, `#MLLMs`, `#open-research`

---

## Technology News

<a id="item-tech-news-1"></a>
### [ULA&\#x27;s Vulcan rocket fails minutes after liftoff, destroying 40 Amazon satellites](https://arstechnica.com/space/2026/11/vulcan-rocket-fails-during-launch-dealing-major-blow-to-spacex-competitors/) ⭐️ 9.0/10

A United Launch Alliance Vulcan rocket failed minutes after liftoff on Sunday, and the vehicle and its payload of 40 Amazon Leo broadband satellites fell back to Earth. The failure is expected to ground the rocket indefinitely, disrupting a vehicle contracted to launch roughly half of the US military&\#x27;s national security space missions in the next few years. The lost mission was the first of 38 Vulcan launches booked by Amazon to build out its broadband constellation, which is intended to compete with SpaceX&\#x27;s Starlink. Vulcan had previously overcome strap-on solid rocket booster failures on two of its four prior flights, each triggering months-long reviews before flights resumed.

rss · Ars Technica · Nov 15, 23:11

**「Background」** Vulcan is United Launch Alliance&\#x27;s newer launch vehicle, developed partly to replace the retired Atlas V and to carry national security missions without Russian-made engines; it is contracted for roughly half of upcoming US military space launches. Until now, the rocket had completed four flights without losing a payload, though two of those missions experienced strap-on solid rocket booster failures that Vulcan&\#x27;s flight software corrected in flight, each followed by months-long investigations before ULA was cleared to fly again. The Amazon Leo constellation, formerly Project Kuiper, is Amazon&\#x27;s planned broadband satellite network competing with SpaceX&\#x27;s Starlink, and this mission was the first of 38 Vulcan launches Amazon had booked to build it out.

**「Why it matters」** US national security launch schedules and Amazon&\#x27;s satellite deployment timeline both depend on Vulcan availability, so an indefinite grounding will force delays or re-planning for missions already on the manifest. Organizations with payloads booked on Vulcan should expect schedule uncertainty while the failure investigation runs, as previous booster incidents led to months-long pauses before the rocket returned to flight.

**Tags**: `#space`, `#ULA`, `#Vulcan rocket`, `#launch failure`, `#Amazon Leo`

---

<a id="item-tech-news-2"></a>
### [Is bad news for Jensen Huang also bad news for the AI industry?](https://techcrunch.com/2026/11/15/is-bad-news-for-jensen-huang-also-bad-news-for-the-ai-industry/) ⭐️ 7.0/10

TechCrunch&\#x27;s Equity podcast discusses Jensen Huang&\#x27;s ouster as Nvidia CEO and what it means for Nvidia&\#x27;s role in the AI economy and its ecosystem investments.

rss · TechCrunch · Nov 15, 21:56

**Tags**: `#nvidia`, `#ai-industry`, `#leadership`, `#techcrunch-equity`, `#business-news`

---

<a id="item-tech-news-3"></a>
### [NVIDIA board faces 108,000-signature petition to reinstate Jensen Huang; Microsoft 365 recovers after 19-hour outage](https://sspai.com/post/119119) ⭐️ 7.0/10

A public letter demanding NVIDIA restore Jensen Huang as CEO and guarantee due process has gathered over 108,000 signatures as of the afternoon of November 14, including more than 58,000 shareholders and over 5,600 current employees, with signatories including Elon Musk and Y Combinator&\#x27;s Garry Tan. Forbes analysis attributes Huang&\#x27;s swift removal to NVIDIA&\#x27;s single-class share structure from its 1999 IPO: Huang holds only 3.6% of shares and voting power, less than half of institutional holders like BlackRock or Vanguard, and the company has no succession plan. Separately, Microsoft confirmed that Microsoft 365 fully recovered around 19 hours after a global outage beginning November 12 that affected about 20 services including Outlook, Teams, and Copilot across more than 70 countries; Microsoft attributed the failure to a technical issue introduced by a recent upgrade, with reports indicating the Exchange service exhausted resources on server startup.

rss · 少数派 · Nov 15, 23:24

**「Background」** Jensen Huang resigned as Nvidia&\#x27;s president, CEO, and board member effective immediately on November 12, 2026, following reports of extramarital affairs, with CFO Colette Kress named interim CEO. The current backlash centers on Nvidia&\#x27;s 1999-era one-share-one-vote structure: unlike the dual-class share arrangements popularized by Google&\#x27;s 2004 IPO, which let founders retain super-voting stock and control, Huang holds only 3.6% of shares and votes—less than half of institutional holders like BlackRock or Vanguard—so the board could force out the co-founder without shareholder consent.

**「Practical impact on affected users」** Organizations that depend on Microsoft 365 faced concrete disruption: governments, courts, and healthcare providers in multiple countries delayed proceedings and medical procedures, companies postponed earnings reports and internal actions, and many fell back on phone and paper communications. Given that replacement office workflows carry high switching costs, analysts expect Microsoft&\#x27;s market position to hold in the short term, but businesses assessing resilience may want to review contingency plans for prolonged cloud productivity-suite outages.

**「Community Reaction」** No substantive community discussion is available for this item.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/live/2026/11/12/business/nvidia-jensen-huang-resigns">Nvidia Updates: Huang ’s Resignation Reverberates Through...</a></li>
<li><a href="https://www.youtube.com/watch?v=1TD49xVjtjE">Who Is Kimberly Powell? Behind Jensen Huang &#x27;s Resignation</a></li>
<li><a href="https://en.wikipedia.org/wiki/2026_Microsoft_outage">2026 Microsoft outage - Wikipedia</a></li>
<li><a href="https://uptimerobot.com/reports/microsoft-365-outage-november-2026/">Microsoft 365 Outage, November 2026: What Happened | UptimeRobot</a></li>
<li><a href="https://www.on-sitetechnology.com/microsoft-365-outage-november-2026/">Microsoft 365 and Outlook Outage, Nov 12, 2026: Timeline</a></li>

</ul>
</details>

**Tags**: `#nvidia`, `#corporate-governance`, `#microsoft-365`, `#outage`, `#tech-industry`

---

## Medical News

<a id="item-medicine-news-1"></a>
### [Tirzepatide Cuts BMI in Adolescents With Obesity in Phase III Trial](https://www.medpagetoday.com/meetingcoverage/obesityweek/123891) ⭐️ 8.0/10

The phase III SURMOUNT-ADOLESCENTS trial showed tirzepatide reduced BMI by 18.5% versus a 0.5% increase with placebo at 72 weeks in adolescents with obesity.

rss · MedPage Today · Nov 15, 23:00

**Tags**: `#obesity`, `#tirzepatide`, `#pediatrics`, `#phase III trial`, `#GLP-1/GIP`, `#SURMOUNT-ADOLESCENTS`, `#JAMA`

---

## Astronomy News

<a id="item-astronomy-news-1"></a>
### [Dead Star Spinning Every 8 Minutes Emits Mysterious Radio Pulses](https://www.sciencedaily.com/releases/2026/11/261114202136.htm) ⭐️ 7.0/10

Astronomers report a stellar pair more than 5,000 light-years away in which a dead star spinning once every eight minutes emits mysterious radio pulses while orbiting a Sun-like companion star. The observations also revealed massive magnetic storms on the companion star. The source does not specify the instrument or observing method, the exact spin and distance uncertainties, whether the radio pulses represent a confirmed detection or a candidate signal, or the peer-review status of the finding. The eight-minute rotation with coherent radio emission in a binary is unusual and may point to a rare white dwarf pulsar-type system, though this interpretation is not confirmed in the source material.

rss · ScienceDaily Astronomy · Nov 15, 13:04

**「Background」** The dead star in this binary is likely a white dwarf — the dense, Earth-sized remnant left after a Sun-like star sheds its outer layers — and a small class of rapidly rotating, strongly magnetized white dwarfs, exemplified by AR Scorpii, is known to beam coherent radio pulses like conventional neutron-star pulsars. The 8-minute spin period places this object among the slow-rotating members of that class, and according to Phys.org the study, &quot;A long-period transient with a Sun-like companion,&quot; was published in Nature Astronomy, marking the first detection of radio pulses from a white dwarf orbiting a Sun-like star.

<details><summary>References</summary>
<ul>
<li><a href="https://phys.org/news/2026-11-rare-star-emits-radio-minutes.html">A rare star system emits radio signals every 8 minutes - Phys.org</a></li>

</ul>
</details>

**Tags**: `#radio astronomy`, `#white dwarf`, `#binary system`, `#pulsar`, `#stellar magnetism`

---

<a id="item-astronomy-news-2"></a>
### [Euclid reveals record ~15,000 candidate strong gravitational lenses](https://phys.org/news/2026-11-dark-matterhunting-satellite-euclid-reveals.html) ⭐️ 7.0/10

The Euclid space telescope has revealed roughly 15,000 potential strong gravitational lenses, the largest collection of such objects to date, with researchers from the University of British Columbia contributing to the effort. Strong lenses occur where a massive foreground object, including its dark matter halo, gravitationally magnifies and distorts the light of a background galaxy, acting as a cosmic magnifying glass. The objects are candidates, not yet confirmed detections, and will require follow-up verification. No sky-facing access conditions apply since these detections come from Euclid survey data rather than a time-sensitive observing event.

rss · Phys.org Space · Nov 15, 20:00

**「What strong gravitational lenses are」** Strong gravitational lensing occurs when the gravity of a massive foreground object, such as a galaxy, warps and magnifies the light of a more distant background source, often producing arcs, rings, or multiple images. Because the deflection depends on all the mass in the foreground system, including invisible dark matter, these lenses let astronomers weigh dark matter distributions and test models of galaxy structure with high precision. Before this release, known strong lens samples numbered only in the hundreds to low thousands, which is why a catalog of roughly 15,000 candidates from a single space survey represents a step change in scale; the objects remain candidates until follow-up observations confirm them.

**「Impact」** The candidate catalog gives astronomers a far larger sample of strong lenses than previously available, providing a powerful new toolset for probing the distribution of dark matter in foreground galaxies through follow-up observations and lensing modeling.

**Tags**: `#gravitational lensing`, `#dark matter`, `#Euclid`, `#survey results`, `#dataset release`

---

<a id="item-astronomy-news-3"></a>
### [Reanalysis finds no evidence for overmassive black hole in galaxy UHZ1](https://phys.org/news/2026-11-evidence-outsize-black-hole-early.html) ⭐️ 7.0/10

A reanalysis led by Fan Zou of the University of Michigan finds no evidence for the heavily dust-obscured, overmassive black hole previously claimed in the high-redshift galaxy UHZ1, using existing X-ray data and new infrared observations. The original 2023 claim had presented UHZ1 as an unusually massive black hole formed through direct collapse early in cosmic history. The new study, published in The Astrophysical Journal on Oct. 14, reports no signs of hidden black hole activity and instead suggests UHZ1 may be a low-mass, metal-poor, star-forming galaxy. This is a reinterpretation of existing data rather than a new detection, but it is a peer-reviewed challenge to a prominent result.

rss · Phys.org Space · Nov 15, 14:00

**「Background」** UHZ1 is a high-redshift galaxy that gained prominence in 2023 when X-ray and infrared observations were interpreted as evidence for a heavily dust-obscured, overmassive black hole, a result widely cited as potential support for the direct-collapse scenario in which early black holes form from gas clouds rather than stellar remnants. Such claims matter because overmassive black holes at early cosmic times would strongly constrain how quickly the first black holes could grow. The new peer-reviewed reanalysis, led by Fan Zou of the University of Michigan and published in The Astrophysical Journal, reexamined the same archival X-ray data alongside new infrared observations and found no signature of obscured black hole activity, proposing instead that UHZ1 is a low-mass, metal-poor, star-forming galaxy.

**「Constraints on early black hole formation」** The result weakens a key observational case for direct-collapse black hole formation in the early universe, and the multi-wavelength approach used to rule out obscuration offers a template for vetting other candidate overmassive black holes at high redshift.

**Tags**: `#black holes`, `#UHZ1`, `#early universe`, `#reanalysis`, `#X-ray astronomy`, `#JWST`, `#direct collapse`, `#peer-reviewed`

---

<a id="item-astronomy-news-4"></a>
### [Simulations Offer Explanation for Uranus and Neptune&\#x27;s Tilted Magnetic Fields](https://www.sciencedaily.com/releases/2026/11/261114202204.htm) ⭐️ 6.0/10

New simulations of conditions deep inside Uranus and Neptune suggest that extreme pressures and temperatures create unusual electrical properties in the planets&\#x27; interiors, offering a possible explanation for their bizarre, wildly tilted magnetic fields. The models further indicate that the magnetic poles could shift by tens of degrees within just a few decades, far faster than on Earth. Uranus and Neptune&\#x27;s strange magnetic fields have puzzled scientists since NASA&\#x27;s Voyager 2 surveyed the planets in the 1980s. This is model-based work rather than an observational detection, so it constrains interior models without yet being confirmed by measurements.

rss · ScienceDaily Astronomy · Nov 15, 13:43

**「Why the ice giants&\#x27; fields are so strange」** Unlike Earth&\#x27;s well-ordered dipolar field, Uranus and Neptune were found by Voyager 2&\#x27;s flybys in the 1980s to have highly disordered, strongly tilted magnetic fields with no clear alignment to their rotation axes. Computer simulations of the planets&\#x27; interior conditions have since explored how water, methane, and ammonia behave at extreme pressures; for example, earlier work by Prof. Militzer showed these ices can phase separate into two distinct fluids at high pressure, a mechanism proposed to produce nondipolar fields. The new models extend this line of work, suggesting the fields could be configured differently now than during the Voyager 2 era and might shift substantially within decades.

**「Constrains interior models」** The results give planetary scientists a physical mechanism to incorporate into models of icy giant interiors, which could shape priorities for future missions or observations aimed at testing the simulated electrical properties.

<details><summary>References</summary>
<ul>
<li><a href="https://www.jsg.utexas.edu/news/2026/11/wacky-magnetic-fields-of-ice-giants-explained/">Wacky Magnetic Fields of Ice Giants Explained | Jackson ...</a></li>
<li><a href="https://phys.org/news/2026-11-wacky-magnetic-fields-ice-giants.html">Wacky magnetic fields of ice giants may stem from ...</a></li>
<li><a href="https://eps.berkeley.edu/news/magnetic-disorder-uranus-and-neptune-explained">Magnetic disorder of Uranus and Neptune explained | Earth ...</a></li>

</ul>
</details>

**Tags**: `#uranus`, `#neptune`, `#magnetic fields`, `#icy giants`, `#simulations`, `#planetary science`

---

## Aerospace News

<a id="item-aerospace-news-1"></a>
### [ULA&\#x27;s Vulcan rocket fails in flight, destroying 40 Amazon Leo satellites](https://spaceflightnow.com/2026/11/15/ula-suffers-first-total-mission-failure-with-loss-of-vulcan-rocket-carrying-40-amazon-leo-satellites/) ⭐️ 9.0/10

A United Launch Alliance Vulcan rocket carrying 40 Amazon Leo internet satellites suffered an anomaly about 10 minutes into flight on Sunday, November 15, 2026, and failed to deliver the payload to orbit. ULA confirmed the failure in a statement roughly 50 minutes after the 12:40 p.m. EST liftoff from Space Launch Complex 41 at Cape Canaveral Space Force Station. It was the first outright failure of a ULA rocket since the Boeing-Lockheed Martin partnership was formed in 2006, and only the fifth flight of the Vulcan, which is replacing the Atlas 5. According to ULA&\#x27;s update, something went wrong during the planned 12-minute 15-second burn of the hydrogen-fueled Centaur upper stage, though no additional details were immediately provided and the cause remains under investigation.

rss · Spaceflight Now · Nov 15, 19:16

**「Vehicle and program context」** Vulcan is ULA&\#x27;s new heavy-lift rocket, developed by the Boeing-Lockheed Martin partnership \(formed in 2006\) to replace the Atlas 5, and Sunday&\#x27;s loss was its first outright mission failure as well as ULA&\#x27;s first in the company&\#x27;s history. The flight was only the fifth for Vulcan and its first in nine months, following work by ULA and booster supplier Northrop Grumman to resolve strap-on solid-booster nozzle problems that marred two earlier flights; those solids appeared to perform normally Sunday, and the failure occurred during the Centaur upper stage&\#x27;s planned 12-minute 15-second burn. The mission was also the first of 38 Vulcan flights Amazon has purchased for its Leo broadband constellation, which will require more than 3,300 satellites to complete and competes with Starlink and other space-based internet providers.

**「Consequences for both programs」** The failure was the first of 38 Vulcan flights Amazon has purchased for its Leo constellation, which requires more than 3,300 satellites and would have reached 436 launched with this mission; Amazon must now wait out ULA&\#x27;s investigation before retrying on a Vulcan. The mishap also potentially grounds the Vulcan while engineers review telemetry, with broader implications for ULA&\#x27;s national security launch commitments, which the U.S. Space Force already had partly held pending analysis of earlier solid-booster nozzle problems. Amazon additionally remains dependent on Blue Origin&\#x27;s New Glenn, grounded after a catastrophic on-pad explosion in May 2026 caused by an oxygen valve problem in a BE-4 engine — the same engine model powering Vulcan&\#x27;s first stage, though the engines flown Sunday had been retrofitted with a fix.

**Tags**: `#ULA`, `#Vulcan`, `#launch failure`, `#Amazon Leo`, `#Cape Canaveral`, `#mission anomaly`

---

## Chemical Products and Polymer Markets

<a id="item-chem-products-1"></a>
### [Sipchem Completes $169M Propylene and PP Expansion at Al Waha](https://news.google.com/rss/articles/CBMivgFBVV95cUxPUEVCV085T2NVQjFQMURNY3dnWVVfZS16bU1NVWxoWGtMN3VEelNQU3hIRTg1SXJ4UnV6SFA3NEl4VXJDZlF3UDZHVXQyVlk0aGtGRjZXY2QyQjIyR1hjY2Z3cTJleDhOV0VJRTBRSHZIeVpSb1cyS3NXa1B4YTJMd3JqdTBTOGVRaktWTTBtYXhmdDMxREZsRzZ0NWVjN09PRFVxOFlmbVhlYUNmaHBGS2FnQ0hMOFBtcEZPT0F3?oc=5) ⭐️ 6.0/10

Sipchem has completed a $169 million expansion of its Al Waha propylene and polypropylene \(聚丙烯\) facilities in Saudi Arabia. The announcement confirms the project has reached completion, but the available information does not specify the added capacity volumes in kt/yr or the commercial startup timing. No sales, contract, or spot price effects were reported in the source.

rss · Google News Polymers \(EN\) · Nov 15, 14:29

**「Context」** The Al Waha complex in Jubail, Saudi Arabia, is Sipchem&\#x27;s platform for propylene and polypropylene \(PP\), feeding Saudi PP output that is largely oriented toward export markets in Asia and elsewhere. Added propylene and PP capacity from a Middle East producer with advantaged feedstock costs typically competes with Asian PP supply, which is why the completion of this $169 million expansion is relevant to regional polymer supply balances. The source does not disclose the added capacity volumes or startup timing, so the scale of the incremental supply remains uncertain.

**「Impact」** The completed expansion adds incremental Saudi PP and propylene supply from a propane/butane-integrated producer, which may intensify competition for PP export cargoes into Asia and Africa once the additional volumes reach the market; buyers should watch for revised availability from Sipchem before factoring it into procurement decisions, since capacity increments and startup dates are not yet disclosed.

**Tags**: `#polypropylene`, `#propylene`, `#capacity expansion`, `#Sipchem`, `#Saudi Arabia`, `#petrochemicals`

---

## Energy News

<a id="item-energy-news-1"></a>
### [Darlington&\#x27;s First BWRX-300 SMR to Exceed C$7.7 Billion Budget and Miss 2030 Target](https://cleantechnica.com/2026/11/15/darlington-smr-cost-overrun-four-reactor-risk/) ⭐️ 6.0/10

Ontario Power Generation has acknowledged that its first GE Vernova Hitachi BWRX-300 small modular reactor at Darlington will exceed its C$7.7 billion approved budget and miss its October 2030 commercial-operation target, with no revised cost or completion figures yet. In its November 10 financial results, OPG attributed the overrun to continuing first-of-a-kind reactor engineering and its effects on construction execution and supply-chain performance, noting that physical work began while parts of the governing design were still evolving. Real construction milestones have been reached, including the 2.1-million-pound reactor foundation, turbine building progress, and assembled cooling-water tunnel equipment, but OPG expects its engineering, cost, and schedule review to be substantially complete only by mid-2027.

rss · CleanTechnica · Nov 15, 15:56

**「Context」** The Darlington BWRX-300 is Ontario&\#x27;s first grid-scale small modular reactor and part of a four-unit programme originally budgeted at C$20.9 billion, split into C$6.1 billion for the first reactor, C$1.6 billion of shared site infrastructure, and C$13.2 billion for Units 2 through 4. The programme&\#x27;s economics rest on learning effects: the first unit is meant to teach suppliers and builders how to execute the design so that the later three reactors cost less per unit, a premise that the first unit&\#x27;s own overrun now calls into question. OPG operates a large existing nuclear fleet at an established site with transmission and public financial backing, making Ontario a comparatively favourable test case for Western SMR deployment even as the BWRX-300 remains a new, not-yet-stabilized design.

**「Rate Filing and Four-Reactor Plan Affected」** The uncertainty has already reached Ontario&\#x27;s electricity planning: in its November 10 filing to the Ontario Energy Board, OPG withdrew the Darlington SMR generation forecast from its 2027–2031 rate application, removing previously planned production of about 0.5 TWh in 2030 and 1.9 TWh in 2031 without announcing a post-2031 commissioning date. The delay also pressures the economics of the four-reactor programme, which carried a C$20.9 billion total budget contingent on Units 2 through 4 becoming cheaper after the first unit&\#x27;s learning; the article argues Ontario should require an outside-view cost and schedule update, disclosure of outstanding design packages, and a system-level comparison against alternatives such as the IESO&\#x27;s May 2026 LT2 procurement of 1,115 MW of wind and solar at a weighted average C$88.84/MWh plus 640 MW of battery capacity, before committing to the next three reactors.

**Tags**: `#nuclear`, `#SMR`, `#Canada`, `#cost overrun`, `#project delay`, `#BWRX-300`, `#OPG`

---

## Oil and Gas Industry News

<a id="item-oil-gas-news-1"></a>
### [Kazakhstan Oil Output Falls Sharply After Drone Attacks Force Export Terminal Closure](https://news.google.com/rss/articles/CBMixwFBVV95cUxNUEN3X1RsX3VzbUFYalIxUExOdi1DaVBsNnVkTV9LS0F4dm9XS2xxc0p5UmxzWWVzblYzZzlRMnBHMVNqX1pQeFhmcnFxX0ROQmo2TWRWYUlFZC1xdlcyUzJfT0VOMWhoaUxOZWx3OVc2M2JYQzkxeHZuakxVc2NjZ25GaGNzQjF4aThHR1lydWdXZ2NJM0ZpWERqdTN3VUxNbW01UnVwV3BPd25IZDV4d002U0RyZ0djZFVPSGdUUEZiTDIzaWp3?oc=5) ⭐️ 7.0/10

Kazakhstan&\#x27;s oil output has reportedly plummeted after drone attacks forced the closure of a key oil exporting terminal, according to sources cited by EnergyNow.com. The report does not name the terminal, quantify the production drop, or indicate how long the closure is expected to last, so the scale and duration of the disruption remain unclear.

rss · Google News Oil &amp; Gas \(EN\) · Nov 15, 13:11

**「Context」** Kazakhstan, one of the world&\#x27;s ten largest oil producers, ships the bulk of its crude exports through the CPC pipeline terminal on Russia&\#x27;s Black Sea coast at Novorossiysk, making the terminal a single point of failure for the country&\#x27;s output. According to Reuters reporting, the closure followed suspected Ukrainian drone attacks on the export terminal in late July 2026, prompting Kazakhstan to cut production, with its daily output reportedly more than halving as loadings halted.

**「Impact」** As a significant crude exporter, any sustained halt at Kazakhstan&\#x27;s main export terminal would tighten seaborne light crude supply and could force shippers to seek alternative export routes, but the concrete volume effect cannot be assessed from the available reporting.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/business/energy/kazakhstans-oil-output-plummets-after-drone-attacks-forced-exporting-terminal-2026-07-23/">Kazakhstan slows oil output after drone strikes on export ...</a></li>
<li><a href="https://www.reuters.com/business/energy/kazakhstans-daily-oil-output-halves-after-exporting-terminal-closure-source-says-2026-07-27/">Kazakhstan&#x27;s daily oil output halves after export terminal ...</a></li>

</ul>
</details>

**Tags**: `#Kazakhstan`, `#supply disruption`, `#export terminal`, `#drone attacks`, `#market impact`

---

<a id="item-oil-gas-news-2"></a>
### [£2.1 billion Jackdaw gas field begins production in UK North Sea](https://news.google.com/rss/articles/CBMioAFBVV95cUxPSExmR2dUNFlyODZsZ3dHcHNRclhjbkNxX19WQ2VVQktrbkltM0FaWjlXUzBNdU9kcldMclVlbng5UGRQTm02bEl4SmR6aVN2ZlE1OUNHMjA4a0xlNlFYSGVmWGVNT2kwa0FNVGJQcWlTeThZdHNKZjR0OFk3UWc2SXkwMmw1dDRHMjVNb0hCWmlQNGxNVDJiZEZFYl91MnhC?oc=5) ⭐️ 7.0/10

The £2.1 billion Jackdaw gas field in the UK North Sea has started production, according to The Herald. The startup marks the transition of the project from construction into operation, adding a new domestic gas supply source for the UK. The £2.1 billion figure is the reported capital investment in the development. No production rate or reserve volume figures were provided in the source report.

rss · Google News Oil &amp; Gas \(EN\) · Nov 16, 00:05

**「Context for the Jackdaw startup」** Jackdaw is a gas field development in the UK North Sea carried at a capital investment of £2.1 billion, and its start of production follows the multi-year permitting and construction phase typical of North Sea gas projects. The project&\#x27;s startup comes as the UK continues to rely on domestic North Sea gas alongside imports for its supply, making new field startups relevant to domestic production levels. Details on the operator, plateau production volumes, and reserves cited for the field were not included in the supplied source, so those specifics remain unconfirmed here.

**「Supply effect」** The startup adds domestically produced gas to UK supply at a time when North Sea output is in structural decline, modestly reducing reliance on imports. As a mid-sized field, its contribution is incremental rather than transformative for the UK gas market.

**Tags**: `#North Sea`, `#UK`, `#Jackdaw`, `#gas field startup`, `#project milestone`

---

## Literature News

<a id="item-literature-news-1"></a>
### [M. John Harrison&\#x27;s &\#x27;The End of Everything&\#x27; Wins 2026 Booker Prize](https://www.nytimes.com/2026/11/09/books/booker-prize-winner-2026-science-fiction.html) ⭐️ 9.0/10

M. John Harrison&\#x27;s dystopian novel &quot;The End of Everything&quot; has won the 2026 Booker Prize, as reported by the New York Times on the announcement. The book prevailed over higher-profile nominees including Marlon James, Elizabeth Strout, and Douglas Stuart. The result is notable for a science-fiction-leaning dystopian work taking one of the English-speaking world&\#x27;s most prominent literary awards.

rss · New York Times Books · Nov 15, 23:26

**「Context」** The 2026 shortlist included several writers with higher public profiles than Harrison, among them Marlon James, Elizabeth Strout, and Douglas Stuart, making the victory for a dystopian novel a notable upset. The result also underscores the recurring conversation about how genre-adjacent work, often categorized as science fiction, is received by major literary institutions such as the Booker Prize.

**「Impact」** Booker Prize winners typically see substantially increased readership, sales, and translation-rights interest, bringing Harrison&\#x27;s work to a far wider audience and giving genre-adjacent fiction greater visibility in mainstream literary circles.

**Tags**: `#Booker Prize`, `#awards`, `#M. John Harrison`, `#literary fiction`, `#science fiction`

---

<a id="item-literature-news-2"></a>
### [Editors Reassess the Real Patricia Highsmith Ahead of Helen Mirren Film](https://www.theguardian.com/books/2026/nov/15/she-was-a-monster-the-real-patricia-highsmith-by-the-people-who-knew-her) ⭐️ 7.0/10

Melissa Denes reports in the Guardian on editors and publishers, including Otto Penzler, reassessing Patricia Highsmith&\#x27;s difficult reputation ahead of a new film starring Helen Mirren about the Ripley author&\#x27;s later years. Penzler recalls a 1984 reading at his Mysterious Bookshop in New York that drew only about four people, with Highsmith cutting signings short and dismissing his small talk about France. The feature tests whether she was truly as rude and eccentric as her legend suggests, drawing on firsthand recollections from those who worked with her during her two decades living in Europe.

rss · Guardian Books · Nov 15, 12:00

**「Context」** Patricia Highsmith \(1921–1995\) was an American crime writer best known for the Ripley novels and for Strangers on a Train, and she spent her later decades living in Europe, largely away from public life. The article&\#x27;s reassessment of her difficult personality is tied to renewed attention around a new film starring Helen Mirren about her later years, with recollections from figures such as publisher and bookseller Otto Penzler, who hosted one of her rare appearances at his New York bookshop in 1984.

**「Impact」** The piece offers readers a renewed framing of Highsmith&\#x27;s life and personality ahead of the Mirren film, which is likely to shape how a new audience encounters her crime fiction and biography.

**Tags**: `#Patricia Highsmith`, `#literary profile`, `#film adaptation`, `#crime fiction`, `#Guardian Books`

---

<a id="item-literature-news-3"></a>
### [New York Times Reviews Louise Kennedy&\#x27;s Novel &\#x27;Stations&\#x27;](https://www.nytimes.com/2026/11/15/books/review/stations-louise-kennedy.html) ⭐️ 6.0/10

The New York Times Book Review published Alexandra Jacobs&\#x27;s review of Louise Kennedy&\#x27;s novel &quot;Stations&quot; on November 15, 2026. The review centers on the book&\#x27;s story of a young Irishwoman in London who tests the limits of commitment. The item is a single-title review of the new novel rather than coverage of an award or industry development.

rss · New York Times Books · Nov 15, 10:00

**「Author context」** Louise Kennedy is an Irish writer whose fiction, often concerned with Irish women&\#x27;s lives, has drawn significant critical attention in Britain and Ireland. The Times review places &quot;Stations&quot; within that continuing body of work, though the supplied source offers only a one-line characterization of the novel&\#x27;s plot.

**Tags**: `#book review`, `#literary fiction`, `#Irish fiction`, `#New York Times`

---

<a id="item-literature-news-4"></a>
### [Tiffany Watt Smith on Fleeting Friendships and the Russian Poputchik](https://www.theguardian.com/lifeandstyle/2026/nov/15/the-unexpected-power-of-fleeting-friendships) ⭐️ 5.0/10

Tiffany Watt Smith published an essay in the Guardian&\#x27;s Life and Style section on 15 November 2026 arguing that brief, ephemeral friendships deserve more value than a culture that prizes long-lasting relationships permits. Drawing on the Russian word poputchik—a stranger met on a journey to whom one confesses everything precisely because the encounter will never repeat—she traces the idea through Leo Tolstoy&\#x27;s The Kreutzer Sonata and Venedikt Erofeev&\#x27;s 1970s satire Moscow to the End of the Line. Her thesis is that Aristotle&\#x27;s tradition of ranking durable bonds above transient ones leaves out the distinctive intimacy and candour that fleeting encounters make possible.

rss · Guardian Books · Nov 15, 12:00

**「Background」** The poputchik, literally a fellow traveller, was repurposed in Soviet-era usage to describe Marxist sympathisers, but Smith is interested in its original travel meaning. Both literary examples she cites unfold on train journeys: Pozdnyshev&\#x27;s confession of marriage, betrayal and murder in Tolstoy, and the drunken monologue of a retired cable fitter in Erofeev&\#x27;s novel, which a friend of hers calls &quot;therapy, Soviet-style.&quot;

**Tags**: `#essay`, `#literary criticism`, `#Russian literature`, `#friendship`, `#Guardian`

---

<a id="item-literature-news-5"></a>
### [Literary Agents Turn Themselves Into the Product via Newsletters](https://www.nytimes.com/2026/11/15/books/literary-agents-books-substack.html) ⭐️ 5.0/10

A New York Times article by Sophia June, published November 15, 2026, examines how literary agents are building public platforms around themselves through newsletters, books, and other ventures. Agent Kate McKean is cited as one of several figures who have found success by demystifying the publishing business for a general audience. The trend positions agents — traditionally behind-the-scenes dealmakers — as public experts and commentators on how the book industry works.

rss · New York Times Books · Nov 15, 10:00

**「Who Is Kate McKean?」** Kate McKean, a literary agent at the Howard Morhaim Literary Agency in Brooklyn, exemplifies the trend the article describes: she writes the Agents &amp; Books newsletter on Substack and published her first book, &quot;Write Through It: An Insider&\#x27;s Guide to Publishing and the Creative Life,&quot; with Simon Element, with debut picture books scheduled from Sourcebooks in 2026. Her public writing has also appeared in outlets including Poets &amp; Writers, Electric Literature, and Catapult.

**「Impact」** For aspiring writers, these newsletters and books offer direct, publicly available insight into an industry whose workings were previously shared mainly with clients, potentially changing how authors learn to query, negotiate, and choose representation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.simonandschuster.com/books/Write-Through-It/Kate-McKean/9781668055540">Write Through It | Book by Kate McKean | Official Publisher Page</a></li>
<li><a href="https://www.katemckean.com/">Kate McKean</a></li>
<li><a href="https://mswishlist.com/agent/kate_mckean/pubtip">Kate McKean | MsWishList</a></li>

</ul>
</details>

**Tags**: `#publishing industry`, `#literary agents`, `#newsletters`, `#Substack`, `#authorship`

---

<a id="item-literature-news-6"></a>
### [AO3 Comes Back Online After More Than Two Weeks of Downtime](https://www.nytimes.com/2026/11/15/arts/ao3-fan-fiction-site.html) ⭐️ 4.0/10

The fan fiction archive AO3 is back online after an outage lasting more than two weeks, according to a New York Times report. The site hosts stories inspired by works such as &quot;Harry Potter&quot; and &quot;Heated Rivalry,&quot; and its absence left readers without access to the archive. The Times describes readers returning to the site in large numbers after its restoration.

rss · New York Times Books · Nov 15, 22:55

**「Context」** AO3 \(Archive of Our Own\) is a large nonprofit fan fiction archive hosting stories inspired by franchises such as &quot;Harry Potter&quot; and &quot;Heated Rivalry.&quot; Its extended downtime of more than two weeks left the fan fiction community without access to the platform where much of that writing is collected, which explains the scale of reader attention when it returned.

**Tags**: `#fan fiction`, `#AO3`, `#digital platforms`, `#publishing industry`

---