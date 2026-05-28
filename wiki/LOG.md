# Operation Log

*Every ingest and update operation is recorded here.*

---

## 2026-05-24 — Vault Initialized

- **Operation:** INIT
- **Source:** System
- **Pages Created:** CLAUDE.md, wiki/INDEX.md, wiki/LOG.md, raw/README.md
- **Notes:** Vault structure created. Folders: /raw, /wiki/brands, /wiki/scripts, /wiki/ideas, /wiki/campaigns, /wiki/strategies, /wiki/concepts

---

## 2026-05-24 — Bulk Transcript Fetch (40 videos)

- **Operation:** FETCH
- **Tool:** fetch_transcripts.py (youtube-transcript-api v1.2.4)
- **Source:** 40 YouTube URLs (manually provided)
- **Result:** 40/40 transcripts saved to /raw
- **Total segments fetched:** ~31,600 across all 40 files
- **Files saved to /raw:**

| # | Video ID | Title |
|---|----------|-------|
| 1 | up2BLatM1EY | Boy Internet vs Girl Internet |
| 2 | 8MzPLXbNOeQ | What exactly is the "taste economy"? |
| 3 | vHaJu1ExBdg | How to make more money as a creative (offers playbook) |
| 4 | tcqf6sgw_Ho | Once You Master Brand Archetypes, You Master Social Media |
| 5 | CS0A4hJfcy4 | The Art of Yapping (full guide to talking on video) |
| 6 | l3inbx2jeZU | What ACTUALLY Makes People Buy Things (Pricing Psychology) |
| 7 | bpjukyNSjpw | The Branding of Hailey & Justin Bieber |
| 8 | aHNphtjvdhA | Why every product sucks now (enshittification) |
| 9 | Q6m5-kYTcfM | What japan understands about branding no one else does |
| 10 | IdmtqdoZTBA | How to build a marketing team in 2026 (content operations) |
| 11 | QAjjOOMgqCs | The internet is splintering (2026 social trends playbook) |
| 12 | pnbR4RecdLA | How tech uses branding to get you to buy (Apple case study) |
| 13 | 1YVi3iFk3V0 | How to Make a Marketing Plan (2026 Playbook) |
| 14 | 8gvCc5jvcH0 | I've made 1067 short form videos, here's what actually makes money |
| 15 | OSx7YsvnQHw | The Psychology of Luxury |
| 16 | ZzsoouA3FWU | The Rebrand That Saved Bad Bunny |
| 17 | QHPmOgnc96E | 11 ways to get your life together in 2026 (systems for creatives) |
| 18 | gFyvRbkTGZg | The Creative Direction of Sports |
| 19 | kFfN_t3bH_8 | How to get ahead of 99% of brands in 2026 (content playbook) |
| 20 | C9epWGO8VA4 | How to transform your life in 2026 (as a creative) |
| 21 | qifGvtE31N4 | Developing taste is easy, actually |
| 22 | OqxedKwmbYc | The creative director playbook for brands (Ralph Lauren) |
| 23 | LI2qf34jy8k | The Art of the Marketing Campaign (full masterclass) |
| 24 | tSopiLVEreM | The Marketers Guide to AI (full workflows) |
| 25 | jM10LqMwaXY | The Aesthetic Playbook of K-Pop & Korean Fashion |
| 26 | Q4-rF3kQsvc | The downfall of old luxury (2026 premium brand playbook) |
| 27 | C1K5E--EHhM | The dark psychology of creative people |
| 28 | Li-M7A7-plk | The 2026 brand content cheat codes (viral content playbook) |
| 29 | c936_pCbgxQ | The Worst Marketing of 2025 |
| 30 | qviOuXlHYG0 | The Moment Virgil Abloh Became the GOAT |
| 31 | dSyHnvWlAFI | The Art Direction of Quiet Luxury |
| 32 | 13jzjINwFQ0 | Read these books to master branding and marketing |
| 33 | HP_6MJAdILY | The Rise and Fall of Supreme (brand strategy case study) |
| 34 | pKeZ5XK2vp4 | How to start brand social media from scratch in 2026 |
| 35 | zeHkJuMORJE | Marketing is about to change forever (and no one is noticing) |
| 36 | ljEn99Cr9GA | The Art of Spectacle (Balenciaga Case Study) |
| 37 | UBDpGwdkiz4 | The 7 Levels of Brand Building |
| 38 | 1CRdDMK1uIQ | A guide to new and vintage cameras for creatives |
| 39 | qa13iuKa8zA | The Creative's Guide to Personal Branding (Full Playbook) |
| 40 | kl4DLGKK_VI | How to Make Money as a Creative in 2026 |

