---

name: startup-idea-validator


description: "Validate startup, app, or business ideas via a structured, research-backed framework: problem strength, market sizing (TAM/SAM/SOM), competition, go-to-market feasibility, and business model viability — grounded in live web research on market data, competitors, and trends. Produces a Validation Report: 1-5 scorecard, riskiest assumptions, a cheapest-test recommendation, and a Go/Conditional Go/Pivot/No-Go verdict. MANDATORY TRIGGERS: 'validate this idea', 'validate my startup idea', 'pressure-test/stress-test this business idea', 'idea validation', 'is this a viable business'. STRONG TRIGGERS: 'is there a market for X', 'would people pay for X', 'should I build this', 'what do you think of this business idea', 'evaluate this idea'. Use whenever someone describes a startup/product concept and wants honest viability feedback. Do NOT trigger for: naming, pitch decks/marketing copy, legal/incorporation, fundraising mechanics, or pure technical 'how do I build X' questions."

---

# Startup Idea Validator

Founders are bad judges of their own ideas — not because they're foolish, but because they're close to the problem and emotionally invested in the solution. This skill gives an idea the kind of outside, evidence-grounded scrutiny a sharp advisor would apply: it frames the idea precisely, checks it against real market data, scores it across the dimensions that actually determine startup outcomes, and ends with one clear verdict and one concrete next step — not twenty.

The goal is not to crush ideas for sport, and not to be encouraging for its own sake. The goal is to be **right**, and to say so plainly either way.

---

## When to run a validation

**Good validation requests** — a described business/product concept where the user wants to know if it's worth pursuing:
- "Validate this idea: a subscription box for..."
- "Is there a market for an app that helps freelancers..."
- "I'm thinking of building [X]. Tear it apart."
- "Would people actually pay for this?"
- "Here's my business concept — what do you think?"

**Not validation requests** — redirect or just answer directly:
- "Help me name my startup" (naming task)
- "Write a pitch deck for this idea" (creation task — though validation could reasonably precede it; ask if they want both)
- "How do I incorporate an LLC?" (legal/admin)
- "How do I build a waitlist page in React?" (pure technical task)

If the idea is extremely thin (a single word, no problem or customer implied — e.g. "an app for dogs"), ask **one** clarifying question to get enough to frame it, rather than guessing wildly.

---

## The five scored dimensions

Every idea gets scored 1-5 on each of these. The scores aren't decoration — they drive the final verdict, so take them seriously and justify each one with a specific reason tied to research or reasoning, not vibes.

**Scoring rubric (applies to all five dimensions):**

| Score | Meaning |
|---|---|
| 1 | Major red flag — this alone could sink the idea as currently framed |
| 2 | Weak — a real, unresolved concern that needs to change before this works |
| 3 | Mixed — workable, but with open questions that matter |
| 4 | Strong — solid foundation, only minor gaps |
| 5 | Exceptional — a genuine structural advantage on this dimension |

### 1. Problem Strength
Is this solving a "painkiller" (urgent, frequent, expensive problem people actively try to solve today) or a "vitamin" (nice-to-have, low urgency)? Look for evidence that people currently spend time, money, or painful workarounds on this problem. A 5 here means the problem is acute and the current alternatives are visibly bad. A 1 means the "problem" is mostly hypothetical or already solved well enough that nobody's looking for alternatives.

### 2. Market Size & Timing
How big is the addressable market, and why is now a good (or bad) time? This requires research — don't estimate from priors alone. A 5 means a large, growing market with a credible "why now" (a technology shift, regulatory change, behavior shift, or cost collapse that makes this newly possible or newly necessary). A 1 means the market is tiny, shrinking, or the "why now" doesn't hold up.

### 3. Competitive Landscape & Differentiation
Who else is solving this, how, and why would a customer switch to (or choose) this instead? A crowded market isn't automatically bad (it can validate demand) but it raises the bar for differentiation. A 5 means a clear, defensible wedge against real alternatives. A 1 means well-funded incumbents already do this well and the proposed differentiation is cosmetic.

### 4. Go-to-Market Feasibility
Can the target customer actually be reached, and is the path from "doesn't know this exists" to "paying customer" realistic given likely resources? A 5 means there's an identifiable, reachable channel (a community, a platform, a sales motion) that fits the product and price point. A 1 means the GTM plan amounts to "go viral" or requires enterprise sales with no enterprise relationships.

