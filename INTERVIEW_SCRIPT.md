# Interview Script — Domain Discovery

> **Status:** notes / non-authorizing  
> Purpose: gather evidence for R0, R1, R2 and "why not LLM / existing tools" before choosing domain 1.  
> Use the **same core script** for both top candidates; only the opening and domain prompts change.

**Related:** `notes/DOMAIN_SCORECARD.md`, `docs/RISKS.md` (R0–R3), `CONTEXT.md`

---

## Goals (what this interview must answer)

| Risk / question | What you need to hear |
|-----------------|------------------------|
| **R0 — Value perception** | Is the pain strong enough that they would change behavior, or just complain? |
| **R1 — Frequency** | How often does this decision actually happen? |
| **R2 — Product shape** | Do they want a recommendation, a decision made for them, or a tool to decide? |
| **Workarounds** | What do they do today, step by step? |
| **Why not alternatives** | Partner, friends, Maps/Google, TikTok, general LLM — why those fail or "good enough" |
| **Session-1 value** | What would have helped *in that specific moment*? |
| **Return behavior** | Would they use help *next time*, not "is this a cool idea?" |

**Non-goals:** validate the PDE platform vision, Interest Graph, or multi-domain expansion. Do not pitch the company.

---

## Setup

### Who to recruit (start here)

| Domain track | Recruit people who… |
|--------------|---------------------|
| **A — Weeknight cooking** | Cook at home on weeknights at least 2×/week; ideally share decisions with a partner/family |
| **B — Restaurants** | Eat out or order decision-heavy meals with others at least 2×/month; ideally decide in a group/couple |

Aim for **5–8 interviews per track** before drawing conclusions. Friends-of-friends is fine. Prefer people outside the founding team’s bubble when possible.

### Format

- **20–30 minutes** (async voice note or live call both OK)
- **Record with permission**, or take structured notes in the template at the end
- **One domain per interview** — do not mix cooking and restaurants in the same session unless they naturally compare
- **Pay optional** small thank-you later if useful; not required for v1

### Rules for the interviewer

1. **Ask about the last real episode**, not hypotheticals. Prefer "last Tuesday" over "usually."
2. **Do not describe PDE** until the optional end section (or skip entirely).
3. **Do not sell.** If they ask what you’re building: *"We’re researching how people decide what to [cook / eat out]."*
4. **Sit in silence** after key answers; let them add detail.
5. **Capture exact phrases** for pain, workarounds, and "good enough."
6. **Separate opinion from behavior.** "I’d use that" is weak; "I texted three people and still ordered the usual" is strong.

---

## Script

### 0. Intro (1 min)

> Thanks for talking. This is research about everyday decisions — not a product demo. There are no right answers. I’ll ask about a recent time you had to choose something. OK to take notes / record?

Confirm domain track: **cooking** or **restaurants**.

---

### 1. Context (2 min)

*Warm-up; establishes lifestyle, not the product.*

- Tell me a bit about a normal weekday evening for you. Who’s around? How rushed is it?
- Who usually decides [what to cook / where to eat] in your household or group?

**Listen for:** decision owner vs negotiator; solo vs multi-person.

---

### 2. Last concrete episode (8–10 min) — most important section

*Force a specific story. This is the core of the interview.*

**Cooking track:**

> Think of the **last weeknight** when you had to figure out what to cook (or almost cooked and gave up). Walk me through it from the moment the question appeared.

**Restaurants track:**

> Think of the **last time** you had to figure out where to eat out (or order) with someone else. Walk me through it from the moment the question appeared.

**Prompts while they narrate (use only as needed):**

- When was this? What day/time?
- Where were you? Who else was involved?
- What constraints mattered (time, money, energy, diet, kids, location, weather)?
- What did you open, ask, or check? (apps, chat, fridge, Maps, LLM…)
- How long did the whole decision take, roughly?
- What did you end up doing?
- How did you feel during / after? (frustrated, fine, guilty, relieved…)
- Was that outcome "good enough" or did you regret it?

**If they stay abstract:**  
> Can you pick one specific night and tell it like a story?

**Listen for:** time cost, conflict, default-to-same-choice, delivery as escape hatch, who had veto power.

---

### 3. Frequency & pattern (3 min) — R1

- How often does a decision like that come up for you?
- Is it more often on certain days or situations?
- When it happens, is it usually a small annoyance or something that actually bothers you?
- In the last two weeks, how many times did this kind of friction show up? (help them count)

**Listen for:** daily / several× week / weekly / monthly. Push for counts, not adjectives.

---

### 4. Workarounds & alternatives (5 min)

*Map the competitive set they already "hire."*

- What do you normally do when this comes up?
- What tools or people have you tried? (partner, friends, Maps, Instagram/TikTok, recipe apps, Google, ChatGPT/Claude/Gemini, delivery apps…)
- Which of those works **well enough** that you don’t really need anything new?
- Which fails, and how?

**For each alternative they mention, ask:**

> What does it get wrong for you?

**Explicit LLM probe (always ask if not already covered):**

> Have you ever asked ChatGPT or another AI for help with this?  
> If yes: what happened? Would you do it again?  
> If no: why not?

**Explicit social probe:**

> How often does this turn into a negotiation with someone else? What usually breaks the deadlock?

**Listen for:** "good enough" incumbents; where general LLM is already winning; multi-person coordination pain.

---

### 5. Product shape (3 min) — R2

*Do not lead with PDE concepts. Offer concrete behaviors.*

> When this decision is hard, which of these would you actually want?

