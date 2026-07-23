# EXPANSION_HYPOTHESIS.md

> **This document does not authorize building anything beyond domain 1.**
> It exists so a real conversation about horizontal expansion isn't lost — not to plan a roadmap.
> It should only be revisited once domain 1 (the first mini app) has validated retention on its own merits (see R3 in RISKS.md). Until then, nothing below should influence what gets built.

**Context:** written 2026-07-21, before domain 1 has been chosen or validated. Purely a hypothesis about *how* horizontal value might work, in case it becomes relevant later — not a commitment to any sequence or timeline.

---

## The core question

Going from a single domain (e.g., cooking) to a truly horizontal decision engine (entertainment, travel, fitness...) is not automatically easier just because the underlying tech is reusable. The real question is: **what mechanism, if any, makes knowledge from one domain useful in another?** There isn't one answer — there are at least three distinct, competing mechanisms, and they generalize very differently across domain distance.

## The three mechanisms (see RISKS.md, R6 and R6b for the risk framing)

**1. Taste transfer** — preferences in domain A predict preferences in domain B (e.g., liking spicy food → liking a certain travel style). Likely strong only within closely related domains. Probably close to nonexistent across distant ones. This is the mechanism implicitly assumed by the original Interest Graph framing, and it is the weakest of the three for distant domains.

**2. Decision-style transfer** — behavioral traits (novelty-seeking vs. repeats-the-safe-choice, fast vs. deliberate decisions, price sensitivity, trust in social proof vs. objective data) generalize across domains even when taste doesn't. Unvalidated, but structurally more plausible for medium-distance domains.

**3. Social trust transfer** — value comes from shared identity and social proof (the same friends, the same reputation informing decisions across verticals), not from any predictive model of the user at all. This is closer to how real super apps (WeChat, Gojek) actually unified verticals. Requires the least unproven inference, and is likely the most viable mechanism for distant domains.

## Sequencing principle

The default expansion logic should be: **use the least complex mechanism that can plausibly work for the next domain.**

This means PDE should generally test taste transfer and decision-style transfer before building anything that depends heavily on social trust transfer. Not because social trust is less plausible, but because it changes the nature of the product more dramatically.

Taste transfer and decision-style transfer keep PDE closer to the original thesis: a system that helps the user make better decisions by understanding them. Social trust transfer introduces identity, friends, reputation, community, and network effects. That may become valuable, but it is a different strategic fork.

The tentative rule:

- **Near domains** → test taste transfer first.
- **Medium-distance domains** → test decision-style transfer before assuming taste transfer works.
- **Far domains** → expect taste transfer to be weak; social trust transfer may be the more plausible mechanism.

In practical terms:

- Cooking → groceries → restaurants should first test taste transfer.
- Restaurants → fitness/running should test decision-style transfer.
- Cooking → entertainment or travel should probably not rely on inferred taste; social trust may be the more realistic path.

The reason not to jump to social trust too early is measurement clarity. Once friends/community are introduced, we may no longer know whether PDE is working because it understands the user or because people trust recommendations from other people. That distinction matters because it implies a different product, architecture, growth model, and company.

Social trust should therefore be treated as a later strategic fork unless domain 1 naturally has a social use case from day one.

## A tentative expansion order — organized by which mechanism it would test, not by when to build it

The table below uses cooking as an illustrative domain 1. If domain 1 changes, this table should be rewritten rather than reused mechanically.

| Domain step | Distance from domain 1 (cooking) | Mechanism most likely to apply | Notes |
|---|---|---|---|
| Groceries / pantry recipes | Very close (same domain) | Taste transfer | Near-zero risk if this step is ever taken; barely a "new domain" |
| Restaurants | Close (same underlying need: what to eat) | Taste transfer | Good candidate to validate whether taste transfer works at all, at low risk |
| Fitness / running | Medium distance | Decision-style transfer | Should be tested explicitly for style transfer (e.g., "explorer" trait), not assumed via taste |
| Entertainment | Far | Social trust transfer | Approach via "people you trust liked this," not inferred taste or inferred style |
| Travel | Far | Social trust transfer | Same as entertainment — likely the hardest domain to justify via any personalization mechanism other than social proof |

## What would need to be true before taking any step in this table seriously

- Domain 1 has validated retention as a standalone product (R3 resolved positively).
- The specific mechanism relevant to the next step has been tested with real cross-domain usage data, not assumed (R6 / R6b resolved, not just hypothesized).
- The GDPR gate for cross-domain data merging has been addressed (R8), specifically at the point two domains' data are combined for the same user.

## What this document is not

It is not a commitment to build entertainment or travel features. It is not evidence that horizontal expansion will work. It is a record of *how* we'd think about testing it, written now so the reasoning isn't lost or re-derived from scratch later — and so that if domain 1 succeeds, the temptation to jump straight to "add more mini apps" gets redirected toward "test which mechanism, if any, actually transfers" instead.
