# Project Context

> This document represents the current state of the project.
> It should always answer one question:
>
> **"If someone joins the project today, what do they need to understand in five minutes?"**

---

# Current Status

**Project**

Personal Decision Engine (PDE)

**Version**

0.1

**Stage**

Discovery

Current Objective

Validate whether reducing the cost of personal decision making is a problem large enough to build a company around.

---

# Our Compass

We are **not** building a Super App.

We are building a system capable of understanding a person better than any individual application.

The objective is not to recommend the best movie.

The objective is to recommend the best decision for a specific person.

Everything we build should move us towards that goal.

---

# Core Thesis

People's interests are fragmented.

Netflix knows movies.

Spotify knows music.

Google Maps knows restaurants.

Amazon knows purchases.

Booking knows travel.

Each company understands only one part of the user.

We believe there is value in connecting all those interests into a single knowledge model.

That knowledge can then be used to make significantly better recommendations.

Important qualification: cross-domain value is still unvalidated. It may come from taste transfer, decision-style transfer, social trust transfer, or none of them. The project should not assume horizontal expansion works until domain 1 has retention and transfer mechanisms can be tested with real usage.

---

# Technical Value

The technical asset of the company is **not** an AI assistant.

It is a structured representation of the user.

Conceptually:

```
Mini Apps

↓

Interest Graph

↓

Context Engine

↓

Personal Decision Engine

↓

User
```

The AI is only the reasoning layer.

The real asset is the knowledge underneath.

---

# What We Believe

Current hypotheses that appear strong:

- The long-term value is the user model, not the mini apps.
- Every new feature should improve the knowledge of the user.
- AI should reason using structured knowledge instead of memorising information.
- Better recommendations come from understanding people, not individual categories.
- Community recommendations may become as important as AI recommendations.
- The first mini app must win as a standalone product before it can be useful as a sensor.
- Expansion should be organized by transfer mechanism, not by ambition to add more verticals.

---

# Open Questions

These are currently the biggest risks.

1. Can a company built around reducing the cognitive cost of decision making generate enough daily value for users to build long-term retention?

## Product

Why would someone use PDE every week?

What is the smallest product capable of validating our thesis?

What is the first mini app?

Who is the first user?

What specific recurring decision is painful enough to create weekly retention?

How do we create value in less than five minutes?

How do we minimise onboarding friction?

Which transfer mechanism, if any, actually works across domains?

---

## Technology

How should the Interest Graph evolve?

When will PostgreSQL stop being enough?

How much context does the AI actually need?

---

## Business

Can affiliate revenue finance the first years?

What retention would make this a viable business?

When should Premium exist?

---

# Recent Progress

## Decisions

- We abandoned the idea of defining the company as a "Super App".
- The company is now defined as a Personal Decision Engine.
- Mini apps are considered information sources, not products.
- The user model is considered the long-term competitive advantage.
- The primary user problem is no longer considered to be recommendations, but the effort required to evaluate an increasing number of options.
- Product discovery will focus on user behaviour before technology.
- Work will happen local-first before pushing coherent versions to GitHub.
- Cross-domain expansion is captured as a hypothesis, not a roadmap.

---

# Immediate Goal

Define precisely the first user, the first painful recurring decision, and the first domain.

Until that problem is crystal clear, no major technical decisions or expansion decisions should be made.

---

# Working Principle

Every discussion should improve one of these:

- the vision
- the product
- the technology
- the business model

If a conversation does not improve any of them, it probably does not belong in this repository.
