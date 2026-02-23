# PMM Skillset

Claude Code skills for Product Marketing Managers.

Built by [Gab Bujold](https://newsletter.messagingsherpa.com) — The Agentic PMM.

Most AI tools give marketers generic advice. These skills give PMMs a system: opinionated frameworks, evidence-based outputs, and artifacts they can actually use in stakeholder meetings, sales calls, and GTM sprints.

**The core question driving every skill:**
> *"Is our messaging specific enough to move the right people?"*

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
cp -r pmm-skillset/skills/* .claude/skills/
```

Then invoke any skill in Claude Code:

```
/message-market-fit
```

---

## Available Skills

<!-- SKILLS:START -->
| Skill | Status | Description |
|---|---|---|
| [message-market-fit](skills/message-market-fit/) | ✅ Available | Audit existing messaging assets against a specific ICP persona, score them across 5 pillars, generate 4 test variants, and run a 3-week multi-channel sprint with qualitative and quantitative signal in parallel. Produces a stakeholder-ready Messaging Specificity Report. |
<!-- SKILLS:END -->

---

## Full Skill Roadmap

What's being built and in what order — ranked by the impact PMMs get from each skill relative to the effort to implement it.

### Tier 1 — The Foundation
*Build these first. Everything else depends on them.*

| # | Skill | What it does | Why it's first |
|---|---|---|---|
| 1 | `message-market-fit` ✅ | Audit assets, score specificity, test variants, declare winner | The diagnostic that exposes every other problem |
| 2 | `icp-definition` | Build a layered ICP: firmographic → behavioral → psychographic → anti-ICP | You can't write specific messaging without a specific audience |
| 3 | `positioning-audit` | Map your position vs. 3–5 competitors, identify white space, flag positioning debt | Bad messaging is usually a positioning problem in disguise |

### Tier 2 — Build the Messaging System
*Once the foundation is solid, build the architecture.*

| # | Skill | What it does |
|---|---|---|
| 4 | `messaging-hierarchy` | Build the full stack: positioning → POV → value props → proof points → microcopy |
| 5 | `voc-synthesis` | Process customer interview transcripts into ICP patterns, echo language, and JTBD maps |
| 6 | `competitor-teardown` | Analyze a competitor's full messaging posture: positioning, copy, pricing, review sentiment |

### Tier 3 — Activate Across GTM
*Take the messaging system and deploy it where it creates revenue.*

| # | Skill | What it does |
|---|---|---|
| 7 | `launch-brief` | Full launch document: audience, hook, channel plan, success metrics, stakeholder alignment |
| 8 | `battle-card` | One-page competitive battle card for sales — built from your messaging system, not opinions |
| 9 | `sales-narrative` | Transform a pitch deck into a structured story arc: problem → insight → proof → ask |
| 10 | `feature-announcement` | Turn release notes into a product narrative that creates demand, not just awareness |

### Tier 4 — Close the Loop
*Feed real-world signal back into the messaging system.*

| # | Skill | What it does |
|---|---|---|
| 11 | `win-loss-analysis` | Extract patterns from win/loss interviews into messaging implications and positioning adjustments |
| 12 | `objection-handler` | Map common objections to specific messaging responses with proof points and talk tracks |
| 13 | `case-study-framework` | Structure a customer case study using the same messaging pillars as your GTM — so it compounds |
| 14 | `executive-briefing` | Turn market data and messaging results into a tight, revenue-tied narrative for leadership |

---

## Where to Start

**If you're a solo PMM fighting messaging-by-committee:**
→ Start with `message-market-fit`. Run the audit on your current website and outbound. Use the Messaging Specificity Report in your next stakeholder meeting.

**If your pipeline is weak and you're not sure why:**
→ Start with `icp-definition`, then `message-market-fit`. Vague ICP is usually the root cause of weak pipeline — not bad copy.

**If you're launching something in the next 4–6 weeks:**
→ Start with `message-market-fit` to validate your angle, then `launch-brief` to build the GTM plan around it.

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

## About

Built by [Gab Bujold](https://newsletter.messagingsherpa.com), product marketing consultant and creator of the Messaging Sherpa newsletter.

Gab has worked with 30+ B2B SaaS startups on positioning and messaging, surveyed 65+ PMMs on their testing processes, and built the message testing system these skills are based on.

Questions, feedback, or want to contribute a skill? [Open an issue](https://github.com/Fearofsnakes/pmm-skillset/issues) or reach out on [LinkedIn](https://www.linkedin.com/in/gabriel-bujold/).

---

*PMMs don't need more opinions on their messaging. They need a system.*