### 5. Business Model & Unit Economics
Does the way this makes money make sense given what it costs to deliver and to acquire a customer? A 5 means the pricing, margins, and acquisition cost plausibly work even at modest scale. A 1 means the economics only work at a scale that's implausible, or the pricing model doesn't match how the target customer actually buys things.

---

## How a validation session works

### Step 1 — Frame the idea

Extract (or ask for, if missing) four things:
1. **Target customer** — specifically, not "everyone"
2. **The problem** — what pain, and how acute/frequent is it
3. **The proposed solution** — what it actually does
4. **The business model** — how it makes money

Write a one-line framing using this template, and show it to the user as the first thing in the report so they can confirm you understood correctly:

> For **[target customer]** who **[problem/pain]**, **[product/company]** is a **[category]** that **[key benefit]**. Unlike **[main current alternative]**, it **[differentiator]**.

If you genuinely can't fill in 2+ of these four elements even with reasonable inference, ask **one** clarifying question before proceeding. Otherwise, state your assumptions explicitly in the framing and move on — don't stall the analysis on minor ambiguity.

### Step 2 — Market research (live web search)

This is what separates real validation from a confident-sounding opinion. Before scoring anything, run **4-8 targeted searches** (scale with how niche/well-known the space is) covering:

- **Market size**: search for the category's market size and growth rate (e.g. "[industry/category] market size", "[category] market growth"). Look for TAM figures and, if possible, narrow toward a SAM (the slice actually reachable by this product) and an SOM (realistic share in 2-3 years).
- **Competitors**: search for existing players solving this or an adjacent problem (e.g. "[problem] software", "[category] alternatives", "[specific tool name] competitors" if the user named one). Identify 2-4 real competitors or close substitutes — including "do nothing" or a manual/spreadsheet workaround if that's the realistic alternative.
- **Timing / trends**: search for what's changed recently in this space (e.g. "[category] trends 2026", recent funding or product launches, regulatory changes, technology shifts). This is where "why now" gets either confirmed or punctured.
- **Pricing signals**: if competitors were found, a quick check of their pricing pages gives a sanity check for the business model dimension.

Follow the standard search hygiene: short, specific queries (1-6 words), start broad then narrow, use `web_fetch` on the 1-3 most relevant results for real detail rather than relying on snippets. Treat any market-size figures as **directional estimates from secondary sources**, and say so in the report — don't present a single number as gospel.

### Step 3 — Score the five dimensions

For each dimension, give the 1-5 score and a tight (2-4 sentence) justification that explicitly references something from the research where relevant. Resist the pull toward the middle — a 3 should mean genuinely mixed evidence, not "I don't want to commit."

### Step 4 — Riskiest assumptions (Mom Test style)

Identify the **top 3 assumptions** that, if false, would unravel the idea — these are usually different from the five scored dimensions; they're the specific unknowns that the scoring couldn't resolve from research alone (because they depend on facts about this specific founder's execution, this specific customer segment's behavior, etc.).

For each assumption, suggest 1-2 questions the founder should ask **real prospective customers**, following Rob Fitzpatrick's "Mom Test" principle: ask about specific past behavior and money/time already spent, not hypothetical future intentions. "Would you use this?" produces polite lies. "Walk me through the last time you ran into this problem — what did you do?" produces signal.

Bad question: *"Would you pay $20/month for a tool that does X?"*
Good question: *"What do you currently use to handle X? What does that cost you — in money, time, or workarounds?"*

### Step 5 — The cheapest test

Propose **one** concrete, scrappy, low-cost experiment that would meaningfully move the needle on the single riskiest assumption — ideally something runnable in under a week for under a few hundred dollars. Be specific: name the channel, the audience, the artifact (landing page, concierge MVP, a dozen customer conversations, a pre-sell), and what result would count as a real signal versus noise. Avoid generic advice like "do customer interviews" without saying who, how many, and what you're listening for.

### Step 6 — The verdict

Average the five scores (each 1-5) and map to a verdict:

| Average | Verdict |
|---|---|
| 4.0 – 5.0 | **Strong Go** — the fundamentals are sound; focus on execution |
| 3.0 – 3.9 | **Conditional Go** — promising, but validate the riskiest assumptions before building |
| 2.0 – 2.9 | **Significant Pivot Needed** — one or more dimensions has a structural problem that needs to change |
| 1.0 – 1.9 | **No-Go as currently framed** — the core premise doesn't hold up against the evidence |

The verdict should never just restate the average — explain *why*, and if one dimension is so weak it overrides an otherwise decent average (e.g. a 5/5 product idea with a 1/5 "incumbents already own this and have no reason to lose"), say so explicitly. The chairman-style judgment matters more than the arithmetic.

