---
name: awareness-level-diagnosis
description: Diagnoses the exact awareness level of a target market using Eugene Schwartz's 5-level framework, then outputs a strategic brief that determines the correct entry angle, language register, and promise framing for a lead magnet. Use this skill before writing any copy, headlines, or offers — running it first is mandatory for any lead magnet project.
metadata:
  author: lead-magnet-agent
  version: "1.0"
  framework: Eugene Schwartz — Breakthrough Advertising (1966)
  phase: "01 — Market Intelligence"
  skill-number: "01.01"
---

# Awareness Level Diagnosis

## Purpose

Every lead magnet fails or succeeds at the awareness level. Writing a product-aware headline to an unaware market is the single most common and most fatal mistake in direct response marketing. This skill forces a disciplined diagnosis BEFORE any copy is written.

The output of this skill is a **Strategic Awareness Brief** — a single document that determines:
- Which of the 5 levels your market currently occupies
- What they already know, believe, and feel
- What the first sentence of your opt-in page must do
- Which copy angle and promise structure to use

---

## The 5 Levels of Awareness (Schwartz)

| Level | Label | What the prospect knows |
|-------|-------|------------------------|
| 1 | **Unaware** | Does not know they have the problem |
| 2 | **Problem Aware** | Knows the problem, does not know solutions exist |
| 3 | **Solution Aware** | Knows solutions exist, does not know your specific method |
| 4 | **Product Aware** | Knows your method/offer, not yet convinced |
| 5 | **Most Aware** | Knows you, trusts you, just needs the right deal |

---

## Step-by-Step Diagnosis Process

### Step 1 — Gather Market Inputs

Ask the user to provide (or research yourself if not given):

1. **The market/niche** — e.g. "online coaches selling $5k programs"
2. **The specific problem the lead magnet solves** — e.g. "not getting enough qualified leads from Instagram"
3. **The traffic source** — e.g. cold Facebook ads, warm YouTube audience, existing email list, organic search
4. **Any known competitor lead magnets in this space** — names, angles, formats if available

If traffic source is not provided, ask before proceeding. Traffic source is the single biggest determinant of awareness level.

### Step 2 — Apply the Traffic Source Heuristic

Use this as your starting hypothesis before deeper analysis:

| Traffic Source | Default Starting Level |
|---------------|----------------------|
| Cold paid social (Facebook, TikTok, Instagram ads) | Level 1–2 |
| Cold Google/YouTube ads | Level 2–3 |
| Organic SEO (informational keywords) | Level 2–3 |
| Organic SEO (solution/product keywords) | Level 3–4 |
| Warm retargeting audience | Level 3–4 |
| Existing email list or community | Level 4–5 |
| Referral from known authority | Level 3–4 |

### Step 3 — Refine with the 7 Diagnostic Questions

Score each question to confirm or adjust the starting hypothesis. Answer based on what a typical member of this market would say if asked:

**Q1 — Problem Recognition**
> "Do they wake up consciously aware that [specific problem] is costing them something?"
- No → Level 1 signal
- Sometimes / vaguely → Level 2 signal
- Yes, clearly → Level 2+ confirmed

**Q2 — Solution Category Awareness**
> "Do they know that a category of solution (courses, tools, methods, services) exists for this problem?"
- No → Level 1–2
- Yes, generically → Level 3
- Yes, and they've tried some → Level 3–4

**Q3 — Sophistication Signal**
> "Have they already been marketed to heavily in this niche?"
- No → Lower sophistication, lower awareness
- Yes, frequently → Higher sophistication — they're skeptical and harder to impress
- Very saturated market → Must differentiate mechanism, not just promise

**Q4 — Language They Use**
> "What exact words do they use when describing their problem to a friend?"
- Vague, emotional language ("I'm stuck", "nothing is working") → Level 1–2
- Problem-specific language ("my conversion rate is low", "I can't get leads") → Level 2–3
- Solution-specific language ("I need a better funnel", "looking for a VSL template") → Level 3–4
- Brand/method-specific language ("thinking about [your offer]") → Level 4–5

**Q5 — Google Search Behavior**
> "What would they type into Google about this problem right now?"
- Symptom searches ("why am I not making money online") → Level 1–2
- Problem searches ("how to get more clients as a coach") → Level 2–3
- Solution searches ("best lead magnet for coaches") → Level 3–4
- Product searches ("[your name] review" / "[your offer] pricing") → Level 4–5

**Q6 — Emotional State**
> "What is the dominant emotion they associate with this problem?"
- Confusion or unawareness → Level 1
- Frustration and vague dissatisfaction → Level 2
- Hope mixed with skepticism → Level 3
- Informed skepticism, comparison-shopping mindset → Level 4
- Trust and readiness → Level 5