---

## 2026-05-24 — Bulk Wiki Build (40 transcripts → 74 pages)

- **Operation:** INGEST (bulk)
- **Source files:** All 40 transcripts in /raw
- **Method:** 4 parallel agents, each processing 10 transcripts
- **Total pages created:** 74

### Pages Created

**Brands (7)**
- wiki/brands/Apple.md
- wiki/brands/BadBunny.md
- wiki/brands/Balenciaga.md
- wiki/brands/HaileyBieberRhode.md
- wiki/brands/RalphLauren.md
- wiki/brands/Supreme.md
- wiki/brands/VirgilAblohOffWhite.md

**Concepts (24)**
- wiki/concepts/ai-in-marketing.md
- wiki/concepts/art-direction-as-brand-strategy.md
- wiki/concepts/boy-internet-vs-girl-internet.md
- wiki/concepts/brand-archetypes.md
- wiki/concepts/camera-aesthetics-for-creatives.md
- wiki/concepts/content-virality-mechanics.md
- wiki/concepts/creator-economy-in-2026.md
- wiki/concepts/dark-psychology-of-creatives.md
- wiki/concepts/enshittification.md
- wiki/concepts/how-to-develop-taste.md
- wiki/concepts/internet-splintering.md
- wiki/concepts/japanese-branding-philosophy.md
- wiki/concepts/k-pop-aesthetic-playbook.md
- wiki/concepts/pricing-psychology.md
- wiki/concepts/psychology-of-luxury.md
- wiki/concepts/quiet-luxury.md
- wiki/concepts/spectacle-marketing.md
- wiki/concepts/sports-creative-direction.md
- wiki/concepts/streetwear-brand-strategy.md
- wiki/concepts/the-downfall-of-old-luxury.md
- wiki/concepts/the-future-of-marketing.md
- wiki/concepts/the-rebrand-playbook.md
- wiki/concepts/the-taste-economy.md
- wiki/concepts/worst-marketing-patterns.md

**Strategies (19)**
- wiki/strategies/2026-content-playbook.md
- wiki/strategies/7-levels-of-brand-building.md
- wiki/strategies/aesthetic-led-brand-strategy.md
- wiki/strategies/ai-workflows-for-marketers.md
- wiki/strategies/brand-social-media-from-scratch.md
- wiki/strategies/content-operations-playbook.md
- wiki/strategies/creative-director-approach-to-brand-building.md
- wiki/strategies/creative-offers-playbook.md
- wiki/strategies/luxury-brand-positioning-strategy.md
- wiki/strategies/making-money-as-a-creative-2026.md
- wiki/strategies/marketing-campaign-masterclass.md
- wiki/strategies/marketing-plan-framework-2026.md
- wiki/strategies/new-luxury-premium-brand-strategy.md
- wiki/strategies/on-camera-presence.md
- wiki/strategies/personal-branding-full-playbook.md
- wiki/strategies/personal-rebrand-playbook.md
- wiki/strategies/short-form-video-that-makes-money.md
- wiki/strategies/systems-for-creatives.md
- wiki/strategies/viral-content-playbook.md