---

## Output format

Present the full report directly in the conversation using markdown. Structure it as:

```
# Startup Idea Validation: {short idea name}

## The Idea, As Understood
{one-line framing using the template from Step 1}

## TL;DR Verdict
{1-2 sentences: the verdict, the score, and the single biggest reason why}

## Market Research Findings

### Market Size & Timing
{TAM/SAM/SOM estimates with sources, framed as directional. Why-now analysis.}

### Competitive Landscape
{2-4 real competitors/alternatives, what they do, how this would differ}

## Validation Scorecard

| Dimension | Score | Why |
|---|---|---|
| Problem Strength | X/5 | {1-2 sentence justification} |
| Market Size & Timing | X/5 | {1-2 sentence justification} |
| Competitive Landscape & Differentiation | X/5 | {1-2 sentence justification} |
| Go-to-Market Feasibility | X/5 | {1-2 sentence justification} |
| Business Model & Unit Economics | X/5 | {1-2 sentence justification} |
| **Average** | **X.X/5** | |

## Riskiest Assumptions
1. **{assumption}** — {why it's risky}. Ask real customers: *"{Mom Test-style question}"*
2. **{assumption}** — ...
3. **{assumption}** — ...

## The Cheapest Test
{one specific, concrete experiment — channel, audience, artifact, success signal}

## The Verdict
{Go / Conditional Go / Pivot Needed / No-Go, with reasoning that goes beyond the average}
```

If a visualization tool is available and would help (e.g. a quick bar chart of the five scores), it can be a nice addition — but the markdown report must stand on its own without it. If the user wants to keep or share the report, offer to save it as a file (e.g. a Markdown or Word document).

---

## Example (abbreviated)

**User:** "Validate this idea: an app that uses AI to automatically split restaurant bills based on what each person actually ordered, by scanning the receipt."

**The Idea, As Understood:** For *groups of friends splitting restaurant bills*, who *waste time and create awkwardness manually itemizing who-owes-what*, **ReceiptSplit** is a *mobile app* that *scans a receipt and auto-calculates each person's share including tax/tip*. Unlike *manual mental math or generic bill-splitting apps that split evenly*, it *itemizes automatically from the actual receipt*.

*(Research would then check: market size for bill-splitting/payment apps, existing players like Splitwise, Venmo's built-in splitting, Tab, etc., and recent trends in receipt-scanning/OCR + payments integration.)*

**Scorecard (illustrative):**

| Dimension | Score | Why |
|---|---|---|
| Problem Strength | 3/5 | Real but minor annoyance, not acute — most groups tolerate rough splitting or "I'll get it next time" |
| Market Size & Timing | 3/5 | Bill-splitting is a large but already-served market; no strong "why now" beyond OCR being commoditized |
| Competitive Landscape | 2/5 | Splitwise and Venmo already cover 80% of the use case for free; itemization is a feature, not a product |
| Go-to-Market | 2/5 | No obvious viral mechanism beyond "friend group adopts it together," which is a hard cold-start |
| Business Model | 2/5 | Hard to charge for something incumbents offer free as a feature |
| **Average** | **2.4/5** | |

**Verdict:** Significant Pivot Needed. The itemization mechanic is genuinely useful, but it's a *feature* of an existing app's value proposition, not a standalone product. The strongest path forward isn't a new app — it's either a feature pitch/partnership with an existing player, or a pivot toward a use case where itemized splitting is the *primary* job (e.g. expense reports for small teams, where the stakes and frequency are higher).

---

## Important notes

- **Earn the verdict, don't default to it.** Don't be a contrarian for its own sake, and don't be encouraging for its own sake. If the research genuinely supports a Strong Go, say so clearly — but only after the framework, not instead of it.
- **Cite sources** for market data and competitor claims, following normal citation practice — and be explicit when a figure is a rough estimate from a secondary source rather than a precise number.
- **One verdict, one cheapest test.** The most common failure mode for this kind of analysis is burying the user in 15 action items. Resist that. The riskiest-assumptions list (max 3) and the single cheapest test are the actionable core.
- **This is an informed outside perspective, not investment, legal, or financial advice.** Frame it that way if the user seems to be treating the verdict as a final word — real validation ultimately comes from talking to real customers, which the riskiest-assumptions section points toward.
- **Don't skip research even if the idea sounds familiar.** A confident-sounding take based on priors alone is exactly the failure mode this skill exists to avoid. If search results are thin or conflicting, say so rather than papering over the gap.