**Q7 — Proof Requirement**
> "How much proof do they need before they'll act?"
- Very little — they're in pain and want any solution → Level 2
- Moderate — need to see that the mechanism works → Level 3
- High — need to be convinced YOUR version beats alternatives → Level 4
- Minimal — they already trust you → Level 5

### Step 4 — Assign the Final Awareness Level

Tally your signals from Steps 2 and 3. The most frequently indicated level is your diagnosis. If signals split evenly between two adjacent levels, default to the LOWER level — it is always safer to assume less awareness than more.

**Do not blend levels.** A lead magnet written to "Level 2–3" speaks to no one clearly. Pick one.

### Step 5 — Generate the Strategic Awareness Brief

Output the following structured brief:

```
STRATEGIC AWARENESS BRIEF
─────────────────────────────────────────
Market: [market name]
Traffic Source: [source]
Diagnosed Awareness Level: [1 / 2 / 3 / 4 / 5]
Level Label: [Unaware / Problem Aware / Solution Aware / Product Aware / Most Aware]

WHAT THEY ALREADY KNOW:
[2–3 sentences describing what this market can be assumed to know before encountering your lead magnet]

WHAT THEY DO NOT YET KNOW:
[What they are missing that your lead magnet will reveal]

DOMINANT EMOTION RIGHT NOW:
[Single most prevalent emotion in this market regarding this problem]

LANGUAGE THEY USE:
[3–5 verbatim phrases or sentence patterns typical of this market]

─────────────────────────────────────────
COPY ANGLE PRESCRIBED:
[The specific entry angle the opt-in page must use — see Reference Guide]

HEADLINE FRAME PRESCRIBED:
[The structural pattern the headline must follow — see Reference Guide]

PROMISE STRUCTURE PRESCRIBED:
[How bold and how specific the promise can be at this awareness level]

WHAT TO AVOID:
[The specific assumption or language pattern that would alienate this market]
─────────────────────────────────────────
```

---

## Copy Angles by Awareness Level

These are the prescribed entry angles for each level. Deviating from these without strong justification will reduce conversion.

**Level 1 — Unaware**
Open with a story, provocative statement, or pattern interrupt that surfaces a problem they have but haven't named. Never mention your solution in the headline. The job of the entire opt-in page is to make them feel the problem, not sell the solution.
> Headline pattern: "Why [symptom they're experiencing] is actually a sign of [problem they don't know they have]"

**Level 2 — Problem Aware**
Open by naming the problem with surgical precision and emotional accuracy. Show them you understand exactly how it feels. Then present the existence of a solution — not yet your specific solution.
> Headline pattern: "Finally: A [solution category] that actually solves [specific problem] for [specific identity]"

**Level 3 — Solution Aware**
Open by differentiating your mechanism. They know solutions exist — now they need a reason to believe yours is different. Lead with the unique mechanism or the unique result.
> Headline pattern: "How to [desirable outcome] using [unique mechanism] — without [common frustration with other solutions]"

**Level 4 — Product Aware**
Open with proof, urgency, or a compelling reason to act now rather than later. They know what you offer — they need conviction and a trigger.
> Headline pattern: "[Specific result] in [specific timeframe] — here's exactly how [proof element]"

**Level 5 — Most Aware**
Get out of the way. Short copy, clear offer, strong CTA. They trust you — over-explaining kills the conversion.
> Headline pattern: "[Offer name] — [brief benefit statement]. Get it free."

---

## Edge Cases & Common Errors

**"My traffic is mixed"**
Diagnose the awareness level of the COLD portion of your traffic. Your page must convert cold traffic — warm leads will convert regardless of copy quality.

**"The market is very sophisticated / saturated"**
High sophistication does NOT mean high awareness. A sophisticated Level 2 market has heard many promises and believes none of them. Dial specificity to maximum and proof requirement to maximum. The angle shifts but the awareness level stays Level 2.

**"I'm not running paid ads yet"**
Default to Level 2 for all planning purposes. Better to over-explain to a warm audience than to under-explain to a cold one.

**"It's an organic post, not an ad"**
The platform context matters more than the format. Organic TikTok/Instagram = cold Level 1–2 audience unless you have an established following. Organic from an email list = Level 4–5.

---

## Handoff to Next Skills

Once this brief is complete, it becomes the mandatory input for:
- **Skill 01.02** — Dominant Resident Emotion Mapping (emotion confirmed here is deepened there)
- **Skill 03.01** — Headline Architecture (prescribed headline frame from this brief is used directly)
- **Skill 03.07** — The Reason Why (the "why free" argument must match the awareness level)

Do not proceed to any copy skill without a completed Strategic Awareness Brief.

---

See [references/schwartz-awareness-levels.md](references/schwartz-awareness-levels.md) for extended examples and a worked case study.
