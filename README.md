# PMM Skillset

Claude Code skills for Product Marketing Managers.

Built by [Gab Bujold](https://www.linkedin.com/in/gabriel-bujold/) — The Agentic PMM. Subscribe to the [Employee Zero newsletter](https://newsletter.pressxtomarket.com?ref=pmm-skillset) for weekly breakdowns on AI-powered product marketing.

Most AI tools give marketers generic advice. These skills give PMMs a system: opinionated frameworks, evidence-based outputs, and artifacts they can actually use in stakeholder meetings, sales calls, and GTM sprints.

**The core question driving every skill:**
> *"Is our messaging specific enough to move the right people?"*

---

## How Skills Work Together

Each skill produces a specific artifact. Skills chain together — the output of one becomes the input of the next.

```
                    ┌─────────────────┐
                    │  icp-definition  │
                    │   (who to target)│
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │positioning-audit │
                    │ (where you stand)│
                    └────────┬────────┘
                             │
               ┌─────────────┼─────────────┐
               │             │             │
      ┌────────▼───────┐    │    ┌────────▼────────┐
      │ voc-synthesis   │    │    │ competitor-      │
      │ (buyer language)│    │    │ teardown         │
      └────────┬───────┘    │    └────────┬────────┘
               │             │             │
               └─────────────┼─────────────┘
                             │
                    ┌────────▼────────┐
                    │   messaging-    │
                    │   hierarchy     │
                    │ (what to say)   │
                    └────────┬────────┘
                             │
          ┌──────────────────┼──────────────────┐
          │                  │                  │
 ┌────────▼───────┐ ┌───────▼────────┐ ┌───────▼────────┐
 │message-market-  │ │ competitive-   │ │  launch-brief  │
 │fit              │ │ landing-page   │ │  (GTM plan)    │
 │(test & prove)   │ │ (convert)      │ │                │
 └─────────────────┘ └───────┬────────┘ └───────┬────────┘
                             │                  │
          ┌──────────────────┼──────────────────┤
          │                  │                  │
 ┌────────▼───────┐ ┌───────▼────────┐ ┌───────▼────────┐
 │ battle-card     │ │ sales-         │ │ feature-       │
 │ (arm sales)     │ │ narrative      │ │ announcement   │
 │                 │ │ (tell story)   │ │ (create demand)│
 └─────────────────┘ └────────────────┘ └────────────────┘
```

You don't have to run them in order. Each skill works standalone. But they compound when chained.

---

## How to Install

```bash
# Install all skills
npx skills add Fearofsnakes/pmm-skillset

# Install a specific skill
npx skills add Fearofsnakes/pmm-skillset --skill message-market-fit
```

Or clone and copy manually:

```bash
git clone https://github.com/Fearofsnakes/pmm-skillset.git

# Install all skills (preserves tier structure)
cp -r pmm-skillset/skills/* .claude/skills/

# Install a single tier
cp -r pmm-skillset/skills/tier-1/* .claude/skills/
```

Or use as a git submodule (keeps skills updated):

```bash
git submodule add https://github.com/Fearofsnakes/pmm-skillset.git .claude/skills/pmm-skillset
```

Then invoke any skill in Claude Code:

```
/message-market-fit
```

---

## Available Skills

<!-- SKILLS:START -->
| Skill | Tier | Status | Description |
|---|---|---|---|
| [icp-definition](skills/tier-1/icp-definition/) | 1 | ✅ Available | Build a layered ICP across 4 dimensions (firmographic, behavioral, psychographic, language), define the anti-ICP with disqualification signals and resource-drain indicators, calculate your disqualified ratio, and operationalize it with a signal map and activation checklist. Produces a stakeholder-ready ICP Profile Document. |
| [positioning-audit](skills/tier-1/positioning-audit/) | 1 | ✅ Available | Define and audit your positioning across 4 pillars (use case/category, audience, competitive alternative, differentiation), score positioning strength, flag positioning debt, and identify white space opportunities. Produces a stakeholder-ready Positioning Audit Report. |
| [messaging-hierarchy](skills/tier-1/messaging-hierarchy/) | 1 | ✅ Available | Build a 5-layer messaging stack from positioning: POV, value proposition, 3 benefits, proof points, and features — with quality tests at every layer, persona adaptations, channel mapping, and a narrative structure. Every element traces up the chain. Produces a stakeholder-ready Messaging Hierarchy Document with a "how to use this" guide per use case. |
| [message-market-fit](skills/tier-2/message-market-fit/) | 2 | ✅ Available | Audit existing messaging assets against a specific ICP persona, score them across 5 pillars, generate 4 test variants, and run a 3-week multi-channel sprint with qualitative and quantitative signal in parallel. Produces a stakeholder-ready Messaging Specificity Report. |
| [voc-synthesis](skills/tier-2/voc-synthesis/) | 2 | ✅ Available | Synthesize messy, multi-source VOC data (transcripts, surveys, reviews, CRM notes) into a structured Buyer Brain with frequency-weighted patterns, echo language bank, contradiction map, and evidence chains. Every claim traces to a real quote. Feeds directly into `/messaging-hierarchy`, `/positioning-audit`, and `/message-market-fit`. |
| [competitive-landing-page](skills/tier-2/competitive-landing-page/) | 2 | ✅ Available | Generate production-ready "Your Product vs Competitor" landing pages for Google Ads. Collects product identity, competitive intelligence, and real review quotes (G2, Capterra, TrustRadius), then outputs a complete self-contained HTML page with 13 conversion-optimized sections. First page becomes the template; subsequent competitors take ~10 min. Includes [example output](skills/tier-2/competitive-landing-page/examples/pipelineos-vs-dealforce.html). |
| [homepage-messaging](skills/tier-2/homepage-messaging/) | 2 | ✅ Available | Review a homepage structurally, block by block, against a fixed 4-layer rubric (hero, problem section, value propositions, whole page). Captures every block verbatim, scores each against a named criterion with pass/weak/fail and evidence, rewrites every failure, and separates the argument-order problems from the writing problems. Produces a side-by-side review and a build-ready change order with the blocking decisions surfaced up front. |
| [launch-brief](skills/tier-3/launch-brief/) | 3 | ✅ Available | Turn a product spec into a full launch plan: scope and tier the launch, define the messaging hook, build a channel plan with sequencing, set success metrics, map stakeholders with RACI, and produce a phase-by-phase execution timeline. Produces a stakeholder-ready Launch Brief Document with a 60-second launch pitch. |
| [battle-card](skills/tier-3/battle-card/) | 3 | ✅ Available | Build a one-page competitive battle card for sales — sourced from win/loss patterns, review data, and pricing intelligence. Includes positioning summary, "where we win / where we lose" with talk tracks, objection handling with verbatim responses, landmine questions for discovery, and a 90-second briefing. Every claim traces to evidence. |
| [sales-narrative](skills/tier-3/sales-narrative/) | 3 | ✅ Available | Transform a pitch deck into a structured 7-beat story arc: the shift → the cost → the old way → the new way → the proof → the product → the ask. Audits existing pitches for structural failures (feature dump, buried lead, no villain), builds persona-adapted talk tracks, and produces a slide-by-slide narrative guide with a 60-second version. |
| [feature-announcement](skills/tier-3/feature-announcement/) | 3 | ✅ Available | Turn release notes into a multi-channel announcement package that creates demand, not just awareness. Extracts the story from the spec, finds the narrative angle (moment, before/after, or unlock), and generates ready-to-ship copy for blog, email, social, in-product, and changelog — with a quality check per asset. |
<!-- SKILLS:END -->

---

## Full Skill Roadmap

What's being built and in what order — ranked by the impact PMMs get from each skill relative to the effort to implement it.

### Tier 1 — The Foundation
*Build these first. Everything else depends on them.*

| # | Skill | What it does | Why it's first |
|---|---|---|---|
| 1 | `icp-definition` ✅ | Build a layered ICP: firmographic → behavioral → psychographic → anti-ICP | You can't write specific messaging without a specific audience |
| 2 | `positioning-audit` ✅ | Map your position vs. 3–5 competitors, identify white space, flag positioning debt | Bad messaging is usually a positioning problem in disguise |
| 3 | `messaging-hierarchy` ✅ | Build the full stack: positioning → POV → value props → proof points → microcopy | The architecture that makes everything downstream consistent |

### Tier 2 — Test, Validate & Convert
*Once the foundation is solid, test it against the market.*

| # | Skill | What it does |
|---|---|---|
| 4 | `message-market-fit` ✅ | Audit assets, score specificity, test variants, declare winner |
| 5 | `voc-synthesis` ✅ | Synthesize multi-source VOC data into a frequency-weighted Buyer Brain with echo language, contradiction map, and evidence chains |
| 6 | `competitive-landing-page` ✅ | Generate production-ready "vs Competitor" landing pages for Google Ads with real review quotes, feature comparisons, and conversion-optimized copy |
| 7 | `homepage-messaging` ✅ | Review a homepage block by block against a fixed rubric, separate the order problems from the writing problems, and emit a build-ready change order |
| 8 | `competitor-teardown` | Analyze a competitor's full messaging posture: positioning, copy, pricing, review sentiment |

### Tier 3 — Activate Across GTM
*Take the messaging system and deploy it where it creates revenue.*

| # | Skill | What it does |
|---|---|---|
| 9 | `launch-brief` ✅ | Full launch document: audience, hook, channel plan, success metrics, stakeholder alignment |
| 10 | `battle-card` ✅ | One-page competitive battle card for sales — built from win/loss patterns, not opinions |
| 11 | `sales-narrative` ✅ | Transform a pitch deck into a 7-beat story arc: shift → cost → old way → new way → proof → product → ask |
| 12 | `feature-announcement` ✅ | Turn release notes into a multi-channel announcement package that creates demand, not just awareness |

### Tier 4 — Close the Loop
*Feed real-world signal back into the messaging system.*

| # | Skill | What it does |
|---|---|---|
| 13 | `win-loss-analysis` | Extract patterns from win/loss interviews into messaging implications and positioning adjustments |
| 14 | `objection-handler` | Map common objections to specific messaging responses with proof points and talk tracks |
| 15 | `case-study-framework` | Structure a customer case study using the same messaging pillars as your GTM — so it compounds |
| 16 | `executive-briefing` | Turn market data and messaging results into a tight, revenue-tied narrative for leadership |

---

## Set Up Your CLAUDE.md First

Every skill in this repo reads your project's `CLAUDE.md` file for context — your product, ICP, positioning, competitive landscape, proof points, and voice. If your CLAUDE.md is weak, every skill output is weak. If it's dialed in, every skill operates like a PMM who's been at your company for 6 months.

**[Grab the template →](CLAUDE.md.template)** Copy it to the root of your project directory as `CLAUDE.md` and fill it in. Takes about an hour. Pays for itself on every single skill run.

---

## Where to Start

**If you're a solo PMM fighting messaging-by-committee:**
→ Start with `icp-definition` and `positioning-audit` to build the foundation, then run `message-market-fit` to score your current messaging with evidence your stakeholders can't argue with.

**If your pipeline is weak and you're not sure why:**
→ Start with `icp-definition`. Vague ICP is usually the root cause of weak pipeline — not bad copy. Then run `message-market-fit` to test what you've got.

**If you're launching something in the next 4–6 weeks:**
→ Start with `messaging-hierarchy` to lock your message stack, then `launch-brief` to build the GTM plan around it.

**If sales keeps rewriting your messaging:**
→ Start with `message-market-fit` to produce evidence, then `battle-card` to give reps a tool that's faster than rewriting your work.

---

## What Makes These Different

**Built for PMMs, not generalists:**
These skills encode the unique challenges of the PMM role — stakeholder buy-in, messaging by committee, connecting copy to pipeline, sales enablement. Not generic marketing advice repackaged.

**Every skill produces a real artifact:**
A scored report, a set of variants, a battle card — not just "here's what to think about." PMMs don't need more frameworks. They need outputs they can put in front of a CEO.

**Evidence-based, not opinion-based:**
These skills crawl real assets (website URLs, ad copy, email sequences), score them against your specific ICP persona, and produce evidence-backed recommendations. The output changes based on your actual situation, not a template.

---

## Contributing

Want to contribute a skill or improve an existing one? See [CONTRIBUTING.md](CONTRIBUTING.md) for the skill structure, quality checklist, and submission process.

---

## About

Built by [Gab Bujold](https://www.linkedin.com/in/gabriel-bujold/), product marketer and creator of the [Employee Zero newsletter](https://newsletter.pressxtomarket.com?ref=pmm-skillset).

Gab has worked with 40+ B2B SaaS startups on positioning and messaging, surveyed 65+ PMMs on their testing processes, and built the message testing system these skills are based on.

Questions, feedback, or want to contribute a skill? [Open an issue](https://github.com/Fearofsnakes/pmm-skillset/issues) or reach out on [LinkedIn](https://www.linkedin.com/in/gabriel-bujold/).

---

## License

[MIT](LICENSE)

---

*PMMs don't need more opinions on their messaging. They need a system.*
