# PMM AI System

A system of seven AI-powered skills for B2B product marketing. Each skill encodes a specific PMM workflow with operator frameworks, structured inputs, routing logic, quality standards, and stress tests built in.

## Why a system, not a prompt library

Most "AI for marketers" content stops at prompts. A prompt is a single instruction. A skill is a workflow: it loads context, diagnoses the job, routes to the right framework, produces structured output, runs quality checks, and feeds results into downstream skills.

The difference matters. A prompt for competitive analysis gives you a generic summary. A skill for competitive analysis loads your positioning context, applies Dunford's competitive alternatives framework (which includes do-nothing, in-house, and agency alternatives most CI programs miss), cross-references product documentation against marketing claims, captures Sharp's distinctive brand assets, and produces a battlecard structured for a rep under pressure in a live deal. Then the next skill in the system reads that battlecard when building launch messaging.

Every skill in this system reads from and writes to a shared context layer, so work compounds across the full PMM surface instead of starting from zero each session.

## Before you run anything: what you need to provide

The frameworks are built in. The company-specific context is not — and that's intentional. Generic inputs produce generic output. Before running any skill, you populate the Context Foundation file with your specifics:

| Input area | What to provide |
|------------|----------------|
| Product | What it does, real differentiators, feature set, roadmap direction |
| Pricing and packaging | Tiers, value metric, free/trial motion if applicable |
| Competitive landscape | Direct competitors, indirect alternatives, do-nothing option, in-house build |
| Audience | ICP profile, persona breakdown, trigger events, buying fears |
| Sales motion | How deals are sourced, cycle length, where they stall, how reps actually sell |
| Current positioning | Existing messaging, perception gaps, known objections |

The Context Foundation skill structures these inputs against the operating frameworks. Every downstream skill inherits the result. This is what separates the system from a prompt library: the frameworks run on your specific reality, not a generic approximation of it.

## The system

| Skill | What it does | Frameworks |
|-------|-------------|------------|
| [Context Foundation](skills/context-foundation.md) | Builds and maintains the shared knowledge base every other skill reads from | Ritson (diagnosis → strategy → tactics), Dunford (positioning components), Sharp (mental availability, CEPs), Kramer (audiences → goals → strategies → tactics) |
| [Positioning & Messaging](skills/positioning-messaging.md) | Builds positioning frameworks, message houses, value props, and launch narratives using the right framework for the job | Dunford, Fletch (Pierri & Kaminski), Raskin, Neumeier, Sharp + Laja stress tests |
| [Competitive Intelligence](skills/competitive-intel.md) | Produces battlecards, comparison pages, and competitive monitoring with research across marketing claims, product docs, and brand assets | Dunford (competitive alternatives), Sharp (distinctive brand assets) |
| [Buyer Research](skills/buyer-research.md) | Runs win/loss analysis, JTBD mapping, VoC synthesis, and message testing | Ritson (diagnosis-first research design), Moesta (JTBD + forces of progress), Dunford (win/loss spine), Laja/Wynter (message testing) |
| [Go-to-Market](skills/go-to-market.md) | Builds launch playbooks, GTM timelines, sales enablement, and cross-functional coordination | Ritson (diagnose before you plan), Oakley (launch tiering), Kramer (audiences → goals → strategies → tactics), Raskin (strategic narrative) |
| [Pricing & Packaging](skills/pricing-packaging.md) | Develops pricing strategy, tier structure, value metric selection, and PLG pricing mechanics | Poyar (value metrics, PLG benchmarks, packaging principles) |
| [PLG Growth Pulse](skills/plg-growth-pulse.md) | Weekly PLG health check benchmarked against industry data | Poyar (PLG benchmarks by ACV band), Sharp (light-buyer reality) |

## How the system connects

```
Context Foundation
    ├── Positioning & Messaging
    │     ├── Go-to-Market (reads messaging, writes launch plans)
    │     └── Competitive Intel (reads positioning, writes battlecards)
    ├── Buyer Research (reads ICP, writes insights that update context)
    ├── Pricing & Packaging (reads ICP + competitive, writes packaging)
    └── PLG Growth Pulse (reads context weekly, benchmarks against Poyar)
```

The Context Foundation skill runs first. It builds the shared knowledge base (market diagnosis, positioning components, competitive landscape, ICP, mental availability mapping) that every downstream skill inherits. When any skill produces new insight (a win/loss pattern, a competitive shift, a PLG metric trend), it updates the context layer so the next skill session starts smarter.

## The frameworks baked in

- **April Dunford** (Obviously Awesome) — positioning components, competitive alternatives
- **Mark Ritson** — diagnosis → strategy → tactics, research-first discipline
- **Byron Sharp** (How Brands Grow) — mental availability, CEPs, distinctive brand assets, light-buyer reality
- **Andy Raskin** — strategic narrative for B2B SaaS
- **Emily Kramer** (MKT1) — audiences → goals → strategies → tactics
- **Bob Moesta** (JTBD) — forces of progress, switch interview methodology
- **Jason Oakley** (Productive PMM) — launch tiering (T1/T2/T3) and launch operations
- **Kyle Poyar** — PLG benchmarks by ACV band, value metrics, packaging principles
- **Peep Laja** (CXL) — message testing, conversion, PLG
- **Martina Lauchengco** (Loved) — PMM operating model, product-market fit signals
- **Marty Neumeier** (Brand Gap, Zag) — brand differentiation, category design

When the system draws on these frameworks, it weaves them into the workflow as operating logic, not as citations. Senior PMMs who articulate strong frameworks as their own thinking come off as practitioners. Senior PMMs who recite framework names come off as academic.

## What this system has produced

- A competitive intelligence program with 12 maintained battlecards and 75% reduction in ad-hoc research time
- AI positioning for a skeptical creative audience that turned resistance into adoption
- A PLG motion built from scratch inside a sales-led org, with weekly benchmarked health checks
- Launch playbooks that compressed messaging development from weeks to days
- Win/loss analysis structured around forces of progress, not post-rationalized survey responses

## How I think about AI in PMM

AI doesn't replace the strategic judgment in product marketing. It replaces the manual labor that used to sit between a strategic question and a useful answer.

The pattern across every skill in this system is the same: AI compresses research, synthesis, and first-draft generation so I spend more time on the work that actually matters — positioning decisions, narrative architecture, go-to-market sequencing, the politics of getting a room full of stakeholders to agree on a story. The human judgment layer never gets automated. The grunt work does.

The key insight that made this system work: generic AI prompts produce generic output. AI grounded in specific frameworks, structured inputs, quality standards, and stress tests produces output at the level of a senior practitioner's first draft. That's the difference between "use AI for competitive research" and a skill that knows to check product documentation against marketing claims, capture distinctive brand assets most CI programs miss, and structure the battlecard for a rep under pressure in a live deal.