**Ideas (23)**
- wiki/ideas/idea-adversarial-review-pre-launch.md
- wiki/ideas/idea-catalog-your-expertise-ranking-video.md
- wiki/ideas/idea-clipping-ecosystem-for-brands.md
- wiki/ideas/idea-indie-brand-founder-vlog.md
- wiki/ideas/idea-monoculture-moment-campaign.md
- wiki/ideas/idea-oracle-archetype-expert-rankings.md
- wiki/ideas/idea-spectacle-pr-kit-unboxing.md
- wiki/ideas/idea-world-builder-fictional-brand-series.md
- wiki/ideas/reel-idea-brand-second-brain-reveal.md
- wiki/ideas/reel-idea-competitor-analysis-tiktok.md
- wiki/ideas/reel-idea-content-format-versus.md
- wiki/ideas/reel-idea-content-pillar-breakdown.md
- wiki/ideas/reel-idea-identity-change-process.md
- wiki/ideas/reel-idea-niche-history-deep-dive.md
- wiki/ideas/reel-idea-offer-structure-breakdown.md
- wiki/ideas/reel-idea-system-reveal.md
- wiki/ideas/reel-idea-year-type-decision.md
- wiki/ideas/steal-the-k-pop-reference-method.md
- wiki/ideas/the-halo-product-secret.md
- wiki/ideas/the-quantified-man-sell.md
- wiki/ideas/two-internets-one-brand.md
- wiki/ideas/what-stage-is-your-brand-really-at.md
- wiki/ideas/why-your-price-is-killing-your-brand.md

**Reference (1)**
- wiki/reference/recommended-books.md

---

## 2026-05-25 — Wiki Expansion Pass (40 transcripts re-analyzed → 98 pages)

- **Operation:** EXPAND
- **Source files:** All 40 transcripts in /raw (re-analyzed with broader lens)
- **Method:** 3 parallel agents, each extracting a different category cluster
- **Previous total:** 74 pages
- **New total:** 98 pages (+24 new pages)

### Why This Expansion Happened

Original ingest focused heavily on marketing, reel strategy, and brand analysis. The expansion pass re-read the same 40 transcripts to extract content that was present but not captured: creative psychology, identity and mindset frameworks, business models, aesthetics and visual craft, cultural analysis, collaboration dynamics, and intellectual development. The vault scope expanded from "marketing knowledge base" to a full creative and brand-building knowledge base.

### New Concept Pages Created (15)

- wiki/concepts/communication-as-a-life-skill.md — Four questions of communicating well; idea-workshopping loop; why content-making sharpens all communication
- wiki/concepts/creative-self-sabotage.md — Six named patterns (Ceiling Collapse, Justified Distraction, Inaction Loop, Stolen Idea Trap, Taste Masquerade, Organic Discovery Trap)
- wiki/concepts/group-think-in-creative-industries.md — Three-phase enforcement mechanism; four named patterns; AI-in-creative-work case study
- wiki/concepts/identity-and-creative-work.md — Identity as predictive model; five-step deliberate change mechanism; Identity Ceiling, Frozen Self, Comfort-Group Anchor patterns
- wiki/concepts/the-taste-paradox.md — Why taste develops faster than skill; Quality Excuse, Organic Recognition Fantasy, Gatekeeping Trap, Comparison Spiral traps
- wiki/concepts/value-and-pricing-philosophy.md — Agency extraction model; "selling out" conditioning; salary anchor problem; TikTok Shop ROI quantification
- wiki/concepts/offer-architecture.md — "I do X for Y at Z" formula; three differentiators; offer stacking; two-tier pricing; VSL layer
- wiki/concepts/taste-as-a-learnable-skill.md — Five-phase development path; critique matrix (composition/effectivity/vibes); design periods to study
- wiki/concepts/visual-craft-philosophy.md — What each camera format communicates; lens choices as aesthetic signature; full toolkit map
- wiki/concepts/lessons-from-1000-hours-of-content.md — Ten meta-lessons from 1,067 videos; volume as teacher; three-level creator framework
- wiki/concepts/subculture-to-mainstream-pipeline.md — Five-stage model: founding community → gatekeeper networks → crossover moment → institutional absorption → echo phase
- wiki/concepts/creative-collective-dynamics.md — How collectives form and amplify; Been Trill, Supreme, K-pop, Japanese brand ecosystems
- wiki/concepts/japan-as-a-creative-philosophy.md — Imitation-to-surpassing dynamic; Muji restraint as confidence; curation as original practice; craft-as-identity
- wiki/concepts/legacy-and-creative-impact.md — Virgil's Free Game philosophy; documentation as legacy infrastructure; iconography as residue; ripple effects
- wiki/concepts/the-reading-mind-for-creatives.md — Full learning philosophy; 25+ named books by category with author, what each teaches, and application context

