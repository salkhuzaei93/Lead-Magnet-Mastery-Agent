# How to Deploy This Agent in a Claude Project

## What Is a Claude Project?

A Claude Project is a persistent workspace inside Claude.ai that holds:
- A **system prompt** (called "Instructions") that defines the agent's behavior
- A **Knowledge base** of uploaded files the agent can reference in every conversation
- A shared conversation history if you're working in a team

This agent is designed specifically for Claude Projects. The system prompt tells Claude *how to behave*. The uploaded skill files tell Claude *what to do and how to do it*. Both are required.

---

## Step 1 — Create the Project

1. Go to [claude.ai](https://claude.ai)
2. In the left sidebar, click **"New Project"**
3. Name it: **Lead Magnet Mastery Agent** (or any name you prefer)
4. Click **Create**

---

## Step 2 — Paste the System Prompt

1. Inside your new project, click **"Edit project details"** or the settings/pencil icon
2. Find the **"Instructions"** field (this is the system prompt)
3. Open `AGENT_INSTRUCTIONS.md` from this folder
4. Copy the **entire contents** and paste into the Instructions field
5. Save

This defines how the agent behaves: its role, its enforcement rules, its sequencing gates, its output standards.

---

## Step 3 — Upload the Knowledge Files

This is the most important step. The agent cannot execute skills it cannot read.

In the Project, find the **"Add content"** or **"Knowledge"** section and upload files.

**Upload in this order (priority order if there are file limits):**

### Tier 1 — Must Upload (Core Execution Files)
These are the files the agent reads during every skill execution:

```
phase-01-market-intelligence/01.01-awareness-level-diagnosis/SKILL.md
phase-01-market-intelligence/01.02-dominant-emotion-mapping/SKILL.md
phase-01-market-intelligence/01.03-conversation-archaeology/SKILL.md
phase-01-market-intelligence/01.04-desire-stratification/SKILL.md
phase-01-market-intelligence/01.05-competitive-intelligence/SKILL.md
phase-01-market-intelligence/01.06-psychographic-profiling/SKILL.md
phase-02-strategic-architecture/02.01-one-big-promise/SKILL.md
phase-02-strategic-architecture/02.02-specificity-engineering/SKILL.md
phase-02-strategic-architecture/02.03-value-to-friction-ratio/SKILL.md
phase-02-strategic-architecture/02.04-format-selection-science/SKILL.md
phase-02-strategic-architecture/02.05-bridge-architecture/SKILL.md
phase-02-strategic-architecture/02.06-consumption-design/SKILL.md
phase-02-strategic-architecture/02.07-quick-win-architecture/SKILL.md
phase-02-strategic-architecture/02.08-scarcity-of-information-framing/SKILL.md
```

That is 14 files. Upload all 14.

### Tier 2 — Strongly Recommended (Reference Files)
The agent loads these when it needs deeper theory or worked examples:

```
phase-01-market-intelligence/01.01-awareness-level-diagnosis/references/schwartz-awareness-levels.md
phase-01-market-intelligence/01.02-dominant-emotion-mapping/references/collier-emotional-frameworks.md
phase-01-market-intelligence/01.03-conversation-archaeology/references/halbert-mining-techniques.md
phase-01-market-intelligence/01.04-desire-stratification/references/schwartz-desire-architecture.md
phase-01-market-intelligence/01.05-competitive-intelligence/references/kennedy-positioning-principles.md
phase-01-market-intelligence/01.06-psychographic-profiling/references/ogilvy-portrait-method.md
phase-02-strategic-architecture/02.01-one-big-promise/references/hopkins-promise-principles.md
phase-02-strategic-architecture/02.02-specificity-engineering/references/caples-specificity-evidence.md
phase-02-strategic-architecture/02.03-value-to-friction-ratio/references/kennedy-value-friction-framework.md
phase-02-strategic-architecture/02.04-format-selection-science/references/sugarman-format-psychology.md
phase-02-strategic-architecture/02.05-bridge-architecture/references/kern-bridge-methodology.md
phase-02-strategic-architecture/02.06-consumption-design/references/bencivenga-reading-psychology.md
phase-02-strategic-architecture/02.08-scarcity-of-information-framing/references/hopkins-scarcity-methodology.md
```

### Tier 3 — Operational Tools (Scripts and Assets)
Upload these if you want the agent to produce filled worksheets and templates:

```
phase-01-market-intelligence/01.03-conversation-archaeology/scripts/reddit-search-queries.md
phase-01-market-intelligence/01.05-competitive-intelligence/scripts/competitor-audit-template.md
phase-01-market-intelligence/01.06-psychographic-profiling/assets/prospect-portrait-blank.md
phase-02-strategic-architecture/02.01-one-big-promise/scripts/promise-drafting-worksheet.md
phase-02-strategic-architecture/02.02-specificity-engineering/scripts/vagueness-audit-checklist.md
phase-02-strategic-architecture/02.03-value-to-friction-ratio/scripts/value-friction-calculator.md
phase-02-strategic-architecture/02.04-format-selection-science/assets/format-decision-matrix.md
phase-02-strategic-architecture/02.05-bridge-architecture/scripts/bridge-design-worksheet.md
```

### Tier 4 — Optional (Navigation Docs)
```
INDEX.md
QUICK_START.md
```

**Total files: up to 35.** Claude Projects support up to 50 files, so you can upload everything.

---

## Step 4 — Test the Setup

Start a new conversation inside the project and type:

> "I want to build a lead magnet. My market is [describe your market]. Let's start."

The agent should:
1. Ask for your market, the specific problem, and the paid offer
2. Begin with Skill 01.01 — Awareness Level Diagnosis
3. Ask you the 7 diagnostic questions for awareness level

If it does this, the project is configured correctly.

---

## Step 5 — Running a Full Project

A complete Phase 01 + Phase 02 run takes **3–6 hours of conversation time** depending on how much market research you bring in vs. how much the agent needs to elicit from you.

**Option A — Agent-led (you answer questions, agent synthesizes):**
Tell the agent your market and let it ask you questions to complete each skill. Best when you know your market well but haven't formalized the research.

**Option B — Research-first (you bring data, agent processes it):**
Gather raw data first — Reddit threads, competitor opt-in pages, Amazon reviews, client interviews — paste it into the conversation, and let the agent process it through the skills. Faster and produces higher-fidelity outputs.

**Option C — Hybrid:**
Complete Phase 01 through conversation, then bring structured research for Phase 02 where specific data (competitor analysis, VOM language) produces better outputs than answers to questions alone.

---

## How the Agent Uses the Knowledge Files

When you ask the agent to run a skill, it:
1. Reads the relevant SKILL.md from its knowledge base
2. Confirms the required inputs are present in the conversation
3. Executes the skill step-by-step, following the instructions exactly
4. Produces the output in the exact template format
5. Signals the next skill

The reference files (e.g., `schwartz-awareness-levels.md`) are consulted when the agent needs to apply nuanced theory — for example, when a market situation is ambiguous and the deeper framework context helps it diagnose correctly.

The script and asset files (e.g., `value-friction-calculator.md`) are used when the agent is filling out a scoring tool, running an audit, or producing a worksheet for you to complete.

---

## One Project Per Lead Magnet

Each lead magnet project should be its own Claude Project (or a long, continuous conversation within one project). The 14 output artifacts from Phases 01–02 accumulate over the conversation and feed each other. Starting a new project with fresh context clears all the Phase 01 intelligence.

If you are building multiple lead magnets for the same market, you can run Phase 01 once (the market intelligence does not change) and run Phase 02 multiple times for different lead magnets within the same conversation.

---

## Adding Phase 03–06 Skills

When Phase 03 skills are completed, you will:
1. Receive the new SKILL.md files
2. Upload them to the same project as Tier 1 files
3. Update the AGENT_INSTRUCTIONS.md with the Phase 03 sequencing rules
4. Re-paste the updated Instructions into the project

The project expands as the skill library expands. No restructuring required.

---

## Troubleshooting

**"The agent is not following the skill steps"**
The SKILL.md files may not have uploaded correctly. Go to the Knowledge section, confirm all 14 SKILL.md files are present, and try again. You can also paste the SKILL.md content directly into the conversation as context.

**"The agent skipped a skill and went straight to writing copy"**
The sequencing enforcement in the system prompt was overridden by a strong user request. Restart and be explicit: "Follow the skill sequence strictly. Do not write copy until Phase 02 is complete."

**"The outputs are too short / not matching the templates"**
Ask explicitly: "Produce the full [Skill Name] output using the exact template format from the SKILL.md." The agent sometimes summarizes when it should fill the template.

**"I want to use the agent for a different market on the same project"**
Start a new conversation within the same project (not a new project). The instructions and knowledge files persist. The conversation history does not carry over between conversations, which is what you want — clean context for a new market.
