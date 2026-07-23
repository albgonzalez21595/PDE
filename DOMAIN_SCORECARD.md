# Domain Scorecard (scratch)

> **Status:** notes / non-authorizing  
> Written to support discovery of domain 1. This is not a roadmap and does not choose domain 1.  
> Scores are judgment calls for debate — update them after real user conversations.

**Related:** `CONTEXT.md`, `docs/RISKS.md` (R0–R3, R6), `docs/EXPANSION_HYPOTHESIS.md`, `docs/WORKING_BACKWARDS.md`

---

## Purpose

Force a comparable view of candidate first domains so the project can pick **who to interview and test first**, not which vertical PDE "is forever."

PDE remains the long-term vision (reduce decision friction by understanding the person).  
A domain is only a **wedge**: a concrete recurring decision used to validate demand, frequency, product shape, and learning loops.

---

## Scorecard criteria (0–2 each)

Higher = better **wedge for PDE discovery** at the current stage.

| # | Criterion | 0 | 1 | 2 |
|---|-----------|---|---|---|
| C1 | **Decision frequency** | Monthly or rarer | Weekly | Several times per week |
| C2 | **Pain intensity** | Mild annoyance | Real friction, still tolerable | High frustration / conflict / time sink |
| C3 | **Habit gap** | Strong incumbent "good enough" | Partial tools, still messy | No clean "pick for me" habit winner |
| C4 | **Session-1 value** | Needs weeks of data | Some value day 1 with light prefs | Clear value in &lt;2 min with minimal input |
| C5 | **Learning loop** | Hard to know if pick was good | Weak feedback | Natural outcome signal (cooked it, went, liked it) |
| C6 | **LLM weakness** | Chat alone is excellent | Chat helps but misses constraints | Needs private/local/multi-person/context chat lacks |
| C7 | **Standalone product (R3)** | Only valuable as sensor | Borderline | Users would want this even without "PDE" |
| C8 | **Trust / creep risk** | Feels surveillance-heavy early | Manageable with care | Feels helpful, not invasive |
| C9 | **Buildable part-time** | Heavy supply/ops/data | Medium | Concierge or thin slice feasible |
| C10 | **Optional near expansion** | Isolated dead-end | Weak adjacency | Natural near domain later (*not required for v1*) |
| C11 | **Monetization non-toxic** (light weight now) | Hard without killing trust | Plausible later | Natural affiliate/subscription fit |
| C12 | **Distribution surface** | Only cold App Store | Some share/trigger moments | Natural share, group, or recurring trigger |

**Max score:** 24

### How to weight at this stage

- Optimize for **C1–C7 and C9** first (demand, frequency, product shape, learning, LLM gap, standalone value, feasibility).
- Use **C10–C12** as tie-breakers only — not as permission to expand or monetize early.
- **Hard caution flags:**
  - If **C6 = 0** (general LLM already wins the job), weak wedge unless you have a sharp non-chat advantage.
  - If **C1 = 0** (too rare), misaligned with a weekly-retention / sensor thesis unless you deliberately want a low-frequency, high-ticket business shape.

### Open question to keep explicit

> Why would someone use this instead of a general LLM (with memory) for this decision?

Also compare against: partner/friends, Maps/Google, TikTok/Instagram, and the default habit ("the usual").

---

## Forced wedge fields (fill after interviews, per domain)

Do not treat a domain as "chosen" until these are specific enough to falsify:

1. **Who** — specific person, not "people who decide"
2. **When** — recurring trigger situation
3. **What decision** — one decision
4. **Frequency band** — and evidence it is realistic
5. **Current workaround** — exact behavior today
6. **Why workaround still fails**
7. **Session-1 promise** — value in under a minute
8. **Anti-scope** — what v1 will not do
9. **2–4 week success metric** — behavioral, not opinion

---

## Candidate domains (initial scores)

