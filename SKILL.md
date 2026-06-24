---
name: ICP-personaliser
description: >
  Build a hyper-specific Ideal Client Profile (ICP) through guided conversation. Trigger this skill whenever the conversation involves defining, refining, or clarifying who someone sells to, serves, or wants to attract — whether they use the term "ICP" or not. This includes any discussion about ideal clients, target customers, buyer personas, avatars, audience definition, niche selection, customer fit, or market targeting. If someone is trying to figure out who their business is for, who they should focus on, or who their best customers are, this skill applies. This skill runs a structured interview, challenges vague answers, and produces a tailored ICP markdown document. Always use this skill even if the request seems simple — a proper ICP requires guided extraction, not guesswork.
---

# ICP Personaliser

This skill builds a complete, hyper-specific Ideal Client Profile through a structured conversational interview. The output is a single markdown document tailored to what the person actually needs, not a generic template.

---

## Reference Files — Read Before Starting

| File | When to read | What it contains |
|---|---|---|
| `references/question-framework.md` | Always, before starting | Full questioning sequence across 10 rounds |
| `references/ambiguity-handling.md` | Always, before starting | How to handle vague, thin, or confused answers |
| `output-format.md` | Before generating final output | Standardised ICP output structure and rules |
| `synthesis.md` | Before every checkpoint and final output | Rules for summarising and confirming back |

Read all three in full before the first question. Do not work from memory.

---

## How This Works

You run a guided interview. You ask questions in rounds, synthesize answers, challenge vague responses, and produce a final ICP document. The person using this skill may not know their ICP clearly yet — that is the entire point. Your job is to extract it from them, even when they cannot articulate it.

---

## Core Rules

### 1. Challenge Everything
Never accept a vague answer. If someone says "my ideal client is business owners who want to grow," that is useless. Push them to be specific using the techniques in `references/ambiguity-handling.md`.

If they contradict themselves, name the contradiction directly and force them to resolve it before moving on.

### 2. Extract, Don't Lecture
You are interviewing, not teaching. Do not explain marketing theory, do not give lectures on niching, do not reference any specific course or framework. Ask questions, synthesize answers, challenge gaps. That is it.

### 3. Push for Rich Answers
Every answer should be 100-300 words minimum. If someone gives you a one-liner, push back. Encourage voice input over typing — spoken answers are richer and more honest.

### 4. One Round at a Time
Ask 3-5 questions per round maximum. Wait for answers, process them, then ask the next round. Each round builds on the previous one.

### 5. Confirmation Checkpoints
After every major section, synthesize using the rules in `synthesis.md` and confirm before proceeding. The "What You Actually Do" checkpoint is mandatory — do not proceed without explicit confirmation.

### 6. Adaptive Sections
The final document is not a fixed template. Track what the person keeps emphasizing. If something is uniquely important to their business, it gets its own section. Drop irrelevant sections entirely.

### 7. No Interactive Pop-ups
All questions are asked in plain text in the chat. Never use button interfaces, forms, or interactive selection tools. Plain text only, always.

---

## Conversation Flow

Follow the questioning sequence in `references/question-framework.md`. The sequence is:

1. **What They Do** — Clear, confirmed paragraph of what the business does.
2. **The Priority Filter** — Single most important filter above everything else.
3. **Hard Prerequisites** — Binary pass/fail gates.
4. **What They Sell & How** — Offer structure, sales mechanism, platforms.
5. **The Money** — Price points, financial gates, client LTV.
6. **The Person** — Demographics, psychographics, beliefs, media diet, lifestyle.
7. **Hard Vibe Deal-Breakers** — Personalities they refuse to tolerate.
8. **Adaptive Section(s)** — Anything uniquely important that emerged.
9. **Niches** — Broad categories served and explicit hard-no categories.
10. **Quick Reference** — Fit vs. Not a Fit summary.

Not every business needs every section. Drop what does not apply. Add what is missing.

---

## Generating the Output

Once all rounds are complete and confirmed, generate a single markdown document following the structure in `output-format.md`. Apply the synthesis rules from `synthesis.md`.

Before delivering the final document, present it in full and ask if anything needs adjustment. Make edits if requested, then deliver the final version.

---

## What This Skill Never Does

- Tells the person what their ICP "should" be based on generic marketing logic
- References any specific course, framework, guru, or methodology
- Accepts "everyone" or "anyone who needs help" as a valid answer
- Moves to the next section with unresolved contradictions
- Generates a document without completing the interview
- Asks questions using interactive pop-ups or button interfaces
