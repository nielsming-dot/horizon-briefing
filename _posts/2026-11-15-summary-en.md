---
layout: default
title: "Horizon Summary: 2026-11-15 (EN)"
date: 2026-11-15
lang: en
---

> From 163 items, 27 important content pieces were selected

---

**AI News**
1. [Runway open-sources Praxis-1, a video-trained vision-language-action robot model](#item-ai-news-1) ⭐️ 7.0/10
2. [SPU benchmark tests AI on predicting real wet-lab outcomes; frontier models fall short](#item-ai-news-2) ⭐️ 7.0/10
3. [DeepSeek opens full app-level API suite with search, OCR, ASR, and TTS endpoints](#item-ai-news-3) ⭐️ 7.0/10

**Technology News**
1. [Lovable-built apps leak passport data and 200K+ private messages over weak RLS](#item-tech-news-1) ⭐️ 8.0/10
2. [Asian governments react to Nvidia CEO Jensen Huang’s exit](#item-tech-news-2) ⭐️ 8.0/10
3. [SpaceX catches the Starship to end Flight 15](#item-tech-news-3) ⭐️ 7.0/10
4. [Project Zero Tightens Vulnerability Disclosure: 90 to 30 Days](#item-tech-news-4) ⭐️ 7.0/10
5. [PyPI&\#x27;s redesigned project pages with clearer security signals are now live](#item-tech-news-5) ⭐️ 7.0/10

**Medical News**
1. [Airstrike Hits Nasser Hospital&\#x27;s Surgical Wing, Underscoring Gaza&\#x27;s Health Crisis](#item-medicine-news-1) ⭐️ 7.0/10
2. [Trump Admin Pauses Enforcement of Its Medicaid Work Rules](#item-medicine-news-2) ⭐️ 7.0/10

**Astronomy News**
1. [James Webb telescope finds ice older than the star it orbits](#item-astronomy-news-1) ⭐️ 7.0/10
2. [SpaceX catches Starship upper stage with launch tower for first time](#item-astronomy-news-2) ⭐️ 6.0/10
3. [Is this iconic black hole image accurate? New study delivers an independent result](#item-astronomy-news-3) ⭐️ 6.0/10
4. [JWST spots lensed supernova SN Ares, predicts reruns in ~70 years](#item-astronomy-news-4) ⭐️ 6.0/10

**Energy News**
1. [Anthropic Reportedly Orders $3.4 Billion of Gas Engines for AI Data Centers](#item-energy-news-1) ⭐️ 6.0/10

**Oil and Gas Industry News**
1. [Magnolia Oil &amp; Gas to Acquire WildFire Energy in $4.06 Billion Deal](#item-oil-gas-news-1) ⭐️ 7.0/10
2. [New Mexico Federal Oil and Gas Lease Auction Draws Record $4 Billion in Bids](#item-oil-gas-news-2) ⭐️ 7.0/10
3. [Norway Oil Service Workers&\#x27; Strike Cuts Output by 2.4 Million boe](#item-oil-gas-news-3) ⭐️ 7.0/10
4. [Alaska Federal Lease Sale Draws $163 Million in Bids From Major Oil and Gas Companies](#item-oil-gas-news-4) ⭐️ 6.0/10
5. [Kazakhstan Oil Output Falls After Drone Attacks Close Export Terminal](#item-oil-gas-news-5) ⭐️ 6.0/10
6. [Shell Quarterly Profit More Than Doubles to $9.8 Billion on War-Driven Prices](#item-oil-gas-news-6) ⭐️ 6.0/10
7. [EnergyNow Lists Gulf Energy Infrastructure Damaged in Iran War](#item-oil-gas-news-7) ⭐️ 6.0/10

**Education News**
1. [Chicago Protests as Google Warns Districts Banning AI Could Lose Search Access](#item-education-news-1) ⭐️ 6.0/10

**Literature News**
1. [Guardian Long-Read: AI Accusations Rock the Literary World](#item-literature-news-1) ⭐️ 7.0/10
2. [New York Times Reviews &\#x27;The Absent Woman,&\#x27; First Biography of Journalist Eve Sneider](#item-literature-news-2) ⭐️ 6.0/10
3. [Lit Hub Weekly: Debut Novels, Olivia Waite Interview Lead November 9–13 Roundup](#item-literature-news-3) ⭐️ 4.0/10
4. [Profile: David Walliams, Children&\#x27;s Author, Faces Sexual Misconduct Allegations](#item-literature-news-4) ⭐️ 4.0/10

---

## AI News

<a id="item-ai-news-1"></a>
### [Runway open-sources Praxis-1, a video-trained vision-language-action robot model](https://the-decoder.com/runways-open-source-praxis-1-turns-video-ai-into-a-robot-controller/) ⭐️ 7.0/10

Runway has released Praxis-1, a World Action Model that takes camera images, text instructions, and robot position data to predict how a scene will change and derive matching robot movements, with weights and source code under the Apache 2.0 license, downloadable from Hugging Face and GitHub. The model builds on Runway&\#x27;s generative video research \(e.g., Gen-4.5\) and was fine-tuned with robot data, including about 277 hours from the public DROID dataset for a Franka arm and 1,400-2,600 hours for a dual-arm robot. Runway&\#x27;s self-reported results include a 46.2 percent success rate on Nvidia&\#x27;s RoboLab-120 benchmark \(versus 42.9 percent for FLUX 3 Action\), 88 of 100 successful task attempts on a real Franka arm versus FLUX 3 Action&\#x27;s 80, and an 80 percent average success rate on an unseen mobile robot platform after fine-tuning on about 95 hours of data, compared with 52.4 percent for Google&\#x27;s original RT-1. All results were run by Runway itself and have not been independently verified; the company also notes the model sometimes confuses similar-looking objects, struggles with vague instructions, and cannot reliably plan complex multi-step action sequences without explicit step-by-step instructions.

rss · The Decoder · Nov 14, 09:45

**「From video generation to robot control」** Runway is best known for generative video models such as Gen-4.5, and Praxis-1 extends that research into robotics: it starts from a video model that learned how objects move and interact from ordinary footage, then fine-tunes it with videos of human actions plus robot-specific data. Runway first introduced Praxis-1 in late September 2026 with access limited to select partners, including robotics companies Standard Bots, Noble Machines, and Ultra, before this wider open-weight release. The approach follows the broader vision-language-action trend, exemplified by Google&\#x27;s earlier RT-1 model, which serves as the comparison baseline in Runway&\#x27;s transfer tests.

**「Practical implications」** The Apache 2.0 license permits commercial use, letting robotics teams adapt Praxis-1 to their own hardware, though the base model requires additional training for new robot systems and the standard version needs an 80 GB GPU; a compressed version is expected to run on a 32 GB RTX 5090, but actual peak memory usage has not been measured per the GitHub docs. Pre-adapted versions for specific robots are already available, and developers must sign up and agree to access terms on Hugging Face before downloading.

**Tags**: `#open-weights`, `#robotics`, `#vision-language-action`, `#embodied-AI`, `#model-release`

---

<a id="item-ai-news-2"></a>
### [SPU benchmark tests AI on predicting real wet-lab outcomes; frontier models fall short](https://www.qbitai.com/2026/11/510232.html) ⭐️ 7.0/10

UniPat AI, with advisors and wet-lab collaborators from Stanford, Cornell, Harvard, UIC, Peking University, HKUST, FutureHouse, and several biotech companies, released Science Prediction Universe \(SPU\), a benchmark of 116 tasks \(100 public, drawn from 85 recent papers, and 16 private from four unpublished collaborations\) covering 4,207 real wet-lab experiments across chemistry, materials science, biology, and medicine. Models run autonomously for eight hours with 8-core CPUs, 16 GiB RAM, one H20 GPU, and internet access, then submit ranked orderings scored by Spearman correlation against hidden measured results, with scoring isolated in offline containers and automated checks for source-paper identifiers to guard against memory contamination. In the first evaluation of 12 frontier models across 13 configurations, the best average score was 0.486 \(Claude Opus 5.5\), and across configurations only 34%–52% of tasks exceeded a 95th-percentile random-ordering threshold, indicating no model yet performs reliably. Notably, raising GPT-6 Astra from medium to maximum reasoning effort increased median runtime 4.8x and median API cost 5.3x with almost no score change, and per-run API costs ranged from $0.22 to $65.91 across configurations; public task packages and code are open-sourced, while the 16 private tasks remain held back for controlled evaluation.

rss · 量子位 · Nov 14, 09:58

**「Prior context for wet-lab outcome prediction benchmarks」** Predicting wet-lab outcomes before running experiments has long been a purely human skill, but existing evaluations did not test it in the way SPU does: BrainBench asks models to judge reported experimental results directly, ScienceAgentBench focuses on analyzing already-collected data, and long-horizon benchmarks such as Terminal-Bench 4.0 and Long-Horizon-TB check task artifacts against preset tests. None of these combine an AI&\#x27;s autonomous research process with prediction of real, hidden experimental outcomes. SPU positions itself against that gap by requiring models to search literature, choose computational methods, and rank conditions over an eight-hour session, with scoring measured by Spearman correlation against measured results.

**「Impact」** For teams deploying models on scientific work, SPU shows that capability claims must be scoped to specific measurement targets: on private tasks, 13 configurations scored 0.89–0.95 predicting electrolyte ionic conductivity but -0.55 to 0.07 \(below random\) on electrochemical window, so a model that excels at one chemistry prediction may fail on another in the same domain. The 300x spread in per-run API cost also gives procurement teams a concrete cost-versus-accuracy basis for model selection, and the finding that extra compute and tool calls often add no predictive value suggests budgets are better spent auditing which computed quantities actually map to the experimental measurement. These results come from the benchmark organizers&\#x27; own paper and have not yet been independently reproduced.

**Tags**: `#benchmark`, `#ai-for-science`, `#wet-lab-prediction`, `#evaluation`, `#model-capability`

---

<a id="item-ai-news-3"></a>
### [DeepSeek opens full app-level API suite with search, OCR, ASR, and TTS endpoints](https://www.qbitai.com/2026/11/510003.html) ⭐️ 7.0/10

DeepSeek announced it has opened its full application-level capability suite as standalone API endpoints, including automated web search, Fetch, OCR, ASR, and TTS, each separately callable and separately billed, alongside an open-source lightweight chat frontend demo that supports importing DeepSeek conversation history. This builds on Search and Fetch endpoints first opened on October 17: developers previously had to wire tool calls to the model themselves, whereas the model can now automatically decide when to search, which pages to read, and how to answer from results. Voice is newly exposed, with ASR priced at 0.39 yuan/hour \(50% off the 0.78 yuan list price, roughly 1/3 to 1/16 of listed OpenAI and Google Cloud rates\) and TTS at 1.5 yuan per 10,000 characters; search remains 5 yuan per 1,000 successful calls and OCR 1.5 yuan per 1,000 pages. The V4.1-Flash model supports the conversation extensions under Messages, Responses, and Chat Completions interfaces; no benchmarks or independent evaluations are included in the announcement.

rss · 量子位 · Nov 14, 02:39

**「Background」** Before this release, DeepSeek&\#x27;s API exposed model inference but not the application-level features of its App: developers who wanted web-connected answers had to orchestrate tool calls themselves, and those building voice assistants had to integrate third-party ASR and TTS services. A partial step came on October 17, when DeepSeek first opened its in-house Search and Fetch endpoints, though developers still had to write the code linking model decisions to search calls and result summarization. The current release extends that trajectory by automating search orchestration and, for the first time, exposing voice capabilities as official standalone endpoints.

**「Why it matters for builders」** Developers building assistants, transcription, or document-processing products can now source search orchestration, parsing, and speech I/O from a single vendor at low unit prices instead of gluing separate providers — the stated ASR rate is about 4.6x cheaper than OpenAI GPT-Transcribe&\#x27;s listed hourly price. The main caveat is that the &\#x27;1:1 replica of the DeepSeek App&\#x27; framing is DeepSeek&\#x27;s own claim; pricing, reliability, and output quality should be verified in hands-on testing before committing production workloads.

**Tags**: `#deepseek`, `#api-release`, `#developer-tools`, `#voice-asr-tts`, `#web-search`, `#open-source`

---

## Technology News

<a id="item-tech-news-1"></a>
### [Lovable-built apps leak passport data and 200K+ private messages over weak RLS](https://www.crissyfield.de/research/lovable-en/) ⭐️ 8.0/10

Security research from Crissy Field found that apps built with the Lovable AI app-generation platform were exposing passport details and more than 200,000 private messages, exploitable simply by inspecting browser network calls. The leaks stem from insufficient Row-Level Security \(RLS\) in the apps&\#x27; Supabase-backed databases. Lovable&\#x27;s Head of Security, Igor Andri, acknowledged the findings and said the company automatically scans every app before publishing, offers a free deeper SAST scan, and provides auto-fix and publish-blocking options for flagged findings.

hackernews · armcat · Nov 14, 17:43 · [Discussion](https://news.ycombinator.com/item?id=50499017)

**「Background」** Lovable is an AI app-generation platform that lets non-developers create working applications from prompts, typically backed by the Supabase database service. Supabase relies on Row-Level Security \(RLS\), a Postgres feature that restricts which users can read or write each row of data; when RLS policies are missing or misconfigured, tables can become readable by anyone who knows the endpoint. The researcher&\#x27;s finding shows that apps generated this way often lacked sufficient RLS policies, meaning that casually browsing an app&\#x27;s network requests in a browser was enough to reach passport scans and hundreds of thousands of private messages.

**「Impact」** Users of apps built on Lovable may have their submitted personal data, including passport details and private messages, readable by anyone with a browser, since the apps require no sophisticated hacking knowledge to exploit. Builders using Lovable \(and Supabase backends generally\) should verify RLS is enabled on every table, run the available security scans, and enable auto-fix or publish blocking rather than assuming generated apps are secure by default.

**「Community Discussion」** Commenters disagreed over where responsibility lies: SOLAR\_FIELDS argued Supabase shares culpability because insecure database defaults were a deliberate onboarding tradeoff, with reports that the October 30 fix still doesn&\#x27;t apply to existing projects. Others, like liquid\_thyme and Oras, framed the incidents as evidence that AI app platforms need deny-by-default databases and least-privilege APIs, since AI-generated apps are numerous, easy targets that average users don&\#x27;t recognize as risky.

**Tags**: `#security`, `#ai-generated-code`, `#vibe-coding`, `#supabase`, `#row-level-security`

---

<a id="item-tech-news-2"></a>
### [Asian governments react to Nvidia CEO Jensen Huang’s exit](https://techcrunch.com/2026/11/14/asian-governments-react-to-nvidia-ceo-jensen-huangs-exit/) ⭐️ 8.0/10

Asian governments respond to the reported exit of Nvidia CEO Jensen Huang amid a board investigation into espionage allegations and personal misconduct, raising questions about chip supply commitments and AI industry ties.

rss · TechCrunch · Nov 14, 16:34

**Tags**: `#nvidia`, `#semiconductors`, `#geopolitics`, `#ai-industry`, `#corporate-leadership`

---

<a id="item-tech-news-3"></a>
### [SpaceX catches the Starship to end Flight 15](https://www.spacex.com/launches/starship-flight-15) ⭐️ 7.0/10

SpaceX successfully caught the Starship upper stage during Flight 15, marking a milestone toward fully reusable launch systems.

hackernews · ls612 · Nov 14, 21:22 · [Discussion](https://news.ycombinator.com/item?id=50500963)

**Tags**: `#spaceflight`, `#reusable-rockets`, `#SpaceX`, `#aerospace-engineering`, `#hardware`

---

<a id="item-tech-news-4"></a>
### [Project Zero Tightens Vulnerability Disclosure: 90 to 30 Days](https://projectzero.google/2026/11/disclosure-policy.html) ⭐️ 7.0/10

Google Project Zero announced that starting today its policy is &quot;Full 90&quot;: vulnerabilities are disclosed publicly 90 days after being reported to the vendor. The deadline then tightens in phases — to 60 days on February 2, 2027, and to 30 days on January 3, 2028. The announcement applies to all vendors and open source projects receiving Project Zero bug reports.

hackernews · hacb · Nov 14, 11:13 · [Discussion](https://news.ycombinator.com/item?id=50496051)

**「Background」** Project Zero is Google&\#x27;s security research team that reports vulnerabilities to affected vendors and, under the policy described in the announcement, publishes technical details after a fixed window once that window expires. The current baseline referenced in the announcement is a &quot;Full 90&quot; policy, meaning bugs are disclosed publicly 90 days after being reported, and the announced change tightens that deadline in two scheduled steps: to 60 days on February 2, 2027, and to 30 days on January 3, 2028. The fixed-deadline approach is intended to pressure vendors to patch promptly rather than delay fixes indefinitely, which is why commenters debated whether shorter windows give slow-moving projects, such as Linux distributions, enough time to ship updates.

**「Impact」** Vendors and open source maintainers will face progressively shorter fix windows, and a commenters&\#x27; concern suggests some, like Ubuntu, may struggle to patch complex issues within even 90 days. Organizations consuming affected software should expect faster public disclosure of unfixed vulnerabilities as the deadlines tighten.

**「Community discussion」** Commenter my-huge-pony relayed the policy details verbatim, while wewewedxfgdf argued distros like Ubuntu &quot;will need a LOT more time&quot; to comply. Glitchc went further, saying Project Zero should release bugs immediately since only public disclosure reliably compels vendors to fix them.

**Tags**: `#security`, `#vulnerability-disclosure`, `#project-zero`, `#policy`, `#infosec`

---

<a id="item-tech-news-5"></a>
### [PyPI&\#x27;s redesigned project pages with clearer security signals are now live](https://blog.pypi.org/posts/2026-11-06-ui-updates-complete/) ⭐️ 7.0/10

PyPI has rolled out redesigned project pages that surface clearer security signals, most notably build provenance, directly to users browsing package files. The change makes it visible at a glance whether a release was produced through attestable builds, such as those published via trusted publishing with keyless signing. Provenance is shown per release, though coverage is uneven: some projects publish it and others do not, so its absence does not itself indicate a compromised package.

hackernews · rbanffy · Nov 14, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50497892)

**「Background」** The new pages build on PyPI&\#x27;s existing support for build provenance, which is generated when maintainers publish packages using Trusted Publishing and sigstore-style keyless signing—short-lived OIDC-based credentials from a CI/CD system like GitHub Actions instead of long-lived upload tokens. Provenance records which build system produced a distribution and under what identity, letting users verify that an artifact came from the project&\#x27;s own pipeline rather than an unknown source. As commenters noted, coverage is not universal: some packages on PyPI already display provenance data while others do not, which is the gap the redesigned pages make visible.

**「Why it matters」** Maintainers who want the new signals to appear for their releases need to publish provenance, which in practice means adopting trusted publishing and OIDC-based keyless signing in their CI/CD pipelines. The visible per-package display also gives downstream users a concrete signal to check before pinning dependencies.

**「Community reaction」** Commenters largely welcomed the emphasis on provenance, with one noting that trusted publishing still lacks reusable-workflow support in GitHub Actions, and another hoping keyless signing pushes third-party CI providers to support secure OIDC. Skeptics argued the trust model centralizes on big cloud providers and risks lock-in, and one commenter cautioned that provenance only detects when a project&\#x27;s PyPI publishing path is hijacked, not inherently malicious projects.

**Tags**: `#pypi`, `#supply-chain-security`, `#package-management`, `#provenance`, `#sigstore`

---

## Medical News

<a id="item-medicine-news-1"></a>
### [Airstrike Hits Nasser Hospital&\#x27;s Surgical Wing, Underscoring Gaza&\#x27;s Health Crisis](https://www.medpagetoday.com/hospitalbasedmedicine/hospitalists/123869) ⭐️ 7.0/10

An Israeli airstrike on the surgical wing of Nasser Hospital, the largest hospital in southern Gaza, killed six people including a surgeon and a 13-year-old boy, and heavily damaged operating rooms and patient wards during a ceasefire that took effect in October 2025. The Israeli military said it targeted Muhammad Abu Ismail, whom it identified as a Hamas brigade commander using the hospital as a headquarters, but did not provide evidence or explain why the surgical unit was hit, and did not confirm whether he was killed. The World Health Organization has documented more than 1,050 attacks on health facilities in Gaza during the war, and the U.N. reports more than 1,700 medical personnel killed. These figures come from journalistic reporting and UN/Rights-group documentation rather than peer-reviewed data, and key claims, including the military&\#x27;s targeting justification, remain unverified.

rss · MedPage Today · Nov 14, 21:00

**「Context」** Gaza&\#x27;s healthcare system has been devastated by three years of war, including sieges and strikes on hospitals such as Gaza City&\#x27;s Shifa Hospital; at the war&\#x27;s worst points only 14 of Gaza&\#x27;s 36 prewar hospitals were functioning, and currently 20 operate, none fully. A WHO report from September 30 found 47% of essential medicines out of stock, with shortages of lab supplies, equipment, spare parts, and fuel. Under the Geneva Conventions, hospitals lose protected status only if used for military purposes, and even then a warning, proportionality, and civilian protection are required before an attack.

**「Practical Significance」** The destruction of Nasser Hospital&\#x27;s operating rooms further reduces surgical capacity in a territory where thousands of patients have life-changing war wounds and communicable disease is widespread, while Israel&\#x27;s continuing restrictions on medicines and equipment entry hinder reconstruction of services.

**Tags**: `#public health`, `#health policy`, `#conflict`, `#hospitals`, `#humanitarian crisis`

---

<a id="item-medicine-news-2"></a>
### [Trump Admin Pauses Enforcement of Its Medicaid Work Rules](https://www.medpagetoday.com/washington-watch/washington-watch/123887) ⭐️ 7.0/10

The Trump administration paused Medicaid work-requirement enforcement until July 1, 2027, giving states additional time to prepare for the national mandate effective January 1, 2027.

rss · MedPage Today · Nov 14, 18:09

**Tags**: `#health policy`, `#Medicaid`, `#work requirements`, `#CMS`, `#coverage`

---

## Astronomy News

<a id="item-astronomy-news-1"></a>
### [James Webb telescope finds ice older than the star it orbits](https://arstechnica.com/science/2026/11/james-webb-telescope-finds-ice-older-than-the-star-it-orbits/) ⭐️ 7.0/10

JWST detected amorphous water ice mixed with carbon dioxide in the Beta Pictoris debris disk, suggesting water-rich planet ingredients are common around young stars.

rss · Ars Technica Science · Nov 14, 12:15

**Tags**: `#astronomy`, `#astrophysics`, `#James Webb Space Telescope`, `#Beta Pictoris`, `#protoplanetary disks`, `#water ice`, `#comets`, `#planet formation`

---

<a id="item-astronomy-news-2"></a>
### [SpaceX catches Starship upper stage with launch tower for first time](https://www.space.com/space-exploration/launches-spacecraft/spacex-chopsticks-catch-starship-upper-stage-flight-14) ⭐️ 6.0/10

On Nov. 14, 2026, SpaceX caught the upper stage of its Starship rocket — Ship 42, launched on Flight 15 the previous evening from Starbase in South Texas — using the launch tower&\#x27;s &\#x27;chopstick&\#x27; arms, the first time the company has ever recovered an upper stage this way. The catch occurred at 4:20 p.m. EST \(2120 GMT\), roughly 22.5 hours after liftoff, with the ship returning from orbit. The mission&\#x27;s goal of catching both stages was not achieved: the Super Heavy booster diverted to a Gulf of Mexico splashdown after a low-fuel alarm. SpaceX had previously caught the Super Heavy booster on three test flights but had never attempted the maneuver with Ship, which flies higher, farther, and faster than the booster.

rss · Space.com · Nov 14, 13:00

**「Why the catch matters」** The upper stage is a harder catch target than the booster because it descends from orbital velocity and range, making a controlled tower landing far more demanding. SpaceX frames the catch as key to rapid inspection, refurbishment, and reflight of Starship, which the company says is required for the launch cadence needed to deploy large satellite constellations such as Starlink V3 and the proposed million-spacecraft Starmind AI data-center constellation.

**「Next steps」** SpaceX plans to attempt the double chopstick catch again, likely on the next Starship test flight, which the company says is not far off. Flight 15 also deployed 52 Starlink V3 satellites in low Earth orbit, following the first such deployment on Flight 14 in September, establishing a repeatable path for the constellation buildup.

**Tags**: `#spaceflight`, `#spacex`, `#starship`, `#rocket-recovery`, `#test-flight`

---

<a id="item-astronomy-news-3"></a>
### [Is this iconic black hole image accurate? New study delivers an independent result](https://phys.org/news/2026-11-iconic-black-hole-image-accurate.html) ⭐️ 6.0/10

A new study reportedly provides an independent check on the accuracy of the 2019 EHT image of M87&\#x27;s central black hole.

rss · Phys.org Space · Nov 15, 01:30

**Tags**: `#black hole`, `#EHT`, `#M87`, `#independent verification`, `#astrophysics`

---

<a id="item-astronomy-news-4"></a>
### [JWST spots lensed supernova SN Ares, predicts reruns in ~70 years](https://phys.org/news/2026-11-cosmic-magnifying-glass-reveal-supernova.html) ⭐️ 6.0/10

Using the James Webb Space Telescope, astronomers discovered a gravitationally lensed supernova, named SN Ares, whose light left its source when the universe was about 4.9 billion years old. The magnification by a massive foreground galaxy cluster distorted the explosion into multiple images arriving at different times. A discovery paper posted to the arXiv preprint server on Oct. 23 predicts that the remaining lensed images will reappear roughly 70 years from now, giving astronomers an unusually long scheduled window for follow-up. Because the result is a preprint rather than a peer-reviewed publication, the reappearance prediction should be treated as a candidate forecast pending review.

rss · Phys.org Space · Nov 14, 18:20

**「How gravitational lensing replays a supernova」** When light from a distant supernova passes near a massive galaxy cluster, the cluster&\#x27;s gravity bends and magnifies it, producing multiple images that reach Earth along paths of different lengths. Because each path adds a different delay, the same explosion can appear several times, separated by years or decades, a phenomenon previously seen in lensed supernovae such as Refsdal and in multiply imaged quasars. This makes strongly lensed transients valuable for measuring cosmic expansion, since the image time delays depend on the magnification and mass distribution of the lensing cluster.

**「What it enables」** The predicted ~70-year time delay turns SN Ares into a long-baseline target: future observatories can image the returning lensed views to measure the time delays directly, which constrains the mass distribution of the lensing cluster and can probe cosmic expansion rates through time-delay cosmography.

**Tags**: `#supernova`, `#gravitational lensing`, `#JWST`, `#high-redshift`, `#transient`

---

## Energy News

<a id="item-energy-news-1"></a>
### [Anthropic Reportedly Orders $3.4 Billion of Gas Engines for AI Data Centers](https://cleantechnica.com/2026/11/14/3-4-billion-anthropic-order-for-gas-power-plants/) ⭐️ 6.0/10

Anthropic has reportedly signed a $3.4 billion contract with OnePWR Solutions, a Texas-based energy company, to purchase gas-fired engines that would supply off-grid electricity to its AI data centers. According to the Financial Times, which broke the news, this is the largest known single purchase of power-generation equipment by an AI lab. The item is a reported deal rather than a commissioned or installed project, and the available coverage does not quantify the capacity, engine count, or delivery timeline. The purchase signals AI labs are turning to on-site fossil generation to bypass grid interconnection delays, drawing criticism given the associated CO2 and methane emissions.

rss · CleanTechnica · Nov 15, 00:33

**「Why an AI lab is buying its own power plants」** AI companies are increasingly procuring dedicated power equipment because grid interconnection queues and utility timelines cannot keep pace with data center buildouts, pushing labs toward off-grid generation. According to follow-up reporting on the Financial Times story, Anthropic signed the agreement in late September 2025 with OnePWR Solutions, and the deal covers gas-fired equipment capable of producing roughly 1.7 gigawatts of power to run its data centers independently of public electricity grids. The Financial Times described it as the largest known single purchase of power-generation equipment by an AI lab, though the reported figures have not been confirmed by Anthropic and the deal is a purchase agreement rather than commissioned capacity.

**「Why It Matters」** The deal indicates that AI data center power demand is being met with dedicated fossil generation rather than grid or renewable supply, meaning emissions occur directly at data center sites regardless of grid decarbonization progress. It also establishes a pricing benchmark for off-grid power equipment procurement by AI companies, potentially encouraging similar large-scale gas orders from competitors facing the same interconnection bottlenecks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techspot.com/news/114505-anthropic-going-rent-power-ai-data-centers-decided.html">Anthropic was going to rent power for its data centers, then... | TechSpot</a></li>
<li><a href="https://www.naturalnews.com/2026-11-11-anthropic-strikes-off-grid-power-agreement-reports.html">Anthropic Strikes $ 3 . 4 Billion Off-Grid Power Agreement to Bypass...</a></li>

</ul>
</details>

**Tags**: `#natural gas`, `#AI data centers`, `#Anthropic`, `#power procurement`, `#emissions`, `#market news`

---

## Oil and Gas Industry News

<a id="item-oil-gas-news-1"></a>
### [Magnolia Oil &amp; Gas to Acquire WildFire Energy in $4.06 Billion Deal](https://news.google.com/rss/articles/CBMilgFBVV95cUxPcVBXM1dLLWlsb1FCVHVmZ29aejE5aUc5cldRczNkZ2tTNEY2elZNTGctQzJkWXU1ak9jTVVSQnc5RVhBSGs5QWpOeWVnc1pwRENIVWQ4eURYdlVIQ1JmRVFkZkJPTHJYUVowT1k0XzhoYzhCbEhRc0ZhRUpmZGN0cno3VUZUM0hmZUt3OGFQd0c1MjZqQnc?oc=5) ⭐️ 7.0/10

Magnolia Oil &amp; Gas has announced an agreement to acquire WildFire Energy in a transaction valued at $4.06 billion. The announcement, reported by EnergyNow.com, establishes Magnolia as the acquirer and WildFire Energy as the target in the upstream consolidation move. Details beyond the headline deal value, including transaction structure, expected closing timeline, and regulatory conditions, are not provided in the available source. The transaction is an announced deal and its completion remains subject to customary closing conditions.

rss · Google News Oil &amp; Gas \(EN\) · Nov 14, 13:38

**「Deal Context」** Magnolia Oil &amp; Gas said it agreed to acquire the privately held WildFire Energy for approximately $4.06 billion, including debt, to expand its position in the Giddings field in South Texas, where the Eagle Ford and Austin Chalk plays are located. The transaction adds roughly 810,000 net acres in the Giddings field and more than 500 miles of gas gathering pipelines in South Texas. Under the terms, WildFire shareholders will receive 32.2 million Magnolia shares, and Magnolia will assume WildFire&\#x27;s $600 million of outstanding notes due 2029.

**「Consolidation Effect」** If completed, the acquisition would consolidate assets under Magnolia Oil &amp; Gas, expanding its upstream portfolio through the $4.06 billion purchase. The full operational impact, including effects on production volumes and asset locations, cannot be assessed from the available source information.

<details><summary>References</summary>
<ul>
<li><a href="https://boereport.com/2026/07/20/magnolia-oil-gas-to-buy-wildfire-energy-in-4-06-billion-deal/">Magnolia Oil &amp; Gas to buy WildFire Energy in $ 4 . 06 billion deal</a></li>
<li><a href="https://pgjonline.com/news/2026/july/magnolia-buys-wildfire-energy-in-406-billion-deal-adds-500-miles-of-pipelines?trk=article-ssr-frontend-pulse_little-text-block">Magnolia Buys WildFire Energy in $ 4 . 06 Billion Deal , Adds 500 Miles...</a></li>
<li><a href="https://finance.yahoo.com/energy/articles/magnolia-oil-gas-acquire-wildfire-113309877.html">Magnolia Oil &amp; Gas to Acquire WildFire Energy for $ 4 . 06 Billion</a></li>

</ul>
</details>

**Tags**: `#M&amp;A`, `#Magnolia Oil &amp; Gas`, `#WildFire Energy`, `#upstream`, `#consolidation`

---

<a id="item-oil-gas-news-2"></a>
### [New Mexico Federal Oil and Gas Lease Auction Draws Record $4 Billion in Bids](https://news.google.com/rss/articles/CBMiqgFBVV95cUxQVnhGakZiM2FxS3dkRVVJMlpuT0FzNHBCX3BaQ2RlS3pMeU5lbEdCcVNXeHZqYnpyeE92NDFJMDdMY2xxVVR0X2FINEF5bW9KRU9id3p5NXFHZVcyS1lZMk5uOE4ySlV4eENoZ0V6eWFTTDh6TFBpNFB4WGVfSVg3b2FGd3VlZFZTNGJIQnQ0b2VONU5GUnBid2pMdTZqT0RtSk5mb3dDRkpnZw?oc=5) ⭐️ 7.0/10

A US federal oil and gas lease auction covering New Mexico acreage attracted a record $4 billion in bids, according to EnergyNow.com. The result marks a record level of bidding for such a sale in the state, which sits at the core of the Permian basin. Details such as the number of tracts, total acreage offered, and the winning bidders were not included in the available source material.

rss · Google News Oil &amp; Gas \(EN\) · Nov 14, 14:06

**「Context」** The result stems from a quarterly Bureau of Land Management lease sale covering 74 parcels across roughly 33,530 acres in New Mexico and Texas, with bonus bids and rental payments totaling about $4.01 billion, making it the largest onshore federal oil and gas lease sale on record. Under the federal revenue-sharing framework, proceeds are split between the federal government and the states hosting the parcels, with New Mexico set to receive about $2 billion. Large exploration and production companies, including major Permian operators, competed aggressively for the high-quality acreage, explaining the record bidding intensity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kwtx.com/2026/05/23/bureau-land-management-announces-historic-oil-gas-lease-sale-new-mexico-texas/">The Bureau of Land Management announces historic oil and gas ...</a></li>
<li><a href="https://www.organmountainnews.com/new-mexico-texas-oil-gas-lease-sale-4-billion-2026/">Interior Department oil and gas lease sale in New Mexico , Texas...</a></li>
<li><a href="https://www.oilgasandenergy.com/post/oil-and-gas-lease-sale-in-new-mexico-and-texas-raises-4-billion">Oil and gas lease sale in New Mexico and Texas raises $ 4 billion</a></li>

</ul>
</details>

**Tags**: `#leasing`, `#federal auction`, `#New Mexico`, `#Permian`, `#bid numbers`

---

<a id="item-oil-gas-news-3"></a>
### [Norway Oil Service Workers&\#x27; Strike Cuts Output by 2.4 Million boe](https://news.google.com/rss/articles/CBMitgFBVV95cUxQekpVSGhLeGRWeW1SQURmWnZpVkhtbVNZQ3ZYUEF4OEVkTXNTZlpCRHBaMVpiMXBlTmhyTDNNSVkxQlJCU3lUWEVXRUc4M29zLVFrNFdLUG40NDY5ODNJVFlpejZVdU5Wcm5RVW11UkhhdTdOMHpiRllSYVo2Szd3MTZzQWg1Mlhwd040YXhzVGlabzNGWW1CME5wajFqcFJMNjZvb1lhRTA1UmNiVEtLMlpLSFE0QQ?oc=5) ⭐️ 7.0/10

An industry group reports that a strike by oil service workers in Norway has cut production by 2.4 million boe. The figure&\#x27;s basis — whether cumulative since the strike began or another measure — and details on affected fields and strike duration were not specified in the reported headline. Norway is a major offshore producer, so the labor dispute represents a direct supply-side disruption, though its persistence depends on how long the stoppage continues.

rss · Google News Oil &amp; Gas \(EN\) · Nov 14, 13:56

**「Background」** Norway&\#x27;s oil service workers have been on strike since June 15, 2026, after wage negotiations between the unions and employers collapsed. Industry group Offshore Norway reports the dispute has reduced the country&\#x27;s oil and gas production by a cumulative 2.4 million barrels of oil equivalent so far this year, with estimated financial losses of $163.6 million when projected impacts are included. The conflict subsequently escalated into a lockout of around 1,000 oil service workers, disrupting drilling and some production on the Norwegian continental shelf.

**「Impact」** The stoppage removes barrels from a major producing country&\#x27;s export supply, which can tighten regional North Sea crude availability and affect service-sector scheduling for operators if the strike extends; the limited detail prevents a firm assessment of the disruption&\#x27;s market significance.

<details><summary>References</summary>
<ul>
<li><a href="https://boereport.com/2026/07/09/norway-oil-service-workers-strike-cuts-output-by-2-4-million-boe-industry-group-says/">Norway oil service workers ’ strike cuts output by 2 . 4 million boe ...</a></li>
<li><a href="https://energiesmedia.com/norway-oil-strike-offshore-output-energy/">Norway oil service workers &#x27; strike reduces offshore output by...</a></li>
<li><a href="https://www.offshore-mag.com/regional-reports/north-sea-europe/news/55387624/norway-oil-service-lockout-takes-effect-disrupts-offshore-drilling">Norway oil service lockout takes effect , disrupts... | Offshore Magazine</a></li>

</ul>
</details>

**Tags**: `#Norway`, `#strike`, `#production disruption`, `#offshore`, `#labor`

---

<a id="item-oil-gas-news-4"></a>
### [Alaska Federal Lease Sale Draws $163 Million in Bids From Major Oil and Gas Companies](https://news.google.com/rss/articles/CBMivgFBVV95cUxNVlA0MURHODIwellzbHRRZkM2ckxaNTMwM1NNNnBrQm81MllVS0g1LWVVVHY0RXpKT3Z4SWxOQVItQU92RGVnemtUbmJMYmJvWjQzZHJZcFB3T2ROY0x4ZDlOLXp5ZWxfQ3FTOVZNZFF4R2pNUWFaa3hzOGZCTXZyYlhQVGhHV1RoMHRLWnhWdG5vVENqRDg2TkZMT1F3dy1PLVZFank3aXlabEFPM2ZNenoyUHRMdUhxTzBTYUlB?oc=5) ⭐️ 6.0/10

An Alaska oil and gas lease sale held under the Trump administration attracted $163 million in bids from major industry players, according to EnergyNow.com. The report confirms the headline bidding total but does not detail the acreage offered, the specific leases sold, or the identities of all participating companies. Details on the sale&\#x27;s scope and winning bidders were not provided in the available report, so the significance of the $163 million figure relative to prior sales remains unclear.

rss · Google News Oil &amp; Gas \(EN\) · Nov 14, 13:40

**「Context」** The sale covered drilling rights in the National Petroleum Reserve–Alaska \(NPR-A\), a federally managed area on Alaska&\#x27;s North Slope that the Trump administration has opened to expanded leasing. The Interior Department issued 187 leases in what has been described as the most successful NPR-A lease sale to date, with ConocoPhillips, Exxon Mobil, Shell, and Repsol among the winning bidders. The result reflects the administration&\#x27;s policy of prioritizing federal leasing and permitting to encourage Alaska energy development.

**「Industry Implications」** Significant bidding from major operators indicates continued industry interest in Alaskan exploration acreage under the current federal leasing posture, though exploration success and any future development decisions would follow only after drilling results. Until the winning companies and lease locations are disclosed, the effect on Alaska&\#x27;s supply outlook or operator portfolios cannot be quantified.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/global-energy-network_usgovernment-alaska-npra-activity-7440426948427751425-0UcI">US Govt Sells Alaska Oil Leases for $ 163 M to Repsol, Shell... | LinkedIn</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-03-18/oil-giants-bid-163-million-in-trump-s-record-alaska-lease-sale">Oil Giants Bid $ 163 Million in Trump ’s Record Alaska Lease Sale</a></li>
<li><a href="https://www.powerthefuture.com/alaska-lease-sale-shows-what-real-energy-leadership-looks-like/">Alaska Lease Sale Shows What Real Energy... - Power The Future</a></li>

</ul>
</details>

**Tags**: `#Alaska`, `#lease sale`, `#US policy`, `#licensing`, `#federal offshore`

---

<a id="item-oil-gas-news-5"></a>
### [Kazakhstan Oil Output Falls After Drone Attacks Close Export Terminal](https://news.google.com/rss/articles/CBMixwFBVV95cUxNUEN3X1RsX3VzbUFYalIxUExOdi1DaVBsNnVkTV9LS0F4dm9XS2xxc0p5UmxzWWVzblYzZzlRMnBHMVNqX1pQeFhmcnFxX0ROQmo2TWRWYUlFZC1xdlcyUzJfT0VOMWhoaUxOZWx3OVc2M2JYQzkxeHZuakxVc2NjZ25GaGNzQjF4aThHR1lydWdXZ2NJM0ZpWERqdTN3VUxNbW01UnVwV3BPd25IZDV4d002U0RyZ0djZFVPSGdUUEZiTDIzaWp3?oc=5) ⭐️ 6.0/10

Kazakhstan&\#x27;s oil output reportedly fell sharply after drone attacks forced the closure of a key crude exporting terminal, according to a headline-only report by EnergyNow.com citing sources. The report does not identify the terminal, state output volumes, or indicate how long the disruption is expected to last, and the underlying figures cannot be verified from the available item. The event remains an unconfirmed supply disruption claim pending further reporting.

rss · Google News Oil &amp; Gas \(EN\) · Nov 14, 13:14

**「Context」** Kazakhstan, one of the world&\#x27;s ten largest oil producers, depends heavily on a single export route: the Caspian Pipeline Consortium terminal on Russia&\#x27;s Black Sea coast, which handles the bulk of its crude and, unusually for a Kazakh export artery, sits on Russian territory. Reuters reported in late July 2026 that suspected Ukrainian drone attacks forced this main export terminal to close and that Kazakhstan had cut production, with a source saying daily output had more than halved as a result. By August 2026, Kazakh authorities had acknowledged that the country&\#x27;s 2026 oil and condensate production would not reach the previous year&\#x27;s record high because of the drone attacks on the export pipeline and terminal, underscoring how exposure of its export infrastructure to the Russia-Ukraine conflict directly constrains national output.

**「Impact」** If confirmed, the closure of a Kazakh export terminal would remove crude barrels from export flows that pass largely through Black Sea and Caspian routes, tightening available supply for buyers of Kazakh grades. However, the scale and duration of the effect cannot be assessed because the headline-only report provides no volume, terminal, or timeline detail.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/business/energy/kazakhstans-oil-output-plummets-after-drone-attacks-forced-exporting-terminal-2026-07-23/">Kazakhstan slows oil output after drone strikes on export ...</a></li>
<li><a href="https://www.upstreamonline.com/production/black-sea-terminal-attacks-dent-kazakhstan-oil-ambitions/2-1-2033986?zephr_sso_ott=5iR65a">Black Sea terminal attacks dent Kazakhstan oil ambitions</a></li>
<li><a href="https://www.reuters.com/business/energy/kazakhstans-daily-oil-output-halves-after-exporting-terminal-closure-source-says-2026-07-27/">Kazakhstan&#x27;s daily oil output halves after export terminal ...</a></li>

</ul>
</details>

**Tags**: `#Kazakhstan`, `#supply disruption`, `#drone attacks`, `#export terminal`, `#crude output`

---

<a id="item-oil-gas-news-6"></a>
### [Shell Quarterly Profit More Than Doubles to $9.8 Billion on War-Driven Prices](https://news.google.com/rss/articles/CBMixAFBVV95cUxPa0plQVFmeFNZX3hwVmZ6TXFVaXAxb0dELTVVZXo0RFRXVnRfS09XU24xalZYdE9kR0M1M3R1eElCV0F4cDg0ZTNfS1R4MmFJZU5EV1FFS0NhNGxaWldqaVFGSnIwRkV2dTh5eHotSjZWek85OUJ0OGV6cmV0QWVneVgyQ195SERfYVBLdUlEX0RhZ2h1WkZMVEFRbGsydGx4a2dvVWtPMEV4VjZYSU10QW9zcjh5ZTNDNmExWkpBY0c3ZFF1?oc=5) ⭐️ 6.0/10

Shell reported a quarterly profit that more than doubled to $9.8 billion, the second-highest result in the company&\#x27;s record, according to EnergyNow.com. The company attributed the surge primarily to elevated oil and gas prices driven by the Iran war. The available source material does not disclose segment-level performance, production volumes, shareholder distributions, or forward guidance, so the durability of the earnings level beyond this quarter remains unclear.

rss · Google News Oil &amp; Gas \(EN\) · Nov 14, 07:48

**「Context」** Shell&\#x27;s second-quarter 2026 net profit of $9.84 billion, reported on July 30, beat analyst expectations and came amid higher energy prices and increased market volatility. The Middle East conflict, particularly involving Iran, fueled a boom in trading and refining results that lifted earnings across global energy companies, according to Reuters and Bloomberg reporting.

**「Why It Matters」** For Shell and its peers, the result demonstrates how sharply geopolitical risk premiums on oil prices translate directly into supermajor earnings, strengthening near-term cash flow available for shareholder returns and investment decisions. However, because the gain is tied to a war-driven price environment rather than structural factors, it signals earnings volatility rather than a lasting shift in the industry&\#x27;s cost or supply position.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/business/energy/shell-more-than-doubles-its-profit-q2-beating-expectations-2026-07-30/">Shell profit more than doubles to $9.8 billion, second ...</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-07-30/shell-reports-profit-surge-as-oil-trading-and-refining-boom">Shell Profit Surges to $9.8 Billion on Oil Trading and ...</a></li>
<li><a href="https://www.globalbankingandfinance.com/shells-profit-doubles-9-8-billion-iran-war-boosts-oil-gas/">Shell Profits Double to $9.8B as Iran Conflict Lifts Oil, Gas ...</a></li>

</ul>
</details>

**Tags**: `#Shell`, `#earnings`, `#supermajor`, `#oil prices`, `#geopolitics`

---

<a id="item-oil-gas-news-7"></a>
### [EnergyNow Lists Gulf Energy Infrastructure Damaged in Iran War](https://news.google.com/rss/articles/CBMilwFBVV95cUxQdjVzWWVVSWthaTRmcmRHRk40Tno3SngwdnBUb1pxT3lxdHN5bC1KLUFPbGs1eEZGX3BrYTJjVXhkdHI4M3RRMkJQck5fWUFsd043d1pMckxlVExwYUJkYzh6TWdBWDlGT1Y1Rjk0cTVobFkxa09Ma3NMbklCdXJuZGtFdlVzRGs5YTVzQTFqUmY0V1VRZjRB?oc=5) ⭐️ 6.0/10

EnergyNow published a roundup listing Gulf energy infrastructure that sustained damage during the Iran war, according to the headline. The supplied content consists only of the headline and link, without the underlying article, so no named facilities, damage extents, production impacts, or repair timelines can be confirmed from this item.

rss · Google News Oil &amp; Gas \(EN\) · Nov 14, 11:59

**「Context」** The supplied item consists only of a headline; EnergyNow&\#x27;s list of Gulf energy infrastructure damaged in the Iran war is not reproduced here, so no specific facilities, damage assessments, or timelines can be confirmed from the available content. Any background on the individual assets referenced would require the full underlying article, which was not supplied.

**「Why it matters」** Damage to Gulf energy infrastructure bears directly on regional supply reliability and shipping risk through the Persian Gulf, making the full list a decision-relevant reference for operators and traders; however, the specific consequences cannot be assessed until the named facilities and damage details in the underlying article are verified.

**Tags**: `#Middle East`, `#geopolitics`, `#infrastructure damage`, `#supply risk`, `#Iran conflict`

---

## Education News

<a id="item-education-news-1"></a>
### [Chicago Protests as Google Warns Districts Banning AI Could Lose Search Access](https://www.the74million.org/article/protests-in-chicago-after-google-warns-schools-about-disabling-ai-feature/) ⭐️ 6.0/10

Protests took place Wednesday in Chicago and Cambridge, Massachusetts, after Google said earlier this month that schools banning generative AI would not be able to use its search engine, because AI is embedded in the technology. Chicago Public Schools, which recently blocked student access to generative AI tools such as ChatGPT, Claude, and Google Gemini, has not finalized a response; a district spokesperson said CPS is exploring options to independently suppress the AI overview atop Google searches or shift to other search solutions. About 30 protesters, mostly parents and educators with some students, demonstrated outside Google&\#x27;s Chicago office, led by Illinois Families for Public Schools, which wants a three-year moratorium on generative AI in CPS classrooms. Google said it is piloting a &quot;Guided Learning&quot; feature that walks students through problems step-by-step rather than giving quick answers, but the district-level conflict remains unresolved.

rss · The 74 · Nov 14, 11:30

**「Background」** Chicago Public Schools&\#x27; conflict with Google follows earlier district decisions on generative AI: despite previously approving tools including Google Gemini, Microsoft Copilot, and Gemini Notebook under contracts barring student data from training AI models, CPS abandoned a planned rollout of Gemini in high schools for 2026-2027 after community pushback. The district&\#x27;s recent block on student access to generative AI tools such as ChatGPT, Claude, and Google Gemini set the stage for the current dispute over Google&\#x27;s warning that schools banning AI may lose access to search. The protest was led by Illinois Families for Public Schools, which has sought a three-year moratorium on generative AI in CPS and urged school board candidates to sign its pledge, with about half of incoming board members doing so.

**「Why it matters」** Districts restricting student-facing AI may face a concrete access problem: if they cannot technically disable Google&\#x27;s AI features, CPS has indicated it would seek alternative search solutions, potentially requiring new procurement, costs, and changes to how students research. The dispute also highlights that CPS had previously approved at least three generative AI tools, including Google Gemini and Microsoft Copilot, and backtracked on a planned Gemini rollout in high schools for 2026-2027 after community pushback, leaving district AI policy in flux.

**Tags**: `#AI in education`, `#edtech`, `#K-12 policy`, `#Google Gemini`, `#Chicago Public Schools`, `#protests`

---

## Literature News

<a id="item-literature-news-1"></a>
### [Guardian Long-Read: AI Accusations Rock the Literary World](https://www.theguardian.com/books/ng-interactive/2026/nov/14/its-like-the-wild-west-how-ai-has-rocked-the-literary-world) ⭐️ 7.0/10

Sophie McBain&\#x27;s Guardian long-read, published 14 November 2026, examines how AI is disrupting the publishing industry, from authors losing lucrative deals to writers being removed from prize shortlists. The feature argues that accusations and use of machine writing are spreading with little oversight, captured in the framing that &quot;it&\#x27;s like the wild west.&quot; A central case study is romance novelist Coral Hart, who broke in with Mills &amp; Boon before turning to self-publishing; since 2025 she has written 370 novels under 21 pen names using AI, earning &quot;high six figures.&quot; The piece situates this within the economics of platforms like Kindle Unlimited, whose algorithms reward prolific output, and asks whether the tide of machine writing can still be turned back.

rss · Guardian Books · Nov 14, 09:00

**「Industry context」** This feature lands amid a wave of AI-related disputes in publishing. In one prominent case, Haitian-Canadian author Thélyson Orélien&\#x27;s bestselling novel—winner of the Fnac novel prize—was removed from the Prix Goncourt shortlist in September 2026 after an anonymous X account used the AI detector Pangram to claim it was machine-written. The economics described in the piece, such as Kindle Unlimited rewarding prolific output, mirror a self-publishing landscape that was already competitive before AI made high-volume writing dramatically easier.

**「What It Means」** The report signals that AI has become a live career risk for authors: unproven accusations of AI use are now affecting book deals and prize shortlists, while AI-assisted writers compete at scale on subscription platforms, pressures that self-published and traditionally published authors alike must navigate.

<details><summary>References</summary>
<ul>
<li><a href="https://theconversation.com/a-bestselling-novel-was-pulled-from-a-french-literary-prize-after-ai-accusations-what-next-292963">A bestselling novel was pulled from a French literary prize after AI ...</a></li>
<li><a href="https://www.archyde.com/french-bestselling-novel-dropped-from-literary-prize-over-ai-accusations/">French Bestselling Novel Dropped From Literary Prize Over AI ...</a></li>

</ul>
</details>

**Tags**: `#AI and publishing`, `#industry debate`, `#authorship`, `#Guardian feature`, `#self-publishing`

---

<a id="item-literature-news-2"></a>
### [New York Times Reviews &\#x27;The Absent Woman,&\#x27; First Biography of Journalist Eve Sneider](https://www.nytimes.com/2026/11/11/books/review/the-absent-woman-eve-sneider.html) ⭐️ 6.0/10

The New York Times has published a review by Jennifer Szalai of &\#x27;The Absent Woman,&\#x27; the first biography of journalist Eve Sneider. The review describes the book as drawing on Sneider&\#x27;s archives to portray the person behind her public legend, presenting her as a complex and contradictory figure rather than simply confirming the formidable reputation she carried in journalism.

rss · New York Times Books · Nov 14, 04:12

**「Context」** The review, by Jennifer Szalai in The New York Times Book Review, marks the first biography of Eve Sneider, a journalist described in the source as a formidable figure whose legend has outlasted her. Because the book draws directly on Sneider&\#x27;s archives, the review is positioned to assess how archival material reshapes the public image of a journalist previously known mainly by reputation.

**Tags**: `#book review`, `#biography`, `#journalism`, `#New York Times`, `#new publication`

---

<a id="item-literature-news-3"></a>
### [Lit Hub Weekly: Debut Novels, Olivia Waite Interview Lead November 9–13 Roundup](https://lithub.com/lit-hub-weekly-november-9-13-2026/) ⭐️ 4.0/10

Literary Hub published its weekly digest for November 9–13, 2026, aggregating essays, interviews, and reading lists from across the literary web. The roundup highlights two Lit Hub features: Maris Kreizman&\#x27;s list of ten overlooked 2026 debut novels, and an interview by Zachary Fletcher with former New York Times romance columnist Olivia Waite discussing her firing and the current state of romance criticism. The digest also links to external pieces, including Adam Gopnik on The Sun Also Rises at 100 and Laura Miller in Slate on the closure of Salon, and marks the anniversary of David Copperfield concluding serial publication in 1850.

rss · Literary Hub · Nov 14, 11:30

**「Background」** Literary Hub \(Lit Hub\) is an online literary magazine that publishes a weekly digest aggregating its own essays and interviews alongside notable pieces from other outlets such as Slate, The New Yorker, The Paris Review, and The Nation. The November 9–13, 2026 installment follows that routine format, gathering book-list features, criticism, and interviews rather than reporting a single literary event.

**「Impact」** The linked feature on overlooked debut novels gives lesser-known 2026 authors added visibility and points readers toward titles they may otherwise have missed, while the Waite interview documents debates over the state of romance criticism at major outlets.

**Tags**: `#roundup`, `#debut novels`, `#romance criticism`, `#interviews`, `#reading lists`

---

<a id="item-literature-news-4"></a>
### [Profile: David Walliams, Children&\#x27;s Author, Faces Sexual Misconduct Allegations](https://www.nytimes.com/2026/11/10/world/europe/who-is-david-walliams-sexual-misconduct-allegations-uk.html) ⭐️ 4.0/10

A New York Times explainer profiles David Walliams, the British entertainer and author of more than 40 children&\#x27;s books, following sexual misconduct allegations against him. The piece outlines his rise to fame through the television show &quot;Little Britain&quot; and his parallel career as a prolific children&\#x27;s author. The supplied evidence does not describe the specific allegations in detail or any resulting professional consequences.

rss · New York Times Books · Nov 14, 11:06

**「Context」** David Walliams first rose to fame in Britain through the television comedy series &quot;Little Britain&quot; before building a parallel career as a writer. He has since published more than 40 children&\#x27;s books, making him one of the UK&\#x27;s most prolific authors for young readers. The New York Times explainer profiles his career in light of the recent sexual misconduct allegations against him.

**「Impact」** Walliams&\#x27;s standing in children&\#x27;s publishing makes his work a visible category for readers and booksellers to watch, though no publisher actions or book cancellations are reported in the supplied coverage.

**Tags**: `#celebrity`, `#children&\#x27;s books`, `#misconduct allegations`, `#publishing`, `#UK`

---