Scores below are **pre-interview hypotheses** (2026-07-23). Re-score after evidence.

### Leaderboard

| Rank | Domain | Score | Notes |
|------|--------|------:|-------|
| 1 | Weeknight cooking | 21 | Strongest frequency + constraints + learning + LLM gap |
| 2 | Restaurants / eat out | 20 | Strong social decision + monetization; heavy incumbents |
| 3 | Watch tonight | 16 | Easy to prototype; weaker stakes & incumbents |
| 4 | Gifting | 15 | Painful & monetizable; frequency wrong for weekly graph thesis |
| 5 | Weekend plans | 14 | Attractive vision; fuzzy job & supply-heavy |

---

### 1) Weeknight "what do we cook?" — **21 / 24**

Home cooking under time, pantry, and household taste constraints.

| Criterion | Score | Note |
|-----------|------:|------|
| C1 Frequency | 2 | Most nights for many households |
| C2 Pain | 2 | Time + indecision + partner negotiation |
| C3 Habit gap | 1 | Recipe apps exist; few solve *tonight with our constraints* |
| C4 Session-1 | 2 | Time + ingredients + "not pasta again" → useful fast |
| C5 Learning loop | 2 | Cooked / skipped / ordered out is clear |
| C6 LLM weakness | 2 | Pantry, household tastes, history, fatigue — chat is clumsy |
| C7 Standalone | 2 | Valuable without any platform story |
| C8 Trust | 2 | Low creep if single-domain |
| C9 Part-time | 2 | Concierge via chat/WhatsApp very doable |
| C10 Near expansion | 2 | Groceries, restaurants (taste transfer tests later) |
| C11 Monetization | 1 | Affiliates weak early; clear user value first |
| C12 Distribution | 1 | Daily trigger strong; viral share medium |

**Wedge hypothesis to test:** dual-income couples or families, ~6–8pm, 20–40 min cooking window.  
**Main risk:** content competition; must win on *decision under constraints*, not recipe library.  
**Why not LLM:** general chat does not reliably hold pantry, partner vetoes, "what we ate this week," or energy level without painful re-prompting.

---

### 2) "Where should we eat?" — **20 / 24**

Local restaurants / same-day going out.

| Criterion | Score | Note |
|-----------|------:|------|
| C1 Frequency | 1 | Often weekly, not daily for many |
| C2 Pain | 2 | Classic group indecision |
| C3 Habit gap | 1 | Maps / Google / TikTok strong |
| C4 Session-1 | 2 | Location + budget + cuisine + group size works fast |
| C5 Learning loop | 2 | Went / liked / would return |
| C6 LLM weakness | 1 | LLM + Maps already decent; local freshness hard |
| C7 Standalone | 2 | Clear product |
| C8 Trust | 2 | Familiar category |
| C9 Part-time | 1 | Needs solid local data quality |
| C10 Near expansion | 2 | Cooking, travel later |
| C11 Monetization | 2 | Affiliates / reservations more natural |
| C12 Distribution | 2 | Group decisions = shareable |

**Wedge hypothesis to test:** couples or friend groups deciding dinner out, same-night or same-day.  
**Main risk:** Google/Maps/TikTok incumbency; win via **group decision** or **taste memory**, not listings.  
**Why not LLM:** weak on live local quality, group veto resolution, and "places like the ones we actually loved last time" without structured history.

---

### 3) "What should we watch tonight?" — **16 / 24**

Movies / series for tonight, often multi-person one screen.

| Criterion | Score | Note |
|-----------|------:|------|
| C1 Frequency | 2 | High for many |
| C2 Pain | 1 | Real but often low stakes |
| C3 Habit gap | 1 | Netflix and peers already recommend |
| C4 Session-1 | 2 | Mood + time + available platforms |
| C5 Learning loop | 1 | Finished / abandoned is noisy |
| C6 LLM weakness | 1 | Chat is often good enough |
| C7 Standalone | 1 | Easy novelty; weak vs streaming UIs |
| C8 Trust | 2 | Low sensitivity |
| C9 Part-time | 2 | Easy to prototype |
| C10 Near expansion | 1 | Far from food; weak taste transfer |
| C11 Monetization | 1 | Hard; weak affiliates |
| C12 Distribution | 1 | Couple use possible |

