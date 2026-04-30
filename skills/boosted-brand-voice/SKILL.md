---
name: boosted-brand-voice
description: Apply, audit, or generate content using the Boosted.ai brand voice spec (v3.0.0). Use this skill whenever the user wants to write a LinkedIn post, tweet thread, blog post, email, or any external content as Boosted.ai; wants to check whether a draft conforms to the brand voice; asks about tone, word choice, naming, competitors, source tiers, or the voice rubric; or mentions the Informed Insider, brand voice, SKILL.md, or voice fidelity score. Also trigger when the user pastes a draft and asks "does this sound right?" or "review this."
user-invocable: true
---

# Boosted Brand Voice Skill

Apply the Boosted.ai brand voice to any content the user writes, reviews, or generates.

The full spec lives in `references/brand-voice-spec.md`. Read it at the start of every invocation — the rubric, hard-nos, and source tiers are the gates everything passes through before publish.

An HTML reference page is available at `references/index.html`.

---

## What to do when invoked

### If the user provides a draft to review

1. Read `references/brand-voice-spec.md`.
2. Score the draft against the rubric in §10:
   - 5 voice principles × 5 pts each (§2) — P1 specificity cannot score below 3
   - Channel format checks × 15 pts (§9)
   - Source / claim compliance × 10 pts (§8)
   - Hard-no check — pass/fail (§4); any fail = auto-block regardless of score
3. Return:
   - The score (e.g. "38 / 50 — human review queue")
   - Which gate it hits (auto-publish ≥40 / review queue 30–39 / auto-block <30 / hard-no override)
   - Specific line-level feedback for anything that lost points or tripped a hard-no
   - A revised version if the user asks for one

### If the user asks you to write content

1. Read `references/brand-voice-spec.md`.
2. Confirm the channel (LinkedIn, X/Twitter, blog, email, etc.) and audience (buyside, power retail, brokers) — ask if not clear.
3. Apply the correct modulation from §6 for that audience.
4. Follow channel format rules from §9 (word count, structure, links).
5. Enforce all hard-nos from §4.
6. Internally score the draft before returning it. If it scores below 40, revise until it clears the auto-publish gate (or explain why it can't and flag for human review).
7. Return the final draft with its score.

### If the user asks a question about the voice spec

Answer directly from `references/brand-voice-spec.md`. Cite the section number.

---

## Key rules to internalize (don't look these up every time)

- **Specificity is the only non-negotiable slider.** Everything else flexes by audience. Specificity never goes below 92.
- **Hard-nos are binary.** One hit = auto-block, no exceptions, no partial credit.
- **Byline rule.** AI-generated content never gets a personal human byline. Default: "Boosted Research."
- **Naming canon.** "Boosted.ai" not "Boosted" alone. "Alfa" not "alfa" or "ALFA." "Boosted Research" as house byline.
- **Competitor policy.** Name them only when the data demands it (regulatory filing, earnings). Never "Unlike X…" or comparison tables.
- **Source tiers.** T1 = cite freely. T0 = never as primary fact source.
