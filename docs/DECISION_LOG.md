# Decision Log

---

## 2026-07-21 — From Super App to Personal Decision Engine

### Context

The project started with the idea of building a consumer Super App composed of multiple mini applications connected through a shared recommendation engine.

After several discussions, it became clear that the mini apps themselves are not the long-term value of the company.

### Decision

PDE is no longer defined as a Super App.

PDE is defined as a **Personal Decision Engine**.

Mini apps are simply data collection and interaction mechanisms that contribute to building a richer understanding of each user.

The long-term asset of the company is the continuously evolving user model.

---

## 2026-07-21 — The company exists to reduce the cost of decision making

### Context

Initially, the project focused on building better recommendation systems.

However, analysing real user behaviour revealed that recommendations are not the main problem.

Users spend significant amounts of time searching, comparing and evaluating options before making a decision.

### Decision

The primary problem PDE aims to solve is **the cost of evaluating choices**, not the lack of recommendations.

Success should be measured by reducing the effort required to make decisions rather than by increasing the number of recommendations shown.

---

## 2026-07-21 — The core problem is behavioural, not technological

### Context

Instead of starting from technology (AI, Interest Graph, PostgreSQL...), we analysed how people actually make decisions.

Patterns repeatedly appeared across different domains such as movies, restaurants, books and travel.

### Decision

Product discovery will focus on understanding user behaviour before making architectural decisions.

Technology exists to support the product, not define it.

---

## 2026-07-21 — New company thesis

Current working thesis:

> The Internet solved access to information.
> It did not solve decision making.

This statement will act as one of the central hypotheses of the project until validated or disproved.

---

## 2026-07-22 — Work locally before pushing to GitHub

### Context

The repository was connected to GitHub, but the project is still in an exploratory phase. Most current work is strategy, problem framing and product thinking rather than finalized implementation.

Committing every early draft directly to GitHub would create unnecessary history noise and could make half-formed thinking look more settled than it is.

### Decision

The default workflow will be local-first:

- work on documents locally
- iterate until a version is coherent
- commit only when the change is worth preserving
- push to GitHub after review

GitHub remains the durable source of truth, but not every exploratory edit needs to be pushed immediately.

---

## 2026-07-22 — Normalize the repository structure

### Context

The repository contained top-level files with numbered names and no markdown extensions, such as `1. README`, `2. CONTEXT` and `3. WORKING_BACKWARDS`. The README described a cleaner structure using `README.md`, `CONTEXT.md`, a `docs/` directory and a `notes/` directory.

This mismatch made the repository harder to navigate and created friction for future documentation work.

### Decision

The documentation structure should be normalized:

- `README.md` and `CONTEXT.md` stay at the root
- strategy documents live under `docs/`
- markdown files use `.md` extensions
- `notes/` exists for scratch or lower-certainty thinking

This change is organizational only. It does not change the product strategy by itself.

---

## 2026-07-22 — Working Backwards should start from the customer problem

### Context

The initial `WORKING_BACKWARDS.md` began with the long-term PDE vision and then moved into the user problem.

Starting from vision is useful for motivation, but it risks making the document too broad. A Working Backwards artifact should force clarity about the first customer, the specific decision pain and the first wedge.

### Decision

The next substantial work on `WORKING_BACKWARDS.md` should tighten the problem before expanding the rest of the document.

The useful structure for the problem section is:

- target customer
- situation
- current behavior
- pain
- existing alternatives
- why existing alternatives fail
- core problem statement

The Press Release, Customer Story, FAQ and Success Metrics should be written only after the problem is precise enough to constrain the product.

---

## 2026-07-22 — Cross-domain value may come from multiple transfer mechanisms

### Context

R6 originally framed cross-domain value as weak or absent cross-domain signal. That framing implicitly assumed one mechanism: taste transfer, where preferences in one domain predict preferences in another.

This is too narrow. If taste transfer fails, it would be premature to conclude that horizontal expansion cannot work.

### Decision

The project now distinguishes at least three possible transfer mechanisms:

- **Taste transfer:** preferences in domain A predict preferences in domain B.
- **Decision-style transfer:** behavioral traits such as novelty-seeking, price sensitivity or social-proof reliance generalize across domains.
- **Social trust transfer:** value comes from shared identity, friends, reputation or social proof, not from a predictive model of the user.

This is captured in `RISKS.md` as R6b.

The key implication is that PDE should not assume horizontal value comes from the Interest Graph alone. Different domain pairs may require different transfer mechanisms.

---

## 2026-07-22 — Expansion should be organized by transfer mechanism, not ambition

### Context

The project needs to preserve thinking about horizontal expansion without allowing that thinking to justify premature scope expansion.

Adding more mini apps should not be treated as a roadmap by default. The right question is not "which vertical should we add next?" but "which transfer mechanism are we testing, and why might it work for this domain pair?"

### Decision

Create `EXPANSION_HYPOTHESIS.md` as a non-authorizing strategy note.

The document exists to preserve reasoning about possible expansion paths, but it explicitly does not authorize building beyond domain 1.

The sequencing principle is:

- near domains should test taste transfer first
- medium-distance domains should test decision-style transfer
- far domains should expect taste transfer to be weak and may require social trust transfer

Social trust transfer should be treated as a strategic fork, not a default next step. Introducing friends, reputation and community may make PDE less of a personal AI or Interest Graph product and more of a trusted social decision network.

---

## 2026-07-22 — Domain 1 must win on its own merits

### Context

The expansion hypothesis depends on having at least one real domain with meaningful usage. Without retention in domain 1, cross-domain transfer cannot be tested honestly.

If the first mini app only exists as a sensor for a future graph, it will not generate enough signal to validate anything.

### Decision

No expansion hypothesis should influence what gets built until domain 1 has validated retention as a standalone product.

This reinforces R3: the first mini app must be evaluated as a product, not as a data collection mechanism.