### New Strategy Pages Created (9)

- wiki/strategies/identity-change-framework.md — Six-stage process; five year-types; archetype-building with behavioral specificity; pause technique; 52-week requirement
- wiki/strategies/life-systems-for-creatives.md — All 11 systems with implementation detail: reference repo, ideas list, phone content folders, weekly update, team tracker, process docs, calendar ritual, and more
- wiki/strategies/on-camera-confidence-framework.md — Seven-phase framework; Yap Map (five sources); five content structures; Recut Method; eye-contact rule; three graphic overlay levels
- wiki/strategies/creative-business-models-2026.md — Full economic map; all 7 monetization models with economics and ceilings; best stacks and trap stacks
- wiki/strategies/offer-design-for-creatives.md — Eight-step operational framework: deliverable → competitive position → offer page → VSL → two-tier pricing → funnel → public pricing
- wiki/strategies/developing-a-visual-point-of-view.md — Six-phase process: reference library → forming opinions → format/tool choices → public testing → thrift-store exercise → compounding over time
- wiki/strategies/building-creative-collectives.md — Six-phase operational playbook: finding the room → qualifying on obsession → gravitational centers → first breakout → formalizing sharing norms → tending the network
- wiki/strategies/cross-cultural-creative-borrowing.md — Five-step framework; deep vs. surface borrowing; PAF left/center/right spectrum methodology
- wiki/strategies/intellectual-development-for-creatives.md — Five-level structured approach: sustainable reading practice → diverse category diet → applying reading → physical reference library → contrarian reading

### INDEX.md Updated

- Stats updated: 39 concepts, 28 strategies, 98 total pages
- New concept subcategories added: Creative Psychology & Identity, Business & Creative Economics, Cultural Analysis
- New strategy subcategories added: Creative Systems & Productivity, Business & Monetization, Visual Development, Culture & Collaboration

### Google Drive Synced

All 24 new pages + updated INDEX uploaded to Drive. New INDEX Drive ID: 1gXv1L_bNWcP9gzDt-Z105J9Pksnv8dM8BmJbiVf8LoI

---

---

## 2026-05-25 — Ingest: Dan Martell AI Cheat Codes Video

