---
layout: default
title: "Horizon Summary: 2026-11-23 (EN)"
date: 2026-11-23
lang: en
---

> From 142 items, 19 important content pieces were selected

---

**AI News**
1. [Security researchers show how cheap AI inference providers steal keys and snoop on users](#item-ai-news-1) ⭐️ 8.0/10
2. [Perplexity and Intelligence](#item-ai-news-2) ⭐️ 7.0/10
3. [METR: AI Capability Growth Is Outpacing Safety Evaluation Capacity](#item-ai-news-3) ⭐️ 7.0/10
4. [Anthropic mathematician with Claude claims proof of Navier–Stokes blow-up; human-only Riemann draft released same day](#item-ai-news-4) ⭐️ 7.0/10

**Technology News**
1. [派早报：Anthropic 研究员宣称用 Claude 证明黎曼猜想](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI’s chief scientist has thoughts on how to limit AI development](#item-tech-news-2) ⭐️ 7.0/10

**Astronomy News**
1. [Gap in 257 black hole mergers hints at failed supernovae](#item-astronomy-news-1) ⭐️ 7.0/10
2. [BepiColombo went into orbit around Mercury yesterday\!](#item-astronomy-news-2) ⭐️ 7.0/10
3. [JWST finds a possible black hole that grew faster than its host galaxy in the early universe](#item-astronomy-news-3) ⭐️ 6.0/10
4. [Milky Way simulation reaches record resolution with the help of three supercomputers](#item-astronomy-news-4) ⭐️ 6.0/10

**Energy News**
1. [Ford Begins Producing Its Own LFP Batteries](#item-energy-news-1) ⭐️ 7.0/10

**Oil and Gas Industry News**
1. [US Lends 8.5 Million Barrels of SPR Crude, Second Loan Since Iran War Began](#item-oil-gas-news-1) ⭐️ 6.0/10

**Literature News**
1. [Jilly Cooper&\#x27;s Prudence faces plagiarism allegations](#item-literature-news-1) ⭐️ 6.0/10
2. [Review: Nancy Isenberg&\#x27;s &\#x27;Aristocracy, American Style&\#x27;](#item-literature-news-2) ⭐️ 6.0/10
3. [Huw Green Explains How Psychosomatic Illnesses Arise](#item-literature-news-3) ⭐️ 5.0/10
4. [A.O. Scott Reads Yeats&\#x27;s &\#x27;The Lake Isle of Innisfree&\#x27; in New NYT Video Essay](#item-literature-news-4) ⭐️ 5.0/10
5. [Married Couple&\#x27;s Murder-Mystery Puzzle Book Sells 100,000 Copies](#item-literature-news-5) ⭐️ 4.0/10
6. [Misty Copeland Reviews Lynn Garafola&\#x27;s Biography of Arthur Mitchell](#item-literature-news-6) ⭐️ 4.0/10
7. [NYT Book Review Editor Picks Three Books Ahead of December Screen Adaptations](#item-literature-news-7) ⭐️ 4.0/10

---

## AI News

<a id="item-ai-news-1"></a>
### [Security researchers show how cheap AI inference providers steal keys and snoop on users](https://the-decoder.com/security-researchers-show-how-cheap-ai-inference-providers-steal-keys-and-snoop-on-users/) ⭐️ 8.0/10

Dragos researchers used ~2 million decoy requests to expose compromised AI inference providers actively stealing API credentials and user data, implicating intermediaries and model marketplaces as a major security risk.

rss · The Decoder · Nov 22, 12:07

**Tags**: `#ai-security`, `#credential-theft`, `#inference-providers`, `#incident-report`, `#supply-chain`, `#api-keys`, `#security-research`

---

<a id="item-ai-news-2"></a>
### [Perplexity and Intelligence](https://openai.com/index/perplexity-and-intelligence/) ⭐️ 7.0/10

An OpenAI essay exploring the correspondence between perplexity \(cross-entropy loss\) and model intelligence, generating significant technical discussion about scaling laws and the role of pretraining metrics.

hackernews · acossta · Nov 22, 17:06 · [Discussion](https://news.ycombinator.com/item?id=50601525)

**Tags**: `#scaling-laws`, `#perplexity`, `#openai`, `#model-evaluation`, `#pretraining`, `#research-analysis`

---

<a id="item-ai-news-3"></a>
### [METR: AI Capability Growth Is Outpacing Safety Evaluation Capacity](https://the-decoder.com/ai-is-getting-better-faster-than-experts-can-reliably-test-whether-new-systems-are-safe-metr-warns/) ⭐️ 7.0/10

AI research organization METR warns that AI models are improving at research tasks faster than experts can reliably evaluate them, and that current public data cannot rule out a drastic acceleration in AI research over the next few years. On clearly defined coding and computational tasks with direct feedback, models already beat experienced human professionals most of the time, though not yet large groups of top experts; the task length models can handle doubles roughly every 3.6 months, and a naive extrapolation puts them at a 50% success rate on 200-hour tasks by July 2027. METR cautions that this milestone rests on extrapolation, and that systems still struggle with open-ended questions lacking immediate feedback and with situations that are hard to recreate for training. The organization also warns that common, easy-to-run benchmarks may overestimate real-world performance because developers train models in environments very similar to the tests, potentially leaving humans unable to meaningfully understand, assess, and react to catastrophic risks from new AI systems.

rss · The Decoder · Nov 22, 13:00

**「METR&\#x27;s time-horizon benchmark」** METR measures AI capability by &quot;time horizon&quot; — the length of tasks, expressed in skilled-human work time, that models can complete at a given reliability. Earlier METR work found the horizon doubling roughly every seven months, with signs of acceleration to around four months during 2024, and its Time Horizon 1.1 benchmark \(reported in a prior digest from January 2026\) put Claude Opus 4.6 at 14+ hours of expert work at 50% reliability. The current warning extends this line of research, citing a faster doubling of about 3.6 months on coding and computational tasks and extrapolating to 200-hour tasks by mid-2027.

**「Implication for builders」** Teams relying on standard benchmark scores to gauge model suitability should treat them as potentially inflated: METR&\#x27;s finding that models are trained in environments closely resembling common tests means easy-to-run evaluations may overstate real-world performance, so organizations should validate candidate models on task distributions and feedback structures that differ from public benchmark setups.

<details><summary>References</summary>
<ul>
<li><a href="https://metr.org/blog/2025-07-14-how-does-time-horizon-vary-across-domains/">How Does Time Horizon Vary Across Domains? - METR</a></li>
<li><a href="https://taibui.dev/phases/15-autonomous-systems/01-long-horizon-agents">The Shift from Chatbots to Long- Horizon Agents — Tai Bui</a></li>

</ul>
</details>

**Tags**: `#ai-safety`, `#evaluations`, `#METR`, `#capability-trends`, `#benchmarks`

---

<a id="item-ai-news-4"></a>
### [Anthropic mathematician with Claude claims proof of Navier–Stokes blow-up; human-only Riemann draft released same day](https://www.qbitai.com/2026/11/511870.html) ⭐️ 7.0/10

On November 20, Anthropic mathematician Levent Alpöge and NYU&\#x27;s Tristan Buckmaster released a 79-page paper claiming a proof of finite-time blow-up for the unforced 3D Navier–Stokes equations, covering both ordinary and periodic settings, together with Lean formalization code and a statement that the work used Claude exclusively among AI models. Terence Tao discussed the work, saying the overall strategy is clear—numerically finding a self-similar candidate flow, then proving nearby true solutions exist via rigorous perturbation theory—but that it still needs a formal professional write-up. Key verification gaps remain: the numerical certificates underpinning the construction and related checking computations are not included in the public release, and the patched Lean package had not yet been rebuilt, so the claim cannot be treated as independently verified. The same day, mathematician Alessandro Maria Masullo published a 940-page, ~12-year, AI-free draft proof of the generalized Riemann hypothesis, which within about 8 hours had already drawn reported problems from researchers using AI models; both claims await validation.

rss · 量子位 · Nov 22, 06:03

**「Background」** The Navier–Stokes existence and smoothness problem, one of the Clay Millennium Prize problems, asks whether solutions to the equations describing viscous fluid flow can develop singularities — unbounded velocity at a finite time — or always remain smooth. Prior to this claim, blow-up results had been shown for the inviscid Euler equations, including a September 2026 result by the same authors with smooth external forcing, but removing the forcing while retaining viscosity had remained open. The authors report that Claude was used throughout for proof generation, formalization-to-prose conversion via Scott Armstrong&\#x27;s tooling, and manuscript rewriting, following a workflow that began with Lean formalized code and produced the paper draft from it.

**「Why it matters」** The workflow described here—Lean formalization first, then automated conversion to natural-language proof text via Scott Armstrong&\#x27;s tooling, with Claude rewriting under human direction—signals a shift in how high-stakes mathematical results may be produced and checked, and how fast drafts reach the public before human verification or numerical certificates are complete. Teams relying on formal verification should note that &\#x27;paper plus Lean code released&\#x27; does not equal &\#x27;verified,&\#x27; and that pace pressure is now prompting human researchers \(like Masullo\) to release long-matured work earlier than they would prefer.

**Tags**: `#ai-for-math`, `#millennium-prize-problems`, `#navier-stokes`, `#riemann-hypothesis`, `#lean-formalization`, `#anthropic`, `#unverified-claims`

---

## Technology News

<a id="item-tech-news-1"></a>
### [派早报：Anthropic 研究员宣称用 Claude 证明黎曼猜想](https://sspai.com/post/119418) ⭐️ 8.0/10

AI 辅助的黎曼猜想形式化证明宣称获 Lean 社区核验通过，引发数学界审慎验证与讨论，同时另一份人类证明手稿被 AI 协助发现疑点。

rss · 少数派 · Nov 22, 23:34

**Tags**: `#人工智能`, `#黎曼猜想`, `#Lean 定理证明`, `#Anthropic`, `#形式化验证`

---

<a id="item-tech-news-2"></a>
### [OpenAI’s chief scientist has thoughts on how to limit AI development](https://techcrunch.com/2026/11/22/openais-chief-scientist-has-thoughts-on-how-to-limit-ai-development/) ⭐️ 7.0/10

OpenAI chief scientist Jakub Pachocki proposes using perplexity as a measurable basis for limiting the pace of AI development amid an industry debate on frontier AI safety standards.

rss · TechCrunch · Nov 22, 21:14

**Tags**: `#AI safety`, `#AI policy`, `#OpenAI`, `#frontier AI`, `#language models`

---

## Astronomy News

<a id="item-astronomy-news-1"></a>
### [Gap in 257 black hole mergers hints at failed supernovae](https://www.sciencedaily.com/releases/2026/11/261121221126.htm) ⭐️ 7.0/10

An analysis of 257 black hole mergers, drawn from gravitational-wave observations, identifies a gap in the mass distribution of black holes that suggests many massive stars collapse directly into black holes without producing supernova explosions. The reported pattern indicates the missing mass range corresponds to stars expected to explode, yet whose collapse may instead occur quietly. As a population-level statistical result, it is a candidate feature of the black hole population rather than a confirmed detection, and peer-review status of the analysis is not stated in the source. If confirmed, it would explain the origins of a substantial population of stellar-mass black holes across the universe.

rss · ScienceDaily Physics · Nov 22, 11:46

**「Why failed supernovae matter」** Conventional stellar-evolution models predict that stars roughly 8 to 25 times the Sun&\#x27;s mass end their lives as core-collapse supernovae, but the most massive stars are expected to be vulnerable to a different outcome: their cores grow so large that they collapse straight into black holes, sometimes leaving no luminous explosion at all. Astronomers have long sought observational evidence for these &quot;failed&quot; supernovae, such as surveys that catch massive stars vanishing without a flash. Gravitational-wave detections of black hole mergers offer a new, population-scale way to test this idea, because black holes that formed through direct collapse should carry imprints—such as low spins and a characteristic paucity of masses in a certain range—that differ from those born in successful explosions.

**「Constraints on supernova models」** The apparent gap provides a measurable constraint on stellar-evolution and supernova models, since the location and depth of the mass gap discriminate between scenarios in which massive stars explode and those in which they collapse directly, guiding how merger catalogs are interpreted in future population studies.

**Tags**: `#black holes`, `#gravitational waves`, `#failed supernovae`, `#direct collapse`, `#stellar evolution`

---

<a id="item-astronomy-news-2"></a>
### [BepiColombo went into orbit around Mercury yesterday\!](https://earthsky.org/space/bepicolombo-mission-mercury/) ⭐️ 7.0/10

BepiColombo has been confirmed by ESA flight dynamics to have achieved orbital capture around Mercury, with telemetry assessment ongoing.

rss · EarthSky · Nov 22, 08:30

**Tags**: `#BepiColombo`, `#Mercury`, `#ESA`, `#planetary science`, `#mission milestone`, `#orbital insertion`

---

<a id="item-astronomy-news-3"></a>
### [JWST finds a possible black hole that grew faster than its host galaxy in the early universe](https://phys.org/news/2026-11-jwst-black-hole-grew-faster.html) ⭐️ 6.0/10

A JWST observation suggests a possible early-universe black hole that grew faster than its host galaxy, bearing on how the first massive black holes formed.

rss · Phys.org Space · Nov 22, 16:40

**Tags**: `#jwst`, `#black holes`, `#early universe`, `#supermassive black holes`, `#candidate discovery`

---

<a id="item-astronomy-news-4"></a>
### [Milky Way simulation reaches record resolution with the help of three supercomputers](https://phys.org/news/2026-11-milky-simulation-resolution-supercomputers.html) ⭐️ 6.0/10

Researchers report a record-resolution Milky Way simulation reaching individual-star detail by combining multiple supercomputers with an AI-accelerated, hardware-flexible model to improve understanding of galactic evolution.

rss · Phys.org Space · Nov 22, 14:00

**Tags**: `#galactic simulation`, `#Milky Way`, `#computational astrophysics`, `#supercomputing`, `#galactic evolution`

---

## Energy News

<a id="item-energy-news-1"></a>
### [Ford Begins Producing Its Own LFP Batteries](https://cleantechnica.com/2026/11/21/ford-begins-producing-its-own-lfp-batteries/) ⭐️ 7.0/10

Ford has begun producing CATL-licensed LFP prismatic battery cells at its Michigan plant, reportedly at 40 cells per minute, marking its entry into in-house battery manufacturing.

rss · CleanTechnica · Nov 22, 04:49

**Tags**: `#EV batteries`, `#LFP`, `#Ford`, `#manufacturing`, `#battery production`, `#US supply chain`

---

## Oil and Gas Industry News

<a id="item-oil-gas-news-1"></a>
### [US Lends 8.5 Million Barrels of SPR Crude, Second Loan Since Iran War Began](https://news.google.com/rss/articles/CBMiowFBVV95cUxNX3BNZktJMXBqOEdWZnNwTVd0T3owc2Q1TGZ5YUN6bDh0NFVXWDJDRXpYekRvTHZueldCaDFvaXFVOFh5OHJoTDJib210ZU9JRjlxeW5pS1ZaZDJZbHN0Z1dvNWZsZEZyeUtNODV0NnR6TVlTR0lwVThEM19LYzl0RkF4MnowOHpjNzdEQ3E0UEl4Tl9jTVptbld1NWlQc2x2RHFN?oc=5) ⭐️ 6.0/10

The United States is lending 8.5 million barrels of crude oil from the Strategic Petroleum Reserve, according to EnergyNow.com. This is the second such SPR loan batch issued since the war involving Iran began. The loan provides crude to borrowers on a temporary basis, with volumes expected to be returned to the reserve. Details on the borrowers, exchange terms, and return timeline were not provided in the source item.

rss · Google News Oil &amp; Gas \(EN\) · Nov 22, 16:25

**「Context」** The US Strategic Petroleum Reserve is the government&\#x27;s emergency crude oil stockpile, and exchange or loan agreements allow refiners to borrow crude on a temporary basis, typically to be returned with interest. According to the source, this 8.5 million barrel loan is the second such release since the war involving Iran began, indicating the reserve has been drawn on repeatedly as a stopgap during the conflict. The exact repayment terms and the recipients of the crude are not detailed in the supplied source.

**「Why it matters」** SPR loans temporarily increase crude supply available to refiners or traders during a supply disruption, but the modest 8.5-million-barrel volume is small relative to global consumption, so the action signals official concern about availability tied to the Iran conflict rather than materially changing market balances. Repeated loans also draw down the reserve&\#x27;s immediately available inventory until the barrels are returned.

**Tags**: `#SPR`, `#United States`, `#oil policy`, `#Iran`, `#crude loans`

---

## Literature News

<a id="item-literature-news-1"></a>
### [Jilly Cooper&\#x27;s Prudence faces plagiarism allegations](https://www.theguardian.com/books/2026/nov/22/rivals-author-jilly-cooper-accused-plagiarism) ⭐️ 6.0/10

The Guardian reports that the late bestselling author Jilly Cooper has been accused of plagiarising two other novelists in Prudence, her fifth romance series novel, published in 1978. An analysis cited in the report alleges the novel includes several plagiarised passages from Cyra McFadden&\#x27;s The Serial and Josephine Tey&\#x27;s The Franchise Affair, with claimed similarities in dialogue and narrative structure. The allegations remain unverified claims reported by the newspaper rather than a legal or scholarly finding.

rss · Guardian Books · Nov 22, 15:07

**「Context」** Jilly Cooper, who died in 2025, was one of Britain&\#x27;s bestselling popular novelists, best known for the Rutshire Chronicles including Riders and Rivals, which was adapted into a Disney+ television series in 2024. The allegations concern Prudence, a 1978 novel from early in her career, which the reported analysis says drew passages from Cyra McFadden&\#x27;s The Serial and Josephine Tey&\#x27;s The Franchise Affair. Because the claims rest on a newly reported textual analysis rather than a court ruling or publisher statement, they remain unverified allegations.

**「Impact」** Because the allegations concern a specific novel with named source texts, they may prompt renewed scrutiny of Prudence&\#x27;s text by publishers, scholars, or rights holders, potentially affecting the book&\#x27;s handling in new editions and translations.

**Tags**: `#plagiarism`, `#Jilly Cooper`, `#literary controversy`, `#publishing`, `#Guardian`

---

<a id="item-literature-news-2"></a>
### [Review: Nancy Isenberg&\#x27;s &\#x27;Aristocracy, American Style&\#x27;](https://www.nytimes.com/2026/11/22/books/review/aristocracy-american-style-nancy-isenberg.html) ⭐️ 6.0/10

In the New York Times Book Review dated November 22, 2026, Alexandra Jacobs reviews Nancy Isenberg&\#x27;s new book &quot;Aristocracy, American Style.&quot; The review examines Isenberg&\#x27;s critique of how the ideal of equality is marketed to people who, in practice, are left with &quot;the short end of the stick.&quot; Isenberg, a historian known for work on American social hierarchy, uses the book to argue that aristocratic class structures have persisted beneath the country&\#x27;s egalitarian rhetoric.

rss · New York Times Books · Nov 22, 10:00

**「Context」** Nancy Isenberg is an American historian known for books that examine class and hierarchy in the United States, including &\#x27;White Trash: The 400-Year Untold History of Class in America,&\#x27; which argued that a white underclass has been central to the nation&\#x27;s history despite myths of egalitarianism. The new book extends that line of inquiry, arguing that American equality functions as a marketing pitch to those it fails, a framing Alexandra Jacobs&\#x27;s New York Times review takes up. Isenberg&\#x27;s established profile as a prominent scholar of American social hierarchy makes the review substantive coverage of a notable publication.

**Tags**: `#book review`, `#American history`, `#Nancy Isenberg`, `#New York Times`, `#inequality`

---

<a id="item-literature-news-3"></a>
### [Huw Green Explains How Psychosomatic Illnesses Arise](https://www.theguardian.com/science/2026/nov/22/how-can-we-explain-psychosomatic-illnesses) ⭐️ 5.0/10

The Guardian published an essay by Huw Green on 22 November 2026 explaining psychosomatic illness, arguing that emotions and psychological health can contribute to real, debilitating physical symptoms without any underlying disease or damage. Green builds the explanation around the case of Diego, whose flashing lights and leg weakness initially suggested a stroke but persisted after scans ruled one out. The essay&\#x27;s thesis is that such symptoms arise when the coordinated functioning of the body goes awry, with psychological health an important element in a percentage of cases.

rss · Guardian Books · Nov 22, 12:00

**「Background」** Huw Green writes for The Guardian, where this essay appeared in the publication&\#x27;s science section on 22 November 2026. The piece belongs to a tradition of explanatory science journalism that addresses how psychological states can produce genuine physical symptoms, using an illustrative patient case rather than reporting on a new study or publication.

**Tags**: `#science essay`, `#psychosomatic illness`, `#health`, `#Guardian`, `#explanatory journalism`

---

<a id="item-literature-news-4"></a>
### [A.O. Scott Reads Yeats&\#x27;s &\#x27;The Lake Isle of Innisfree&\#x27; in New NYT Video Essay](https://www.nytimes.com/video/books/review/100000011132055/this-poem-is-a-three-minute-vacation.html) ⭐️ 5.0/10

The New York Times has published a short video essay in which critic at large A.O. Scott discusses William Butler Yeats&\#x27;s poem &quot;The Lake Isle of Innisfree.&quot; The piece, produced by Léo Hamelin, Laura Salaberry, Efim Shapiro, and Adrienne Jeffries, focuses on how the poem&\#x27;s third stanza reframes its imagined retreat from modern life. Scott emphasizes that although the speaker dreams of an island refuge, he remains standing on &quot;a gray pavement,&quot; and that this final turn changes how the whole poem reads.

rss · New York Times Books · Nov 22, 20:24

**「Context」** &quot;The Lake Isle of Innisfree,&quot; first published in 1890, is one of Yeats&\#x27;s most anthologized poems and a staple of the canon, making it familiar territory for accessible critical features. Scott, a longtime Times film critic who now serves as critic at large, has increasingly worked in formats that bring close reading to a general audience. The video belongs to the Times Books video series rather than reporting a new publication or prize.

**Tags**: `#poetry`, `#Yeats`, `#criticism`, `#video essay`, `#New York Times`

---

<a id="item-literature-news-5"></a>
### [Married Couple&\#x27;s Murder-Mystery Puzzle Book Sells 100,000 Copies](https://www.nytimes.com/2026/11/22/books/review/the-killer-isnt-alice-puzzle-book.html) ⭐️ 4.0/10

A New York Times Book Review feature by Elisabeth Egan, published November 22, 2026, profiles a married couple who invented the murder-mystery puzzle book &\#x27;The Killer Isn&\#x27;t Alice.&\#x27; Escape-room enthusiasts, the couple designed the challenge themselves, and it has now sold more than 100,000 copies. The piece frames the book&\#x27;s popularity as a life-changing success for its creators.

rss · New York Times Books · Nov 22, 14:45

**「Context」** The book sits at the intersection of two trends: escape rooms and interactive puzzle books, formats that invite readers to solve a mystery rather than simply read one. The creators&\#x27; background as escape-room fanatics informed the book&\#x27;s design, and its sales milestone places it among notable independently conceived puzzle successes. The feature is a human-interest profile rather than news of an award or industry shift.

**Tags**: `#puzzle books`, `#publishing success story`, `#human interest`, `#murder mystery`

---

<a id="item-literature-news-6"></a>
### [Misty Copeland Reviews Lynn Garafola&\#x27;s Biography of Arthur Mitchell](https://www.nytimes.com/2026/11/22/books/review/arthur-mitchell-lynn-garafola.html) ⭐️ 4.0/10

The New York Times Book Review has published Misty Copeland&\#x27;s review of Lynn Garafola&\#x27;s new biography of Arthur Mitchell, the dancer and choreographer who was a powerful force at both New York City Ballet and Dance Theater of Harlem. Copeland, herself a celebrated ballet dancer, calls the book incisive in her assessment. The review appeared in the November 22, 2026 issue.

rss · New York Times Books · Nov 22, 10:00

**「Context」** Arthur Mitchell was a pioneering figure in American dance, breaking barriers at New York City Ballet before founding Dance Theater of Harlem, and Lynn Garafola&\#x27;s new biography examines his influence at both institutions. The review carries additional resonance because its author, Misty Copeland, is herself a celebrated dancer whose career follows in the tradition Mitchell helped open to Black artists. Dance Theater of Harlem remains the institution most closely identified with his legacy.

**Tags**: `#book review`, `#biography`, `#dance`, `#Arthur Mitchell`, `#Misty Copeland`

---

<a id="item-literature-news-7"></a>
### [NYT Book Review Editor Picks Three Books Ahead of December Screen Adaptations](https://www.nytimes.com/video/books/100000011268506/read-these-books-before-they-hit-screens-in-december.html) ⭐️ 4.0/10

Jennifer Harlan, an editor at The New York Times Book Review, presents a video recommending three books to read before their on-screen adaptations premiere in December. The item is promotional rather than argumentative: it does not name the three titles or the adaptations in the available material. It was produced by Harlan along with Karen Hanley, Paige Money, and Edward Vega, and published on November 22, 2026.

rss · New York Times Books · Nov 22, 19:38

**「Background」** The recommendation comes from Jennifer Harlan, an editor at The New York Times Book Review, which regularly covers the intersection of books and their screen adaptations. The video format highlights titles in the weeks before their December premieres, reflecting the Book Review&\#x27;s practice of guiding readers toward source material ahead of adaptation releases.

**Tags**: `#book-to-screen adaptations`, `#recommendations`, `#video`, `#New York Times`

---