1. **Shortlist** — a few good options with tradeoffs, you still choose  
2. **Strong pick** — "do this one" with a short why; you can reject  
3. **Full decide for me** — just tell me what to do and I’ll mostly follow  
4. **Structure only** — help me ask the right questions / compare criteria; no real recommendation  

Follow-ups:

- Why that one?
- When would you *not* trust a strong pick?
- Would it matter if the suggestion came from AI, from friends’ taste, or from your own past choices?

**Listen for:** tool vs recommender vs decider; trust boundaries; social proof vs personalization.

---

### 6. Intensity & willingness (3 min) — R0

*Hard questions. Stay neutral.*

- On a scale of 0–10, how annoying was the last episode? (0 = nothing, 10 = seriously stressful)
- Have you ever searched for an app or system specifically to solve this?
- If something could cut that decision to under a minute and was usually right for you, what would need to be true for you to **use it the next time** the situation happens?
- What would make you **not** open it (too much setup, creepy, another app, wrong suggestions once…)?

**Optional behavioral ask (stronger than opinion):**

> If I manually helped you for two weeks — e.g. you text me when the decision starts and I reply with 2–3 options — would you actually text me on real nights? Why / why not?

**Listen for:** install/return barriers; setup intolerance; trust/creep; real willingness to change ritual.

---

### 7. Signal & learning (2 min) — early R3 / model loop

- After you [cook / go to a place], how do you know it was a good choice?
- Would you be willing to tap "good / meh / never again" afterward? When would that feel annoying?
- What would you be OK with a system remembering about you? What would feel like too much?

**Listen for:** natural feedback; privacy boundaries; single-domain trust.

---

### 8. Optional close — only if they ask what you’re doing (1–2 min)

Keep it vague:

> We’re exploring whether a simple helper for [weeknight cooking / choosing where to eat] is worth building — something that learns your constraints over time. Not selling anything today.

If useful:

> Can I follow up in a few weeks if we try a tiny manual version?

Thank them. Stop.

**Do not** pitch Personal Decision Engine, Interest Graph, multi-domain, or Super App ideas.

---

## Domain-specific prompt bank (optional deep dives)

Use only if time remains and the story was thin.

### Cooking

- How often do you default to the same 5 meals?
- How big a role does "what’s in the fridge/pantry" play vs "what we feel like"?
- Delivery / takeaway: is it a planned choice or an escape from indecision?
- Partner dynamics: who proposes, who vetoes?
- How long are you willing to cook on a weeknight?

### Restaurants

- Same-night vs planned earlier — which is more painful?
- How often is the problem "don’t know places" vs "can’t agree"?
- Maps ratings vs friends vs TikTok — which do you trust more?
- How far will you travel? Budget range?
- Dietary constraints or kids?

---

## Note-taking template (copy per interview)

```text
Date:
Interviewee (code name):
Domain track: cooking / restaurants
Duration:
Source (how recruited):

--- STORY (last episode) ---
When / who / where:
Constraints:
Steps taken (tools/people in order):
Time to decide:
Outcome:
Emotional tone (quotes):

--- R1 FREQUENCY ---
Stated frequency:
Count in last 2 weeks:
Pattern notes:

--- WORKAROUNDS ---
Primary workaround:
Other tools tried:
What is "good enough":
Where it fails (quotes):

--- LLM ---
Used AI for this? Y/N
What happened / why not:
Would use AI again? Y/N — why:

--- R2 SHAPE ---
Preferred: shortlist / strong pick / decide for me / structure only
Why:
Trust boundary:

--- R0 INTENSITY ---
Annoyance 0–10 (last episode):
Ever searched for a solution? Y/N
Would change behavior next time if…:
Would not use if…:
Concierge willingness: Y/N — why:

--- LEARNING / TRUST ---
How they judge a good outcome:
Feedback OK?:
OK to remember / not OK:

--- QUOTES WORTH KEEPING ---
1.
2.
3.

--- INTERVIEWER INTERPRETATION (label as opinion) ---
Evidence for / against this domain as wedge:
Open questions:
Surprise:
```

---

## After each interview (5 min debrief)

Answer in one short paragraph each:

1. **What evidence moved?** (R0 / R1 / R2 / LLM / workaround)
2. **Was this a real pain or polite agreement?**
3. **Scorecard impact:** which criteria (C1–C6 especially) would you change and why?
4. **Recruit next:** same segment, or a different one?

Log debriefs in `notes/EVIDENCE_LOG.md` (create when first interview is done) so beliefs accumulate outside chat history.

---

## How to use results (decision rules)

After **5–8 interviews per track**:

| Signal | Interpretation |
|--------|----------------|
| High frequency + high annoyance + weak workarounds + LLM not used or fails | Strong wedge candidate |
| High annoyance but monthly frequency | Possible product, wrong shape for weekly sensor thesis |
| Love the idea, no last-episode pain story | R0 failure — opinion without demand |
| Maps/TikTok/partner already "good enough" for most | Habit gap weak (C3); need narrower segment or other domain |
| LLM already solves it well for them | C6 weak; only continue if multi-person or structured memory is the clear gap |
| Prefer "decide for me" but reject wrong picks harshly | High trust bar; start as shortlist/tool |
| Will not do any setup or feedback | Learning-loop risk; session-1 must win almost alone |

**Do not choose domain 1 until both tracks have been heard**, unless one track is overwhelmingly stronger and the other clearly dead.

Then: fill the **forced wedge fields** in `DOMAIN_SCORECARD.md` for the winner and re-score with evidence.

---

## Changelog

| Date | Change |
|------|--------|
| 2026-07-23 | Initial script for cooking + restaurants discovery interviews |