- **Operation:** INGEST
- **Source:** YouTube — Dan Martell, "The AI Cheat Codes Every Founder Needs in 2026" (https://www.youtube.com/watch?v=_24HzGNv-3A)
- **Previous total:** 122 pages
- **New total:** 129 pages (+7 new pages)

### Pages Created (7)

**Concepts (3)**
- wiki/concepts/ai-operating-system-for-founders.md — Core philosophy: AI as operating layer not bolt-on; 17 companies / 1-person finance team; three principles (augment, validate-first, architecture-as-advantage)
- wiki/concepts/three-levels-of-ai.md — 4-tier maturity model: Personal leverage → Team leverage → Compounding leverage → Scalable leverage; 95% stuck at Level 1; diagnostic checklist
- wiki/concepts/ai-mistakes-founders-make.md — 15 named mistakes with structural fixes; three meta-patterns: role confusion, sequence failure, architecture failure; context rot and context fraud defined

**Strategies (3)**
- wiki/strategies/master-prompt-architecture.md — Full 4-tier system: master prompt build process, 7 keywords (Act as/Deep research/First principles/Devil's advocate/Constraints first/Format as/Verify and cite), system prompt creation loop, reverse prompt framework, sequencing principle
- wiki/strategies/ai-tool-stack-for-founders.md — Tool-to-use-case matching: ChatGPT for creativity, Claude for quality, Gemini for research, Perplexity for citations; 8-tool ranked stack; tool selection rule
- wiki/strategies/zero-inbox-system.md — 4-layer system: sorting/prioritization, draft generation, autonomous responses, meeting prep; prerequisites; APEX integration

**Reference (1)**
- wiki/reference/apex-platform.md — Dan Martell's autonomous agent platform: email/scheduling/content/research/software; private servers; multi-agent orchestration; context memory; apex.host waitlist

### INDEX.md Updated

- Stats: 48 concepts, 35 strategies, 7 reference pages, 129 total pages
- New concept subcategory added: "AI & Founders"
- New strategy subcategory added: "AI Systems & Automation"

---

---

## 2026-05-25 — Ingest: Orin John — Open Residency / Viral Content Masterclass

- **Operation:** INGEST
- **Source:** YouTube — Open Residency, "The Most Valuable Marketing Conversation You'll Watch in 2025" ft. Orin John (https://www.youtube.com/watch?v=uI5Qo58FqiE); supplemented by Orin John Viral Content Masterclass (Motion Creative Analytics)
- **Previous total:** 129 pages
- **New total:** 136 pages (+7 new pages)

### Pages Created (7)

**Concepts (4)**
- wiki/concepts/messages-concepts-hooks-framework.md — Three-pillar content system: messages (value props/stories/trends), concepts (10 execution formats), hooks (familiar faces/call-outs/visual uniqueness/poke-in-pool); modular and testable; matrix approach to content calendars
- wiki/concepts/owned-enabled-paid-media-ecosystem.md — Owned (brand accounts) + Enabled (creators/affiliates/employees/fans) + Paid (ads); enabled tier is most underinvested; organic-to-paid pipeline; scale benchmarks (Grünz: 500+ creators, 1,500+ UGC/month)
- wiki/concepts/creator-first-brand-strategy.md — Making creators the primary content engine; all scaling brands have creator-first infrastructure; brand perception reality check (search brand on TikTok — organic already 100:1); "divorce personal taste" principle
- wiki/concepts/tiktok-shop-affiliate-model.md — Commission-based creator commerce; $500M+ Black Friday 2025; creator earnings by tier ($1,500–$25K/mo); once-in-a-lifetime 12-month window; product types that convert; 30-day entry playbook

**Strategies (3)**
- wiki/strategies/viral-organic-content-formats.md — Full taxonomy: 10 formats (yapping with 5 sub-formats, rankings, definitive cultural statements, credible explainers, unpopular opinions, provocative scenarios, transformation, testimonials, tutorials, reaction videos); format-by-goal matrix; industry examples
- wiki/strategies/affiliate-creator-program-strategy.md — Three phases (0→10→100→scale); sourcing from customer base; Discord/WhatsApp communities; Social Snowball/SuperAffiliate tools; organic-to-paid pipeline ($100–400 rights purchase); team structure; scale benchmarks table
- wiki/strategies/creative-strategist-system.md — Notion content database (5 fields); weekly 30-min hook-saving ritual; monthly brand checklist template; persona-based segmentation; 5 human emotion frames (love/spirituality/money/physical health/mental health); tools list

### INDEX.md Updated

- Stats: 52 concepts, 38 strategies, 136 total pages
- New concept section entries added: Creator Systems & Platform Intelligence (4 new)
- New strategy subcategory added: "Creator & Content Operations" (3 new pages)

---

---

## 2026-05-25 — Ingest: Taylor Holiday — 2026 E-Commerce Masterclass (Open Residency)

- **Operation:** INGEST
- **Source:** YouTube — Open Residency, "The 2026 E-Commerce Masterclass That Will Make You Question Everything" ft. Taylor Holiday (https://www.youtube.com/watch?v=RHJSO4eVJVA), 2h41m; supplemented by commonthreadco.com blog posts, Prophit System page, DTC Index, and podcast episodes
- **Speaker:** Taylor Holiday, CEO Common Thread Collective; sold CTC to private equity; Prophit System forecasts $3B+ in DTC revenue within 4% accuracy
- **Previous total:** 136 pages
- **New total:** 144 pages (+8 new pages)

### Pages Created (8)

**Concepts (6)**
- wiki/concepts/prophit-system.md — Financial forecasting infrastructure: 4 data models (Spending Power/Retention/Event Effect/Creative Demand), 3 forecast scenarios (Board/Budget/Bonus), Creative Demand Score (5 inputs: zero spend rate, ad concentration, ROAS degradation, spend degradation, evergreen share); "forecast belongs in marketing, not finance"; Statlas platform
- wiki/concepts/four-quarter-accounting.md — P&L diagnostic framework: 4 × 25% buckets (CAC/COD/OPEX/Profit); reference point not rule; identifies which quarter is over-indexed; first-order profitability standard for 2026; growth formula (V × CR × CM - VC = Profit)
- wiki/concepts/hierarchy-of-metrics-dtc.md — 4-tier KPI pyramid: Tier 1 = Contribution Margin, Tier 2 = Business (MER/AOV/Revenue), Tier 3 = New Customers (CAC/Repeat Rate), Tier 4 = Platform (ROAS/CPM); MER trap explained; platform metrics are information not decisions
- wiki/concepts/flow-era-and-constraint.md — 2026 DTC operating philosophy: constraint as competitive advantage; anti-fragile business benchmarks (OPEX <25%, margin >70%, 50/50 paid:organic); why 9-figure playbooks break 7-figure brands; marketer vs. allocator of capital distinction; CTC fired 100 people in 2022 as origin story
- wiki/concepts/product-architecture-framework.md — SKU categorization system: Champions/Growth Drivers/Underperformers/Hidden Gems; product expansion errors; brand = LTV not product loyalty; 30/100 benchmark (30% LTV lift in 60 days, 100% in a year); Bambu Earth cross-category purchase example; SKU rationalization triggers
- wiki/concepts/shrinking-sponge-problem.md — Active customer file decay: how retention focus without acquisition hollows the business; 5 customer segments (New/Continuing Active/Reactivated/Lapsed/Churned); MER trap as disguise; 4-step recovery (Four Quarter Accounting → Squeeze Sponge → Restart Engine → Track Segments); integrated finance-marketing requirement

**Strategies (2)**
- wiki/strategies/creative-demand-planning.md — Ad creative as supply chain: Creative Demand Score mechanics, 3.5% of ads drive 66% of spend, 150–400+ ads/month reality, iteration over breakthrough, creative-to-paid pipeline (continuous refresh not batch), volume benchmarks by stage, tools (Motion Creative Analytics)
- wiki/strategies/dtc-allocator-of-capital.md — Integrated DTC operating framework: marketer → allocator of capital identity shift; all frameworks connected (Four Quarter → Hierarchy → Prophit → Creative Demand → Product Architecture → Sponge → Flow Era); capital allocation decision tree; contribution margin daily tracking; survival vs. growth mode postures; pre-growth mode benchmarks

### INDEX.md Updated

- Stats: 58 concepts, 40 strategies, 144 total pages
- New concept subcategory added: "DTC & E-Commerce" (6 new pages)
- New strategy subcategory added: "DTC & E-Commerce" (2 new pages)

---

---

## 2026-05-25 — Ingest: Peter Rahal — David Protein / Open Residency

- **Operation:** INGEST
- **Source:** YouTube — Open Residency, "He Built a $725 Million Company in 255 Days. Here's What You're Doing Wrong" ft. Peter Rahal (https://www.youtube.com/watch?v=0OdHGliowm4); supplemented by commonthreadco.com, nosh.com, 20VC interview, and David Protein launch analysis
- **Speaker:** Peter Rahal, Co-Founder & CEO David Protein; former Co-Founder RXBAR ($600M Kellogg acquisition 2017); $85M+ raised; $725M valuation in 255 days; 3,000+ retail locations in 8 months
- **Previous total:** 144 pages
- **New total:** 149 pages (+5 new pages)

### Pages Created (5)

**Brands (1)**
- wiki/brands/David.md — David Protein brand page: 28g protein / 150 cal / 0g sugar specs; brand brief ("Don't overeat calories, get adequate protein, don't spike blood sugar"); anti-marketing tone; science-over-trends positioning; Dr. Attia/Huberman credibility; launch playbook; do's/don'ts

**Concepts (2)**
- wiki/concepts/consumer-surplus-framework.md — Core organizing principle: gap between willingness-to-pay and actual price; RXBAR ($600M) and David ($725M) both built on this; the competitive surplus test (4 questions); designing surplus in; why product creates organic advocacy; trial-to-repeat rate as the real signal
- wiki/concepts/product-first-brand-building.md — Contrarian philosophy: product > marketing; 3 pillars (Product/People/Distribution); why early marketing kills product development; RXBAR vs. David strategic opposition table; "obvious but true" brand philosophy; paleo trap pattern; dyslexia as contrarian advantage

**Strategies (2)**
- wiki/strategies/grassroots-distribution-strategy.md — 3-phase model: Phase 1 community penetration (CrossFit door-to-door), Phase 2 regional founder-led expansion, Phase 3 mainstream retail (Trader Joe's/Whole Foods); David's digital adaptation (giveaway + TikTok → retail); why sequence is non-negotiable; applying the framework
- wiki/strategies/product-launch-seeding-model.md — David's 5-component launch stack: 20K-unit giveaway + email list build, strategic influencer seeding (Attia/Huberman ecosystem), minimal owned content, UGC amplification ("let it speak for itself"), organic social virality (100K–200K+ views per video); 3 conditions required; adapted framework for non-CPG products

### INDEX.md Updated

- Stats: 8 brands, 60 concepts, 42 strategies, 149 total pages
- New brand added: David
- New concept subcategory added: "Product & Launch Strategy" (2 new pages)
- New strategy subcategory added: "Product & Launch" (2 new pages)

---

---

## 2026-05-27 — Ingest: Callaway — Short-Form Content Masterclass (Open Residency)

- **Operation:** INGEST
- **Source:** YouTube — Open Residency, ft. Callaway (https://www.youtube.com/watch?v=VcqQmrGqthg) — full transcript, 4,884 segments, ~36,000 words
- **Speaker:** Callaway — systems-first content strategist, reverse-engineer of viral short-form content; creator of Content.game newsletter, Sandcastles scripting software, Shortform.academy
- **Method:** Full transcript fetched → 25 chunk-by-chunk analysis files written (1,000 words each) → wiki pages extracted from all 25 chunks
- **Previous total:** 149 pages
- **New total:** 164 pages (+15 new pages)

### Pages Created (15)

**Brands (1)**
- wiki/brands/Callaway.md — Systems-first content strategist; reverse-engineers viral content; 7 Lego Bricks + 5 Content Games + Shock Score frameworks; full product ecosystem (Content.game, Sandcastles, Shortform.academy); 16 linked frameworks; do's/don'ts

**Concepts (9)**
- wiki/concepts/three-part-hook-framework.md — Visual hook + text hook + spoken hook must align; confusion=churn; contrast as scroll-stopper; context-first top-down brain processing; thumb stopper; visual set as strategic asset; direct vs. implied contrast math
- wiki/concepts/absorption-rate-framework.md — Absorption rate as master KPI; Content Minutes trust math (offer price requires X content minutes consumed); 20:1 short-form vs. long-form block ratio; bingeability mechanics; thumbnail covers as viral K-factor
- wiki/concepts/five-content-games.md — Five content-business model types (Entertainment Media / Education Media / Commoditized Consumer Product / Educational Consumer Product / B2B High-Education); education vs. entertainment definitional test; Traffic→Funnels→Offers hierarchy
- wiki/concepts/format-maturity-cycles.md — Four cycle stages (low supply → flood → saturation → evolution); Callaway's three format seasons; one-of-one moat when formats commoditize; niche maturity benchmarking
- wiki/concepts/creator-vs-entrepreneur-dichotomy.md — View-addiction spiral; broad-audience monetization failure; narrow ICP economics; open season analytical arbitrage thesis; skill-first mandate
- wiki/concepts/viewer-as-prediction-machine.md — Brain processes video as prediction engine; comprehension decay model; three editing mistakes; eyes-closed pacing test; 70% retention benchmark; one-question-at-a-time story audit; two-dopamine-hit lock-in
- wiki/concepts/one-of-one-content-moat.md — AI replicates formats not lived POV; AI replacement spectrum; term ownership / cult category fandom; five games in the AI era; full AI-proof strategy synthesis
- wiki/concepts/ai-arbitrage-window.md — 2007–2028 free distribution thesis; zig/zag model; post-2028 $10/post pay-to-play prediction; 3-year go-hard mandate; Gen 1 vs. Gen 2/For You era breakdown
- wiki/concepts/shock-score-system.md — 0–100 virality scoring; 100-people-in-a-room test; shocking vs. useful angle types; Payoff Principle (no bait-and-switch); zig-zag storytelling with successive stakes; conflict as subset of contrast

**Strategies (5)**
- wiki/strategies/seven-lego-bricks-short-form.md — All 7 bricks (topic/angle/hook structure/story structure/visual format/key visuals/audio); 6-step reverse-engineering protocol; copy-to-innovate progression; which bricks to hold constant vs. vary by skill level
- wiki/strategies/youtube-packaging-strategy.md — Title/thumbnail-first production order; desire loop psychology; complement rule; three-stage funnel; clickbait vs. bait-and-switch; CTR as noisy metric; 1-of-10 ranking system; TAM factor; dollars-per-view metric
- wiki/strategies/algorithm-sampling-loop.md — 200→2000 cascade mechanics; topic consistency as sample pool hygiene; content pillars; multi-channel atomization; evergreen "every video is a sales agent"; winners-first hack; hub-and-spoke repurposing
- wiki/strategies/short-form-production-loop.md — Six-step workflow; content operator / ideas guy role split; 180-page brain document; Sandcastles software; batching debate; editor management; numbered series binge architecture
- wiki/strategies/zero-to-1m-youtube-blueprint.md — High-ticket + precise YouTube = profit; skill-first mandate; comment cyclone strategy; super shares 1000x weighting; escape velocity; 5-type lead magnet taxonomy; Attention Factory vision

### INDEX.md Updated

- Stats: 9 brands, 69 concepts, 47 strategies, 164 total pages
- New brand added: Callaway
- New concept subcategory added: "Short-Form & YouTube Strategy" (9 new pages)
- New strategy subcategory added: "Short-Form & YouTube" (5 new pages)

---

---

## 2026-05-27 — Ingest: Orin John — LinkedIn Cursed Opportunity

- **Operation:** INGEST
- **Source:** YouTube — Orin John (Orin Meets World), "The Cursed Opportunity of LinkedIn" (https://www.youtube.com/watch?v=HtUiaOX12ls) — 640 segments, ~4,800 words, 4 chunks
- **Speaker:** Orin John — creative operator, marketing/brand/product leader, creator
- **Previous total:** 164 pages
- **New total:** 171 pages (+7 new pages, +2 existing pages updated)

### Pages Created (7)

**Concepts (6)**
- wiki/concepts/linkedin-platform-strategy.md — Overview: cursed opportunity thesis, video plays vs. impressions, bottom-of-funnel closer mechanic, Three Personas (Creator/Brand/Employee), Company Cohort Effect
- wiki/concepts/linkedin-cursed-opportunity.md — LinkedIn's cringe/bad UX reduces competition; vacuum rule; professional stakes; why surface negatives = strategic opportunity
- wiki/concepts/linkedin-impression-inflation.md — Carousel phantom impressions vs. plays as real metric; at-work consumption behavior; how to read LinkedIn analytics
- wiki/concepts/linkedin-bottom-of-funnel-closer.md — LinkedIn as closing layer for creators; professional context removes DM awkwardness; cross-posting as minimum viable strategy
- wiki/concepts/the-steve-role.md — Non-founder employee as brand LinkedIn correspondent; personal pages ~13x brand page reach; how to identify and activate your Steve
- wiki/concepts/linkedin-lens-framework.md — Fixed expertise filter permanently solving "what do I post?"; social-first onboarding (3-5 comments/week); Company Cohort Effect as free amplifier

**Strategies (1)**
- wiki/strategies/linkedin-brand-playbook.md — Chlorophyll Water cheerleading strategy; Steve Role operational details; Corell Water founder-as-distributor model; Lens Framework; social-first onboarding; brand vs. personal page exception logic

### Pages Updated (2)
- wiki/strategies/linkedin-content-strategy-2026.md — Added LinkedIn Platform Context section: Company Cohort Effect, brand account exception, Three Personas summary, plays-not-impressions rule, cross-posting strategy
- wiki/concepts/creator-first-brand-strategy.md — Added LinkedIn as Closing Layer section

### INDEX.md Updated
- Stats: 75 concepts, 48 strategies, 171 total pages
- New concept subcategory added: "LinkedIn" (6 pages)
- LinkedIn Brand Playbook added to Marketing & Campaigns strategies

---

*Next ingest: drop a file into /raw and say `ingest [filename]`*
