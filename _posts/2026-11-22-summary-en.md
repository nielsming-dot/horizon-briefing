---
layout: default
title: "Horizon Summary: 2026-11-22 (EN)"
date: 2026-11-22
lang: en
---

> From 152 items, 22 important content pieces were selected

---

**AI News**
1. [Thinking Machines releases Inkling 2 Mini, a looped-transformer MoE model under Apache 2.0](#item-ai-news-1) ⭐️ 7.0/10

**Technology News**
1. [Lean verification of the Riemann Hypothesis](#item-tech-news-1) ⭐️ 9.0/10
2. [Monitor&\#x27;s Ethernet Adapter Was Cutting Downloads by 75%](#item-tech-news-2) ⭐️ 7.0/10
3. [FBI crime database and USDA reportedly hit by hackers](#item-tech-news-3) ⭐️ 7.0/10
4. [Anthropic goes public on Nasdaq, testing its safety-first model](#item-tech-news-4) ⭐️ 7.0/10
5. [Signal extends screenshot blocking to mobile, citing agentic AI threat](#item-tech-news-5) ⭐️ 7.0/10

**Astronomy News**
1. [BepiColombo enters orbit around Mercury eight years after launch](#item-astronomy-news-1) ⭐️ 7.0/10
2. [JWST captures aftermath of stellar merger in Andromeda galaxy](#item-astronomy-news-2) ⭐️ 7.0/10
3. [Fermi LAT&\#x27;s 14-Year All-Sky Catalog Maps 450 Sources in the &\#x27;MeV Gap&\#x27;](#item-astronomy-news-3) ⭐️ 7.0/10

**Chemical Products and Polymer Markets**
1. [Sasol to close South African VCM and PVC units by end-June 2027](#item-chem-products-1) ⭐️ 6.0/10

**Energy News**
1. [China EV Share Hits Record 68% in October as ICE Sales Crash 44%](#item-energy-news-1) ⭐️ 6.0/10

**Oil and Gas Industry News**
1. [NUPRC Opens Portal for 2026 Licensing Round Covering 40 Oil and Gas Blocks](#item-oil-gas-news-1) ⭐️ 6.0/10
2. [EU Reportedly Delays Methane Compliance for Imported Oil and Gas to 2029](#item-oil-gas-news-2) ⭐️ 6.0/10

**Literature News**
1. [National Book Award Nonfiction Finalist ElGendy May Be Ineligible](#item-literature-news-1) ⭐️ 8.0/10
2. [2026 National Book Award Finalists Headline Lit Hub Weekly Roundup](#item-literature-news-2) ⭐️ 7.0/10
3. [Jonathan Yardley, Pulitzer-Winning Washington Post Book Critic, Dies at 87](#item-literature-news-3) ⭐️ 7.0/10
4. [Hermione Lee Reassesses Anita Brookner&\#x27;s Life and Art](#item-literature-news-4) ⭐️ 7.0/10
5. [Leïla Slimani&\#x27;s First Play, Adapting Tolstoy&\#x27;s &\#x27;Resurrection,&\#x27; Opens at the Comédie-Française](#item-literature-news-5) ⭐️ 6.0/10
6. [New York Times Reviews Daniel Duane&\#x27;s &\#x27;Yosemite Falls&\#x27;](#item-literature-news-6) ⭐️ 5.0/10
7. [New York Times Reviews Ted Scheinman&\#x27;s Memoir &\#x27;Jolt&\#x27; on Electroconvulsive Therapy](#item-literature-news-7) ⭐️ 5.0/10
8. [New York Times Reviews Gary Shteyngart&\#x27;s Essay Collection &\#x27;The Sensualist&\#x27;](#item-literature-news-8) ⭐️ 5.0/10
9. [A.O. Scott Reads Yeats&\#x27;s &\#x27;The Lake Isle of Innisfree&\#x27; in Short NYT Video](#item-literature-news-9) ⭐️ 4.0/10

---

## AI News

<a id="item-ai-news-1"></a>
### [Thinking Machines releases Inkling 2 Mini, a looped-transformer MoE model under Apache 2.0](https://the-decoder.com/new-open-model-inkling-2-mini-thinks-in-loops-to-solve-problems-with-fewer-words-and-still-runs-on-a-laptop/) ⭐️ 7.0/10

Thinking Machines has released Inkling 2 Mini, an open-weight mixture-of-experts model with 26.4 billion total parameters and 5.4 billion active per token, licensed under Apache 2.0. Its distinguishing architecture is a looped transformer: 12 of its 24 layers run three times per token, which the company says allows longer internal reasoning without generating more output tokens. The model is multimodal \(text and images\), has a 1-million-token context window, and reportedly leads open models under 100 billion parameters on agentic coding benchmarks with 48.2 percent on DeepSWE v1.1 and 46.5 percent on the Vals Index v2.2. Artificial Analysis rates it 20 points on its Intelligence Index, tying it with Qwen3.8 27B at roughly six times lower cost and four times the speed; these figures come from the vendor and leaderboard evaluations, not independent reproduction.

rss · The Decoder · Nov 21, 10:33

**「Background」** Conventional transformers pass each token through their layers once, so longer internal reasoning typically means generating more output tokens and paying more compute per answer. Looped transformers change this by reusing the same weight layers multiple times per token — in Inkling 2 Mini, 12 of 24 layers run three times — trading extra compute per token for fewer generated tokens. Thinking Machines Lab, which released the model on Nov 20, 2026 under Apache 2.0, positions it on the Pareto frontier of intelligence versus active parameters, with Artificial Analysis scoring it at 20 on its Intelligence Index for a 26.4B total / 5.4B active mixture-of-experts model.

**「Practical relevance」** The weights and a research version with variable loop counts are downloadable from Hugging Face, and the model runs locally on Macs with at least 32 GB of memory and on Nvidia&\#x27;s DGX Spark, making it a concrete option for on-device agentic coding work where API latency or data handling rules rule out cloud models. The reported benchmark advantages should be treated as vendor and leaderboard claims until independently validated.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/inkling-2-mini">Thinking Machines has released Inkling 2 Mini, an open ...</a></li>
<li><a href="https://casrai.org/news/thinking-machines-inkling-2-mini-open-looped-model-laptop-2026">Inkling 2 Mini: open looped model for laptops — CASRAI</a></li>

</ul>
</details>

**Tags**: `#open-models`, `#architecture`, `#looped-transformer`, `#benchmarks`, `#efficiency`

---

## Technology News

<a id="item-tech-news-1"></a>
### [Lean verification of the Riemann Hypothesis](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 9.0/10

A Riemann Hypothesis proof reportedly verified in Lean, with AI playing a major formalization role, sparks major community discussion about proof-assistant trust and AI-driven mathematics.

hackernews · g-b-r · Nov 21, 14:36 · [Discussion](https://news.ycombinator.com/item?id=50589618)

**Tags**: `#formal-verification`, `#lean`, `#riemann-hypothesis`, `#ai-mathematics`, `#proof-assistants`

---

<a id="item-tech-news-2"></a>
### [Monitor&\#x27;s Ethernet Adapter Was Cutting Downloads by 75%](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

A developer diagnosed why downloads through his monitor&\#x27;s built-in USB Ethernet adapter were running at roughly 25% of expected speed on his 2.5-gigabit symmetrical line. The cause was the extra latency added by packets traveling through the monitor&\#x27;s USB hub, which prevented his laptop from acknowledging packets quickly enough; the adapter&\#x27;s buffer filled and it began dropping packets, triggering retransmissions. Swapping to a different adapter that required less frequent acknowledgement resolved the slowdown.

hackernews · soheilpro · Nov 21, 10:36 · [Discussion](https://news.ycombinator.com/item?id=50587875)

**「Why a USB Ethernet adapter can slow downloads」** Many monitors and docks include a built-in USB-to-Ethernet adapter, so a laptop&\#x27;s network traffic actually travels through the USB hub inside the monitor rather than through a direct network interface. TCP performance depends on the receiver acknowledging packets quickly; if the adapter&\#x27;s buffering adds enough latency, acknowledgments lag, the sender&\#x27;s buffers fill up, and packets get dropped, which shows up to the user as large and unexplained speed losses.

**「Practical takeaway」** Users routing network connections through monitor USB hubs or docks may see similar mysterious throughput loss, since added acknowledgement latency can silently overflow adapter buffers and drop packets. If unexplained slowdowns occur through such a chain, testing a direct or lower-latency adapter is a concrete first diagnostic step.

**「Community discussion」** Commenters clarified that the monitor itself was incidental — as manarth put it, it was effectively &quot;my USB network switch was cutting my download speed&quot; — and fancyfredbot noted many readers misread the article&\#x27;s actual latency-and-buffer explanation. Others reported similar experiences: gh123man described the same problem for over a year with a MacBook and Thunderbolt dock, only mitigating it by enabling flow control, while senko drew an analogy to Ghostty&\#x27;s io\_uring usage being misread as I/O pressure by Baldur&\#x27;s Gate 3&\#x27;s shader-compile throttling.

**Tags**: `#networking`, `#usb`, `#ethernet`, `#troubleshooting`, `#hardware`

---

<a id="item-tech-news-3"></a>
### [FBI crime database and USDA reportedly hit by hackers](https://www.theverge.com/tech/1039543/fbi-usda-hacked) ⭐️ 7.0/10

Reports on Friday, November 20–21, 2026, indicate that both the FBI and the US Department of Agriculture were hacked. The FBI breach targeted the National Crime Information Center, the database federal, state, and local law enforcement use to share warrants, background checks, and missing persons information; President Trump confirmed the hack in a Fox News interview, saying &quot;it&\#x27;s not good.&quot; According to Reuters, the known extent of the USDA intrusion is a payments database, though former officials warned the breach may not be limited to it. The scope of both breaches, including what data was accessed, is not yet clear.

rss · The Verge · Nov 21, 17:42

**「Background」** The National Crime Information Center \(NCIC\) is an FBI-run computerized database that federal, state, and local law enforcement agencies use to share records on warrants, fugitives, missing persons, criminal histories, and stolen property. This is also the second reported cyberattack on the FBI in recent months: in September, the agency reportedly told agents and support staff that their personal information had been stolen in a separate cyberattack.

**「Why it matters」** Because law enforcement officers rely on NCIC records to make operational decisions, a former FBI official told CNN the concern is not only whether sensitive information was taken, but whether attackers could compromise the accuracy of the information officers rely on — a risk for anyone subject to warrants or checks in the database. This is also the second reported FBI cyberattack in recent months: in September the bureau told agents and support staff their personal information had been stolen.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/fbi-database-ncic-hack-d066cff87a64a564db0a00172c124972">FBI probing hack of its national criminal justice database ...</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#government-breach`, `#FBI`, `#national-security`, `#data-breach`

---

<a id="item-tech-news-4"></a>
### [Anthropic goes public on Nasdaq, testing its safety-first model](https://www.theverge.com/podcast/1038701/anthropic-ipo-ai-safety-openai-nvidia-structure) ⭐️ 7.0/10

Anthropic, the AI lab behind Claude, went public on the Nasdaq last Thursday, pricing its IPO at $83 per share before the stock rose to $111 on debut day, making it the first pure AI lab to go public and one of the most valuable companies in the world. On a Verge Decoder podcast episode published November 21, host Nilay Patel and senior AI reporter Hayden Field examined what the IPO means for the company&\#x27;s safety-first identity, now that it must answer to public shareholders while covering compute commitments they describe as roughly $900 billion over the coming years. The discussion covered Anthropic&\#x27;s unusual corporate governance structure, which gives its founders more control than it may appear, and the tension between its safety branding and the profit-oriented demands of being a public company. Field argued the IPO itself provides little new information about whether the AI bubble will pop, calling the moment peak AI hype.

rss · The Verge · Nov 21, 15:00

**「Background」** Anthropic was founded as a public benefit corporation in 2021 and created a long-term benefit trust in 2023 to ensure it balances shareholder goals with its broader mission. Its IPO filing disclosed a governance structure the company itself admits &quot;differs significantly&quot; from most public companies, giving ordinary shareholders virtually no control over decisions — a design critics, including NYC Comptroller Mark Levine, say strips power from shareholders.

**「Why it matters」** The report suggests OpenAI is treating Anthropic&\#x27;s debut as a trial balloon: Sam Altman reportedly once wanted to beat Anthropic to market, but after a year of setbacks and negative publicity, OpenAI appears content to watch how markets value a rival AI lab&\#x27;s revenue before telling its own IPO story. Companies weighing IPO timing or investment in frontier AI labs now have Anthropic&\#x27;s market reception as a reference point, and Anthropic&\#x27;s safety branding — which also serves as its pitch to enterprise customers — will face heightened scrutiny from shareholders as the company manages its compute spending.

<details><summary>References</summary>
<ul>
<li><a href="https://qz.com/nyc-comptroller-anthropic-ipo-shareholder-power-governance-110226">Comptroller Mark Levine says Anthropic IPO strips shareholder power</a></li>
<li><a href="https://www.nytimes.com/2026/11/18/business/anthropic-ipo-corporate-governance.html">Anthropic ’s Public Debut Sets Up ‘Experiment’ in Corporate Power</a></li>
<li><a href="https://www.ft.com/content/a6c43402-719e-4295-ae5f-541edb0aeb29?syn-25a6b1a6=1">‘Bold but sane’: what we learnt from Anthropic ’s 240,000-word IPO filing</a></li>

</ul>
</details>

**Tags**: `#anthropic`, `#ai-safety`, `#ipo`, `#ai-industry`, `#openai`

---

<a id="item-tech-news-5"></a>
### [Signal extends screenshot blocking to mobile, citing agentic AI threat](https://techcrunch.com/2026/11/21/signal-restricts-mobile-screenshots-as-it-confronts-existential-threat-of-ai-surveillance/) ⭐️ 7.0/10

Signal announced on Friday that it is extending screenshot-blocking restrictions to its Android and iOS apps, building on the default screenshot block already in place on its Windows app. President Meredith Whittaker framed the move as a response to an &quot;existential threat&quot; from operating systems — Windows, Android, and macOS/iOS — whose integrated agentic AI can scan on-screen data outside Signal&\#x27;s control. Users can disable the restriction, though Whittaker said doing so would &quot;break our privacy guarantees.&quot; She acknowledged the measure is &quot;incomplete,&quot; since it does not address other ways AI agents could potentially access application data.

rss · TechCrunch · Nov 21, 21:37

**「Background」** Signal, an end-to-end encrypted messaging app, already blocked screenshots of its Windows desktop app by default before this change. The new restriction extends that same approach to Android and iOS, reflecting a shift in the threat model: rather than another user capturing the screen, the concern is now OS-level agentic AI that can scan and store anything displayed on screen, data that leaves Signal&\#x27;s control once captured.

**「What it means」** Mobile users who rely on Signal for sensitive conversations will no longer be able to capture screenshots by default and will need to explicitly opt out, which the company says weakens privacy protections for everyone in the conversation. The protection is also limited: OS-level AI agents could capture data through means other than screenshots, so Signal&\#x27;s end-to-end guarantees no longer fully cover what happens on a user&\#x27;s screen.

**Tags**: `#privacy`, `#signal`, `#agentic-ai`, `#security`, `#mobile`

---

## Astronomy News

<a id="item-astronomy-news-1"></a>
### [BepiColombo enters orbit around Mercury eight years after launch](https://www.space.com/space-exploration/missions/esa-jaxa-bepicolomobo-mission-mercury-orbit-arrival) ⭐️ 7.0/10

The joint ESA-JAXA BepiColombo mission is scheduled to enter orbit around Mercury today \(Nov. 21, 2026\), following a 37-minute orbit-insertion burn beginning at 1:24 p.m. EST \(1824 GMT\). The mission launched aboard an Ariane 5 rocket in October 2018 and reached the innermost planet via a trajectory of one Earth flyby, two Venus flybys, and six Mercury flybys; the flight time was extended by a year after a solar-panel issue reduced power for the Mercury Transfer Module&\#x27;s electric thrusters. BepiColombo comprises ESA&\#x27;s Mercury Planetary Orbiter and JAXA&\#x27;s Mercury Magnetospheric Orbiter \(Mio\), which remain connected and are expected to separate around Dec. 9. Mio will settle into its highly elliptical polar orbit shortly afterward, while the MPO reaches its less elliptical polar orbit on March 10, 2027, with science operations beginning April 6, 2027.

rss · Space.com · Nov 21, 11:00

**「Background」** BepiColombo, a joint ESA-JAXA mission, launched aboard an Ariane 5 from French Guiana in October 2018 and consists of two orbiters — ESA&\#x27;s Mercury Planetary Orbiter \(MPO\) and JAXA&\#x27;s Mercury Magnetospheric Orbiter \(Mio\) — plus the Mercury Transfer Module providing power and propulsion. Mercury is hard to reach because the sun&\#x27;s gravity accelerates incoming spacecraft to high speeds that must be shed for capture, so the mission used a looping trajectory with one Earth flyby, two Venus flybys, and six Mercury flybys over roughly seven to eight years, a schedule extended by a year after a solar-panel issue reduced power for the electric thrusters. Once both orbiters settle into their final polar orbits in 2027, the mission will study Mercury&\#x27;s magnetosphere and its interaction with the solar wind, the planet&\#x27;s large iron core and internal structure, and the origin of its magnetic field.

**「What comes next」** Once science operations start in April 2027, the two orbiters will gather complementary data from different vantage points on Mercury&\#x27;s magnetosphere and its interaction with the solar wind, the planet&\#x27;s internal structure and large iron core, and the origin of its magnetic field. The dual-orbiter design allows simultaneous measurements from two orbits, a configuration not available during previous single-spacecraft Mercury missions.

**Tags**: `#space missions`, `#Mercury`, `#BepiColombo`, `#ESA`, `#JAXA`, `#planetary science`

---

<a id="item-astronomy-news-2"></a>
### [JWST captures aftermath of stellar merger in Andromeda galaxy](https://www.sciencedaily.com/releases/2026/11/261120075556.htm) ⭐️ 7.0/10

Astronomers observed an eruption in the Andromeda galaxy \(M31\) in which a small star spiraled into a luminous giant roughly 18,000 times brighter than the Sun. NASA&\#x27;s James Webb Space Telescope imaged the aftermath just 47 days after the outburst, providing infrared detail on how two stars merge into one. The report indicates the observations reveal the post-eruption environment of the merger, though the available account does not specify quantitative measurements or whether the results have been peer-reviewed. The event is presented as a witnessed stellar merger, offering a rare view of a process usually inferred only from its long-term remnants.

rss · ScienceDaily Astronomy · Nov 21, 14:53

**「Background」** The event, designated AT 2025abao and nicknamed Bao, occurred in the Andromeda galaxy \(M31\), where a star slightly lighter than the Sun spiraled into a luminous giant over roughly seven orbits inside a shared envelope, or common envelope, before they merged. Common-envelope inspiral is a predicted but rarely directly observed phase of binary evolution, in which friction inside the giant&\#x27;s envelope dissipates orbital energy and can drive ejection of the outer stellar layers. JWST observations beginning in December 2025 provided the evidence that allowed researchers to reconstruct the merger before, during, and after the event, with the results published in Nature.

**「Why it matters for merger physics」** Because the eruption occurred in M31, a well-studied nearby galaxy, and was followed up rapidly in the infrared, the data can directly constrain models of common-envelope evolution and stellar mergers, which previously relied on older, cooler remnants rather than observations taken weeks after the event.

<details><summary>References</summary>
<ul>
<li><a href="https://science.nasa.gov/missions/webb/nasa-data-clinches-first-of-its-kind-stellar-merger/">NASA Data Clinches First-of-Its-Kind Stellar Merger</a></li>
<li><a href="https://www.nature.com/articles/s41586-026-11221-z">An inspiral of a star inside a common envelope with its giant ...</a></li>
<li><a href="https://www.techtimes.com/articles/331105/20261119/andromeda-star-merger-webb-dust-data-suggest-small-star-sank-giant-after-seven-orbits.htm">Andromeda Star Merger: Webb Dust Data Suggest Small Star Sank ...</a></li>

</ul>
</details>

**Tags**: `#stellar merger`, `#James Webb Space Telescope`, `#Andromeda galaxy`, `#common envelope`, `#transient`

---

<a id="item-astronomy-news-3"></a>
### [Fermi LAT&\#x27;s 14-Year All-Sky Catalog Maps 450 Sources in the &\#x27;MeV Gap&\#x27;](https://phys.org/news/2026-11-fermi-year-sky-bridges-astronomy.html) ⭐️ 7.0/10

The Fermi Large Area Telescope \(LAT\) Collaboration has published a 14-year all-sky gamma-ray catalog in The Astrophysical Journal Supplement Series identifying 450 cosmic sources in the poorly covered 20–200 MeV energy range. This peer-reviewed dataset provides the clearest view yet of low-energy gamma rays, a band long known as astronomy&\#x27;s &\#x27;MeV gap&\#x27; because instruments have historically struggled to measure emission there. The catalog does not report a single new detection but rather a systematic survey across the entire sky, building on the LAT&\#x27;s accumulated observations since its launch. It represents the most significant dataset to date for this hard-to-observe energy regime.

rss · Phys.org Space · Nov 21, 13:00

**「What the MeV gap is and why it matters」** The &\#x27;MeV gap&\#x27; refers to a long-standing sensitivity shortfall in gamma-ray astronomy between roughly 20 and 200 megaelectronvolts, a band too energetic for traditional X-ray instruments and too low in energy for most gamma-ray telescopes to detect efficiently. Because hard X-ray telescopes lack sensitivity at these energies and the Fermi Large Area Telescope&\#x27;s pair-conversion detection becomes less effective below about 200 MeV, few instruments could reliably pinpoint sources there, leaving this part of the spectrum poorly charted compared with adjacent bands. Catalogs like the newly published 14-year all-sky analysis, which appears in The Astrophysical Journal Supplement Series, matter because they turn years of accumulated exposures into a reference list of 450 sources that other observers and theorists can use for follow-up.

**「Impact」** The catalog gives observers and modelers a reference source list in the 20–200 MeV band where sensitivity was previously limited, enabling cross-identification with higher-energy gamma-ray catalogs and better characterization of source classes such as pulsars, blazars, and solar-system emission at these energies.

**Tags**: `#gamma-ray astronomy`, `#Fermi LAT`, `#MeV gap`, `#source catalog`, `#survey`

---

## Chemical Products and Polymer Markets

<a id="item-chem-products-1"></a>
### [Sasol to close South African VCM and PVC units by end-June 2027](https://news.google.com/rss/articles/CBMiWEFVX3lxTFA1ZjNNX01iSUhDMWdRckpLZkEzbGppUjN1LUFKTWpPWVJ2a3UwMmpmTUtoS0p1UU9ZUk5ON3FlMEhpTkRKNW03bEhtT2laYjA3SEZUREhRMng?oc=5) ⭐️ 6.0/10

South Africa&\#x27;s Sasol has decided to permanently shut down its vinyl chloride monomer \(VCM\) and PVC production facilities by the end of June 2027. The announcement, reported by 维度网 on 21 November 2026, confirms a fixed closure timeline for the chlor-vinyl assets. The report does not disclose the capacity volumes involved, the share of regional supply the plants represent, or the reason for the exit, so the quantified supply effect remains uncertain.

rss · Google News 化工品 \(ZH\) · Nov 21, 06:09

**「Context for Sasol&\#x27;s chlor-vinyl capacity exit」** Sasol is a global chemicals and energy company, and the planned shutdown of its vinyl chloride monomer \(VCM\) and PVC units by the end of June 2027 comes as the company has emphasized strengthening its financial resilience following its FY2026 results \(year ended 30 June 2026\). Chlor-vinyl production is energy- and feedstock-intensive, so capacity exits in this chain are typically driven by cost competitiveness and portfolio prioritization. The source item does not disclose the capacity volumes involved or Sasol&\#x27;s regional market share, so the size of the supply reduction remains unconfirmed.

**「Impact」** The closure removes Sasol&\#x27;s PVC and VCM output from the South African market by mid-2027, which will force local PVC converters and downstream users to shift toward imports or alternative suppliers, and regional PVC import demand is likely to rise as the exit date approaches.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sasol.com/">Home | Sasol</a></li>

</ul>
</details>

**Tags**: `#PVC`, `#VCM`, `#capacity closure`, `#Sasol`, `#South Africa`, `#supply`

---

## Energy News

<a id="item-energy-news-1"></a>
### [China EV Share Hits Record 68% in October as ICE Sales Crash 44%](https://cleantechnica.com/2026/11/21/ev-share-jumps-to-68-and-small-bevs-rise-to-power-china-ev-sales-report-for-october/) ⭐️ 6.0/10

China&\#x27;s plugin vehicle share reached a record 68% of new car sales in October 2026, split between 45% BEVs and 23% PHEVs, on total sales of around 1.6 million units. The record came despite the overall market falling 27% year over year, because pure ICE sales crashed 44% YoY while plugin sales fell a milder 14%. The 2026 share so far stands at 59%, already 5 points above the full-year 2025 result, with BEVs alone at 40% versus 33% in 2025. The overall top 10 best sellers were all EVs, led by the Geely Xingyuan at 50,190 registrations, up 14% YoY, with small B-segment EVs such as the Leapmotor A10 \(27,247 units, priced at 66,000 yuan\) and BYD Yuan Up \(28,514 units, up 44% YoY\) dominating the hottest segments.

rss · CleanTechnica · Nov 21, 19:38

**「Context」** China is the world&\#x27;s largest automotive market, and plugin vehicles have moved from a niche to the mainstream there over the past several years, with the report noting that the 2026 year-to-date EV share of 59% is already 5 percentage points above the full-year 2025 result, and BEVs alone at 40% versus 33% in 2025. The October milestone — a record 68% plugin share composed of 45% BEV and 23% PHEV — was driven less by plugin growth \(plugins fell 14% year over year\) than by a collapse in internal combustion sales, which dropped 44% YoY as the overall market shrank 27% to roughly 1.6 million units. A key structural feature of the current market is the surge of small, affordable B-segment BEVs, such as the Geely Xingyuan and BYD Yuan Up, which start around $10,000–$11,000 and now dominate the best-seller lists, even as manufacturers largely launch larger SUVs.

**「Price pressure on incumbents」** The rise of affordable small BEVs is compressing incumbent pricing: BYD&\#x27;s new Song Ultra midsize SUV starts at 152,000 yuan \($22,000\) with 1,500 kW DC charging, well below the Tesla Model Y&\#x27;s 259,000 yuan \($38,250\) starting price in China, and Model Y sales fell 60% YoY to 7,807 units. Volkswagen&\#x27;s China-developed ID.Aura T6 reached 20th place in its first full month, the first time in years a VW model outsold Tesla in China, suggesting foreign automakers must now compete with locally developed, price-competitive EVs to hold share. If the October trend continues, the author projects the 2026 full-year EV share will exceed 60%, though such extrapolations are speculative.

**Tags**: `#China`, `#EV sales`, `#market share`, `#BEV`, `#PHEV`, `#ICE decline`

---

## Oil and Gas Industry News

<a id="item-oil-gas-news-1"></a>
### [NUPRC Opens Portal for 2026 Licensing Round Covering 40 Oil and Gas Blocks](https://news.google.com/rss/articles/CBMikwFBVV95cUxNb2xzLUF4ekRZcXBkOXU4amx6YzN0WVlnbHNYdXF0TGFyTlU1ZHZ6MnJjSHZhazNNRGh6U083YXVsT2R2M19IdF8yVDI4NUh6N1ZSWWhHalZoRFdaWVotQXZQeXVYMGQycHRUbTAwVmFQNmVCaEF0aHRzT3ZVSkgxaUJRUTM2eTZGbHZlWVd6UXFfNTg?oc=5) ⭐️ 6.0/10

Nigeria&\#x27;s upstream petroleum regulator, the Nigerian Upstream Petroleum Regulatory Commission \(NUPRC\), has opened the application portal for a 2026 licensing round covering 40 oil and gas blocks. The announcement marks the formal launch of the bid process, though the available report does not specify block locations, contract terms, deadlines, or fee structures. Details on the blocks and application requirements are expected to be published by the regulator as the round proceeds.

rss · Google News Oil &amp; Gas \(EN\) · Nov 21, 18:17

**「Background」** The NUPRC first announced the 2026 Licensing Round in early October 2026, with Commission Chief Executive Mrs. Oritsemeyiwa Eyesan unveiling plans at an October 7 event to offer 40 oil and gas blocks across three terrains. The opening of the application portal follows that announcement and moves the round from launch to the formal bid submission stage.

**「Impact」** The opening of the portal gives international and domestic upstream operators a formal entry point to acquire Nigerian acreage in 2026, and investors will be watching the block slate and fiscal terms for signals about how competitive Nigeria&\#x27;s licensing framework is against other African basins.

<details><summary>References</summary>
<ul>
<li>NUPRC Announces 2026 Licensing Round, Unveils Plans to Boost ...</li>
<li>40 blocks. Three terrains. Nigeria&#x27;s 2026 Licensing Round is officially ...</li>
<li>40 highly prospective oil and gas blocks on offer across diverse ...</li>

</ul>
</details>

**Tags**: `#Nigeria`, `#NUPRC`, `#licensing round`, `#upstream`, `#regulation`

---

<a id="item-oil-gas-news-2"></a>
### [EU Reportedly Delays Methane Compliance for Imported Oil and Gas to 2029](https://news.google.com/rss/articles/CBMijgJBVV95cUxNSlJwRjk1c3dEREFzQWJWYWlyOEdzQ3hTN214WldOT19rLUsyR0toMDlUZ2tQeUgzcTBOYVdFTzRlMXZuX0hjMU9DQkczUUxkb2gyQkxObXBjNjZSY0Ffb01JLWtUbTNHT2tMeGczeWFGbmgyZVQ3WFRURW42ODdzY1c1LVNmYXYybWZlbExxc0ctQzZldm9fMkJDMW1TbDEtV0FQSlphUkxIWDczaTFfYlZmb0phd0hiUFpHY0dNeUJPSnRlZHduQW5RVVpndEFVZjRQeXoyUDdOaWpSdFJHOHhsWDBlak9ET0xORFAxS0xIZUw0TlNxZUVWcEJnUW1KRFE3cVRBSmF0cHlPeXc?oc=5) ⭐️ 6.0/10

The EU has reportedly postponed the methane emissions compliance deadline for imported oil and gas to 2029, according to CPG Click Oil and Gas. The delay gives exporting countries, including Brazil, additional time to meet the EU methane rules before enforcement applies to imports. The source notes Brazil ranked among Europe&\#x27;s top suppliers in September, though the report does not provide specific volumes, quota figures, or details on how the postponement was decided, so the exact scope and final confirmation of the delay remain unclear.

rss · Google News Oil &amp; Gas \(EN\) · Nov 21, 15:29

**「Regulatory context」** The delay stems from the EU Methane Regulation, which originally required importers of oil, gas and coal to meet monitoring, reporting and verification obligations. In October 2026 the European Parliament voted to postpone those rules for importers by three years—two more than the Commission had proposed—and on 19 November 2026 the Council and Parliament reached a provisional agreement securing a two-year postponement for specific methane rules on crude oil, natural gas and coal imports, with operators now required to submit verified reports by 5 February 2029 for operated assets and 5 August 2030 for non-operated assets.

**「Impact」** For exporters whose crude and LNG would have struggled to meet methane intensity requirements, an extension to 2029 means continued access to the EU market without near-term investment in methane monitoring, measurement, and abatement, while suppliers that have already invested in compliance gain less near-term competitive advantage from those efforts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.europarl.europa.eu/news/en/press-room/20261021IPR48321/methane-rules-parliament-backs-longer-delay-for-energy-importers-and-producers">Methane rules: Parliament backs longer delay for energy ...</a></li>
<li><a href="https://www.consilium.europa.eu/en/press/press-releases/2026/11/19/methane-regulation-eu-agrees-targeted-amendment-to-safeguard-security-of-supply/">Methane regulation: EU agrees targeted amendment to safeguard ...</a></li>
<li><a href="https://www.europarl.europa.eu/news/en/press-room/20261118IPR48949/methane-deal-to-delay-reporting-and-monitoring-for-energy-importers">Methane: deal to delay reporting and monitoring for energy ...</a></li>

</ul>
</details>

**Tags**: `#EU regulation`, `#methane`, `#imports`, `#Brazil`, `#trade`

---

## Literature News

<a id="item-literature-news-1"></a>
### [National Book Award Nonfiction Finalist ElGendy May Be Ineligible](https://www.nytimes.com/2026/11/17/books/national-book-award-nonfiction-elgendy-eligibility.html) ⭐️ 8.0/10

The New York Times reports that Abdelrahman ElGendy, whose memoir is a finalist for the National Book Award in nonfiction, may be ineligible for the prize. ElGendy was blocked from traveling to the United States to attend this year&\#x27;s awards ceremony. According to the report, despite his book&\#x27;s finalist status, it appears not to meet the qualification requirements for the award.

rss · New York Times Books · Nov 21, 20:53

**「Prize rules in context」** The National Book Awards&\#x27; current eligibility rules were established in February 2024, after the Pulitzer Prize board adjusted its own criteria in September 2023 to include permanent U.S. residents and authors whose longtime primary home was in the United States. ElGendy&\#x27;s case tests how those rules apply to a finalist unable to enter the country for the ceremony.

**「Impact」** The controversy could affect how the finalist&\#x27;s work is valued and raises questions about prize administration at one of American publishing&\#x27;s major awards, particularly regarding eligibility standards and finalists barred from attending.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/17/books/national-book-award-nonfiction-elgendy-eligibility.html">National Book Award Finalist May Be Ineligible for the Prize</a></li>

</ul>
</details>

**Tags**: `#National Book Awards`, `#prizes`, `#eligibility`, `#nonfiction`, `#publishing industry`

---

<a id="item-literature-news-2"></a>
### [2026 National Book Award Finalists Headline Lit Hub Weekly Roundup](https://lithub.com/lit-hub-weekly-november-16-20-2026/) ⭐️ 7.0/10

Lit Hub&\#x27;s weekly roundup for November 16–20, 2026 leads with the reveal of the 2026 National Book Award finalists. Among the finalists is Abdelrahman ElGendy, whose memoir &quot;Huna&quot; was recognized, and who wrote in The New Yorker about being denied a US visitor visa to attend the awards ceremony. The roundup also aggregates essays on Pompeii&\#x27;s erotic art, AI and consciousness, manga&\#x27;s shift toward an IP economy, and a birthday note marking Olav Duun&\#x27;s birth in 1876.

rss · Literary Hub · Nov 21, 11:30

**「Context」** The National Book Awards are among the most prominent American literary prizes, and the release of each year&\#x27;s finalists typically draws wide attention from publishers and readers. The 2026 list carries an unusually public complication: finalist Abdelrahman ElGendy, recognized for his memoir &quot;Huna,&quot; published an essay in The New Yorker describing being denied a visitor visa to attend the awards ceremony in person. The roundup&\#x27;s other pieces—on Pompeii&\#x27;s erotic art, manga&\#x27;s shift toward an IP economy, and the Internet Archive—are cultural essays rather than prize news.

**「Impact」** Finalists named for the National Book Award gain immediate visibility for their books ahead of the winners&\#x27; announcement, though ElGendy&\#x27;s visa denial means one finalist will be absent from the ceremony in person.

**Tags**: `#National Book Award`, `#prize finalists`, `#literary news roundup`, `#book history`, `#essays`

---

<a id="item-literature-news-3"></a>
### [Jonathan Yardley, Pulitzer-Winning Washington Post Book Critic, Dies at 87](https://www.nytimes.com/2026/11/20/books/jonathan-yardley-dead.html) ⭐️ 7.0/10

Jonathan Yardley, the Pulitzer Prize-winning book critic for The Washington Post, has died at 87, according to a New York Times obituary. Over a decades-long career he reviewed some 3,000 books and was known for a blunt critical style; he believed praise could be boring. His death is reported by obituary writer Sam Roberts in a piece published November 20, 2026.

rss · New York Times Books · Nov 21, 14:39

**「Background」** Yardley spent decades as the book critic of The Washington Post, where his blunt, often contrarian reviews made him one of the most influential voices in American literary criticism. He won the Pulitzer Prize for Criticism in 1981, an honor that cemented his standing among the small group of critics whose daily judgments could shape a book&\#x27;s fortunes.

**Tags**: `#obituary`, `#literary criticism`, `#Jonathan Yardley`, `#Washington Post`, `#Pulitzer Prize`

---

<a id="item-literature-news-4"></a>
### [Hermione Lee Reassesses Anita Brookner&\#x27;s Life and Art](https://www.nytimes.com/2026/11/16/books/review/anita-brookner-hermione-lee.html) ⭐️ 7.0/10

In a New York Times Book Review piece dated November 2026, Dwight Garner reviews Hermione Lee&\#x27;s new book &\#x27;Anita Brookner: Art and Life.&\#x27; Lee, a leading literary biographer, challenges widely held public perceptions of Brookner, a novelist whose private life has remained largely unknown. The review positions the book as a corrective to the established image of Brookner, connecting her art with the realities of her life.

rss · New York Times Books · Nov 21, 15:42

**「Biographer and Subject」** Hermione Lee is a distinguished literary biographer, and her subject, Anita Brookner, was a novelist and art historian long defined in the public imagination by the lonely women of her fiction. According to the publisher, Lee&\#x27;s biography argues that Brookner was the inventor of those solitary characters rather than their alter ego, portraying her instead as formidable, witty, elegant, precise, and controlled. The book&\#x27;s task was complicated by Brookner&\#x27;s own resistance: she did not want a biography written and destroyed her letters and private papers.

**「Impact」** Readers and scholars approaching Brookner&\#x27;s novels now have a major biographical study from a prominent biographer that may reshape how her fiction is read and discussed, likely influencing future criticism and courses on her work.

<details><summary>References</summary>
<ul>
<li><a href="https://www.penguinrandomhouse.com/books/695848/anita-brookner-by-hermione-lee/">Anita Brookner by Hermione ... | PenguinRandomHouse.com: Books</a></li>
<li><a href="https://www.nytimes.com/2026/11/16/books/review/anita-brookner-hermione-lee.html">Book Review: ‘ Anita Brookner : Art and Life ,’ by Hermione Lee - The...</a></li>

</ul>
</details>

**Tags**: `#book review`, `#biography`, `#Anita Brookner`, `#Hermione Lee`, `#literary criticism`

---

<a id="item-literature-news-5"></a>
### [Leïla Slimani&\#x27;s First Play, Adapting Tolstoy&\#x27;s &\#x27;Resurrection,&\#x27; Opens at the Comédie-Française](https://www.nytimes.com/2026/11/21/theater/leila-slimani-resurrection-comedie-francaise.html) ⭐️ 6.0/10

Leïla Slimani, the best-selling author of &quot;The Perfect Nanny,&quot; has written her first play, an adaptation of Tolstoy&\#x27;s novel &quot;Resurrection,&quot; which is opening at the Comédie-Française in Paris. The staging marks the novelist&\#x27;s first foray into theater. According to the New York Times profile by Laura Cappelle, Slimani had long struggled with writing dialogue before taking on the project.

rss · New York Times Books · Nov 21, 13:48

**「Context」** Leïla Slimani is best known as a novelist, most notably for &quot;The Perfect Nanny,&quot; and according to the report had long struggled with writing dialogue, making this her first foray into playwriting. The Comédie-Française, where the adaptation of Tolstoy&\#x27;s &quot;Resurrection&quot; opens, is one of France&\#x27;s most prestigious theaters, giving a debut playwright an unusually prominent stage.

**Tags**: `#theater`, `#Leïla Slimani`, `#adaptation`, `#Tolstoy`, `#Comédie-Française`, `#French literature`

---

<a id="item-literature-news-6"></a>
### [New York Times Reviews Daniel Duane&\#x27;s &\#x27;Yosemite Falls&\#x27;](https://www.nytimes.com/2026/11/21/books/review/yosemite-falls-daniel-duane.html) ⭐️ 5.0/10

The New York Times Book Review has published a review of Daniel Duane&\#x27;s &\#x27;Yosemite Falls,&\#x27; written by Blair Braverman and appearing on November 21, 2026. The book draws on Duane&\#x27;s upbringing in a family steeped in the lore of the Yosemite Valley and in the writings of John Muir. According to the review, with age the author has come to look deeper at that legacy, reexamining the material he grew up with.

rss · New York Times Books · Nov 21, 10:01

**「Context」** Daniel Duane&\#x27;s connection to Yosemite runs through family lore and the writings of John Muir, the naturalist whose celebrations of the valley shaped generations of American nature writing. The review, by Blair Braverman in the New York Times Book Review, frames the book as a mature reconsideration of that inheritance: with age, Duane has come to look deeper at the legacy he grew up inside.

**「Impact」** Coverage in the New York Times Book Review can raise the book&\#x27;s visibility among readers of nature and travel writing and may influence library and bookstore ordering decisions for the title.

**Tags**: `#book review`, `#nature writing`, `#Yosemite`, `#John Muir`, `#Daniel Duane`

---

<a id="item-literature-news-7"></a>
### [New York Times Reviews Ted Scheinman&\#x27;s Memoir &\#x27;Jolt&\#x27; on Electroconvulsive Therapy](https://www.nytimes.com/2026/11/19/books/review/jolt-ted-scheinman.html) ⭐️ 5.0/10

The New York Times has published a review by Julia Scheeres of Ted Scheinman&\#x27;s &\#x27;Jolt,&\#x27; a personal account of his experience with electroconvulsive therapy. The review sets his account against the treatment&\#x27;s frightening public image, one traceable to the 1975 film &\#x27;One Flew Over the Cuckoo&\#x27;s Nest,&\#x27; and notes that Scheinman&\#x27;s actual experience was very different. The review appeared in the Times on November 19, 2026.

rss · New York Times Books · Nov 21, 15:54

**「About the author and the book」** Ted Scheinman&\#x27;s &\#x27;Jolt&\#x27; traces his long struggle with depression, which he traces to early childhood, and his eventual turn to electroconvulsive therapy as the last remaining medical option when his mental health and relationships continued to deteriorate. The memoir is already available in print and as an audiobook, and its release directly engages the treatment&\#x27;s lingering public image shaped by the 1975 film &\#x27;One Flew Over the Cuckoo&\#x27;s Nest.&\#x27;

**「For readers」** A prominent national review in the New York Times Book Review increases visibility for &\#x27;Jolt&\#x27; among readers interested in memoir and mental health, likely shaping how widely the book reaches audiences beyond psychiatric treatment communities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/society/2026/nov/08/ect-electroconvulsive-therapy-how-ted-scheinman-broke-through-depression">‘ I was in a darker place than I ’d ever been. ECT was my... | The Guardian</a></li>
<li><a href="https://www.audible.com/pd/Jolt-Audiobook/B0FXHJDJ3W">Jolt Audiobook by Ted Scheinman</a></li>
<li><a href="https://www.waterstones.com/book/jolt/ted-scheinman/9781035425198">Jolt by Ted Scheinman | Waterstones</a></li>

</ul>
</details>

**Tags**: `#book review`, `#memoir`, `#mental health`, `#New York Times`, `#electroconvulsive therapy`

---

<a id="item-literature-news-8"></a>
### [New York Times Reviews Gary Shteyngart&\#x27;s Essay Collection &\#x27;The Sensualist&\#x27;](https://www.nytimes.com/2026/11/16/books/review/gary-shteyngart-sensualist-pure-pleasure.html) ⭐️ 5.0/10

The New York Times Book Review has published a review by Jeff Giles of &\#x27;The Sensualist,&\#x27; a new essay collection by Gary Shteyngart. The review, dated November 16, 2026, highlights the book&\#x27;s playful personal essays, noting that Shteyngart swills martinis, calls on famous capybaras, and buys a life-changing bespoke suit across the pieces. The collection is presented as characteristically humorous, pleasure-focused writing rather than a major literary event.

rss · New York Times Books · Nov 21, 15:41

**「Context」** Gary Shteyngart is a widely reviewed contemporary American writer whose comic, autobiographical voice has made him a fixture in major outlets such as The New York Times, though this item is a book review rather than an award or industry announcement. The supplied evidence describes &\#x27;The Sensualist&\#x27; as a playful essay collection but provides no further details about his prior books or publishing history, so a fuller account of his trajectory is not possible here.

**「Impact」** Readers interested in contemporary humor and personal essays gain a guide to the collection&\#x27;s tone and subjects ahead of deciding whether to pick it up.

**Tags**: `#book review`, `#essay collection`, `#Gary Shteyngart`, `#New York Times`, `#contemporary fiction`

---

<a id="item-literature-news-9"></a>
### [A.O. Scott Reads Yeats&\#x27;s &\#x27;The Lake Isle of Innisfree&\#x27; in Short NYT Video](https://www.nytimes.com/video/books/review/100000011132055/this-poem-is-a-three-minute-vacation.html) ⭐️ 4.0/10

The New York Times Book Review published a short video feature in which critic at large A.O. Scott discusses William Butler Yeats&\#x27;s poem &quot;The Lake Isle of Innisfree&quot; and its final stanza. The video, credited to Léo Hamelin, Laura Salaberry, Efim Shapiro, and Adrienne Jeffries, frames the poem as an imagined escape from modern life whose speaker nonetheless remains &quot;on a gray pavement.&quot; Scott argues that the third stanza changes how the whole poem reads, presenting a brief, accessible appreciation of the canonical text rather than news of a publication or award.

rss · New York Times Books · Nov 21, 15:05

**「Context」** A.O. Scott is a critic at large for The New York Times, and this video appears as part of the newspaper&\#x27;s Book Review video features. The subject, W.B. Yeats&\#x27;s &quot;The Lake Isle of Innisfree&quot; \(1890\), is one of the most canonical poems in English, well known for imagining an idyllic island retreat while its speaker, as the source notes, remains on a &quot;gray pavement&quot; in the city.

**Tags**: `#poetry`, `#Yeats`, `#video feature`, `#criticism`

---