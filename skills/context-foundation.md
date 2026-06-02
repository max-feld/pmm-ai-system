# Context Foundation

The first skill in the system. Every other skill reads from the context file this one produces.

## The problem it solves

AI sessions start cold. Every time you open a new conversation, the AI knows nothing about your product, market, competitive landscape, ICP, or GTM motion. You re-explain context, it produces generic output, and you spend more time correcting than creating.

This skill builds a persistent, structured knowledge base that every downstream skill inherits. Run it once, maintain it quarterly, and every subsequent PMM workflow starts with full context instead of a blank slate.

## What you need to input

The frameworks in this system are built in. The company-specific context is not — and that's intentional. Generic inputs produce generic output. Before running any downstream skill, you populate the context file with your specifics:

**Product**
- What the product does and the problem it solves
- Real differentiators (not marketing language — actual capability gaps vs. alternatives)
- Current feature set and roadmap direction (as much as you can share)
- Pricing and packaging tiers, value metric, and where free/trial fits (if applicable)

**Market and competitive landscape**
- The real competitive set: direct competitors, indirect alternatives, the do-nothing option, and in-house build
- How your category is currently defined and whether that definition works in your favor
- Known competitive weaknesses and where you win

**Audience**
- ICP: company profile, buying role, and the job they're trying to do
- Persona breakdown: who influences, who decides, who uses, who pays
- The trigger events that move buyers into market
- What they're afraid of getting wrong

**Sales motion**
- How deals are sourced (inbound, outbound, PLG, partner)
- Typical sales cycle length and deal complexity
- Where deals stall and why
- How sales currently talks about the product (not how marketing wants them to — how they actually do)

**Current positioning**
- Existing messaging pillars and where they're working or not
- How the company is perceived vs. how you want it to be perceived
- Known objections and how they're currently handled

## The framework

The context file is structured around four B2B marketing frameworks, applied in the order Mark Ritson teaches:

**1. Diagnosis first (Ritson).** What's actually happening in the business, market, competition, and customer base. Every strategic decision should be traceable to something in the diagnosis. Skipping diagnosis is how strategy goes wrong.

**2. Strategy second.** Built on three complementary frameworks:
- **Dunford** positioning components (competitive alternatives, unique attributes, value themes, ICP, market frame)
- **Kramer** marketing strategy (audiences → goals → strategies → tactics)
- **Sharp** mental availability (Category Entry Points, distinctive brand assets, light-buyer reality)

**3. Tactics last.** Channels, campaigns, enablement, and operational details come after the strategic foundation is set.

## What the context file contains

The output is a single markdown file with these sections:

**Diagnosis** — state of the business, state of the category, state of competition, state of the customer, and the strategic implications ("so what"). This is the section most PMMs skip and it's the most valuable. A good diagnosis names the tensions: where is the category unsettled, where are competitors winning deals they shouldn't, where is the customer behavior shifting.

**Audiences (Kramer)** — named audience segments with triggers, channels, and best paths to conversion. Not generic personas. Each audience has a specific growth motion attached.

**Positioning (Dunford components)** — best-fit ICP, competitive alternatives (including do-nothing, in-house, and agency, not just named competitors), unique attributes, value themes, and market frame of reference. This is the positioning spine every messaging and competitive skill inherits.

**Mental availability (Sharp)** — Category Entry Points (the buying moments you want to own), distinctive brand assets (visual, verbal, narrative), and light-buyer reality (most of your audience thinks about your category a few times a year, not weekly).

**Tactics** — GTM motion, channels, sales enablement patterns, and current priorities.

**Proof points** — quantitative evidence organized for use across messaging, enablement, and content.

## How it feeds downstream

Every skill in the system reads the context file before starting work:

- **Positioning & Messaging** inherits the Dunford components and Sharp stress tests
- **Competitive Intel** inherits the competitive alternatives and distinctive asset baselines
- **Buyer Research** inherits the ICP hypotheses to validate or challenge
- **Go-to-Market** inherits the audience definitions and strategic priorities
- **Pricing** inherits the competitive landscape and GTM motion
- **PLG Pulse** inherits the ICP definition and benchmark targets

When any downstream skill produces new insight (a win/loss pattern, a competitive shift, a PLG metric trend), it writes back to the context file. The knowledge base gets smarter over time.

## Quality standards

Good context is diagnosis-first (every strategic claim traceable to the diagnosis section), specific (named ICP segments, not "marketing teams"), CEP-aware (names the actual buying moments, not abstract triggers), audience-mapped (every priority traceable to a specific audience), honest (captures actual differentiators, not aspirational claims), and current (dated so you know when it was last accurate).

Bad context is tactics-first, generic enough to describe any company in the space, missing the competitive alternatives section, missing CEPs and distinctive assets, full of marketing-speak that doesn't mean anything specific, or so long it adds noise to every downstream session.

## The maintenance cadence

Context isn't set-and-forget. The skill flags when inputs are likely stale: after a product launch, a pricing change, a competitive move, or a significant win/loss pattern shift. Treat it like a living document, not a one-time setup.