**Main risk:** decision happens inside the streaming app; low willingness to open something else.  
**Only interesting if narrowed to:** multi-person taste conflict ("two people, one screen").

---

### 4) Gift / "what should I get them?" — **15 / 24**

Personal gifting under occasion + budget + recipient constraints.

| Criterion | Score | Note |
|-----------|------:|------|
| C1 Frequency | 0 | Spiky (birthdays, holidays) |
| C2 Pain | 2 | High anxiety; high willingness to get help |
| C3 Habit gap | 1 | Amazon / search / friends |
| C4 Session-1 | 2 | Recipient + budget + occasion works |
| C5 Learning loop | 1 | Gift reaction delayed / noisy |
| C6 LLM weakness | 1 | Chat already used heavily here |
| C7 Standalone | 2 | Clear job |
| C8 Trust | 1 | Recipient model can feel sensitive |
| C9 Part-time | 2 | Concierge works |
| C10 Near expansion | 1 | Commerce graph more than lifestyle graph |
| C11 Monetization | 2 | Affiliate native |
| C12 Distribution | 1 | Seasonal spikes |

**Main risk:** frequency kills weekly sensor / Interest Graph learning shape.  
**Fit:** possible different company shape (seasonal commerce helper); weak default for PDE thesis as stated.

---

### 5) "What should we do this weekend?" — **14 / 24**

Local plans / activities.

| Criterion | Score | Note |
|-----------|------:|------|
| C1 Frequency | 1 | Weekly-ish |
| C2 Pain | 2 | Planning fatigue, FOMO, couple conflict |
| C3 Habit gap | 1 | Instagram / friends / group chats dominate |
| C4 Session-1 | 1 | Needs local inventory + preferences |
| C5 Learning loop | 1 | Did it / liked it possible but laggy |
| C6 LLM weakness | 1 | Chat helps; local/events data is the edge |
| C7 Standalone | 1 | Broad, fuzzy job |
| C8 Trust | 1 | Location + social can feel heavier |
| C9 Part-time | 1 | Supply of local options is hard |
| C10 Near expansion | 1 | Sprawl risk (events, travel, food) |
| C11 Monetization | 1 | Tickets / affiliates possible |
| C12 Distribution | 2 | Inherently social |

**Main risk:** scope sponge — becomes a city guide.  
**Only viable if brutally narrowed** (e.g. couples in one city, Saturday afternoon, budget + indoor/outdoor).

---

## Working fork (not a decision yet)

| If you prioritize… | Lean toward |
|--------------------|-------------|
| Max frequency, learning loop, fairer fight vs LLMs | **Weeknight cooking** |
| Group dynamics, shareability, clearer money path later | **Restaurants** |
| Both at once | **Neither — that is expansion before R3** |

Do **not** pick domain 1 from scores alone. Use scores to choose **who to interview first**. Prefer the domain where people describe **last week’s specific failure**, not abstract agreement that "decisions are hard."

---

## Re-score log

| Date | What changed | Why |
|------|--------------|-----|
| 2026-07-23 | Initial scorecard + 5 candidates | Pre-interview baseline from strategy review |

---

## Next discovery use

1. Interview top 2 (cooking + restaurants) with the same script.  
2. After 5–8 conversations each, fill forced-wedge fields.  
3. Re-score C1–C6 from evidence, not opinion.  
4. Run one concierge test only for the winner.  
5. Keep this file in `notes/` until a domain is validated enough to promote a short summary into `CONTEXT.md` / `WORKING_BACKWARDS.md`.
