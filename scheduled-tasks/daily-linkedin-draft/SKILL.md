---
name: daily-linkedin-draft
description: Generate a daily LinkedIn post draft for Boosted.ai and publish it to Notion for team review
---

You are generating a daily LinkedIn post draft for Boosted.ai (the company) / Alfa (the product). Your job is to produce one publish-ready draft, decide on the right visual format for it, source or describe that asset, and create a Notion page for the team to review. This task runs fully headlessly — no browser required.

## Step 1 — Read brand and content guidelines

Fetch these Notion pages:
- AI-Driven Social Marketing Engine: https://www.notion.so/AI-Driven-Social-Marketing-Engine-34f448cd498a8164b91be91e2c0b7778
- What Good Looks Like: https://www.notion.so/What-Good-Looks-Like-Boosted-ai-Content-Standards-351448cd498a81bd9a5cca6a64fa0535
- Brand Guidelines: https://www.notion.so/351448cd498a81b69a39d66b4d69e089

Key rules:
- Company: Boosted.ai. Product: Alfa. Never "Boosted", "ALFA", or "alfa"
- No emojis, no em-dashes, no banned words (unpacking, cutting-edge, game-changer, innovative, seamless, unlock, leverage as verb, actionable insights, disruption, empower)
- No "it's worth noting", "that being said", numbered lists
- Voice: analyst-to-analyst. Insightful, Reliable, Modern, Genuine
- End every post with a question
- Links go in first comment, not post body
- Target: ~150 words

## Step 2 — Read the video asset library

Fetch the Alfa Video Asset Library: https://www.notion.so/357448cd498a81c182e2fc6ea2a2428c

This lists all existing use-case videos with titles, taglines, time saved, and what post types they suit.

## Step 3 — Find today's market news

Search for today's top financial market news — earnings, Fed activity, macro data, analyst calls, AI-in-finance developments. Find 2-3 stories relevant to buy-side analysts, PMs, and heads of research.

## Step 4 — Write the post

Choose the content type that best fits today's context:
- **Data/insight post** — market observation, specific and measurable
- **Product post** — Alfa in action, shown through output not described
- **Thought leadership** — AI in research, fee compression, coverage gaps

The post must:
- Open with a specific, uncomfortable truth or data point — not a question, not "I"
- Connect to a pain the ICP already feels
- Show rather than tell
- End with a genuine question
- Sound like a sharp analyst wrote it, not a marketing team
- Be under 150 words

Also write:
- One-sentence rationale for why this angle today
- One alternative hook (first line only)

## Step 5 — Choose the visual format

Not every post needs a visual. Not every visual should be a video. Choose the format that best serves the post — variance across the week is intentional and good.

**Use this logic to decide:**

**Video** — best when the whole point is showing a workflow transformation (before → after). Use for product posts where motion and speed are the message. Match to the asset library (Step 2). If no existing video fits, generate a new HTML draft (see below).

**Product screenshot** — best when the post references a specific Alfa output (a scorecard, a research brief, a screening result, a transcript summary). The screenshot shows the real deliverable. In the Notion draft, describe exactly what screen to capture: which Alfa feature, what query to run, what the output should look like. Be specific enough that someone can reproduce it in the product.

**Text only** — best for thought leadership and contrarian takes where the argument is the content and a visual would dilute it. Also use when no video or screenshot would genuinely add information — decoration is worse than nothing.

**Rough rotation to aim for across the week:**
- 2x video
- 2x screenshot
- 1x text only

**If video — existing asset:**
Match to the asset library. Include folder slug, title, why it fits, and export instructions.

**If video — new asset needed:**
Generate a self-contained HTML animation file using the Boosted.ai visual system:
- Background: #080808, font: Hanken Grotesk + JetBrains Mono, accent: gold
- 5-scene arc: SceneTitle → SceneProblem → SceneIngest → SceneWhatChanged → SceneCTA
- 30 seconds, square aspect ratio
- Show the painful manual before, then Alfa handling it in seconds, then a clean output
- Save to: /Users/alexlemay/Downloads/alfa-[slug]-draft.html
- Note in draft: "New video draft saved — open file, review, export as MP4 when ready"

**If screenshot:**
Write a precise brief for whoever will capture it:
- Which Alfa feature or workflow to open
- What query or input to use (be specific — name a real ticker, sector, or theme relevant to today's post)
- What the output should show
- Any crop or annotation notes

**If text only:**
Write "Text only — no visual needed" with a one-line reason.

## Step 6 — Create the Notion draft page

Create a new child page under: https://www.notion.so/AI-Driven-Social-Marketing-Engine-34f448cd498a8164b91be91e2c0b7778

Title: "LinkedIn Draft — [Today's date]"

Sections:
1. **Post Draft** — full text, ready to copy-paste
2. **Content Type** — data/insight, product, or thought leadership
3. **Visual Format** — Video / Screenshot / Text only, then the full asset brief (see Step 5)
4. **Why This Angle** — one-sentence rationale
5. **Alternative Hook** — alternate first line
6. **News Context** — 2-3 bullet points on today's market news
7. **Notes for Reviewer** — time-sensitivity, anything flagged

## Success criteria
- Notion page created with today's date
- Post under 150 words, brand-compliant, ends with a question
- Visual format decision is always present and always justified
- Entire task runs without needing Chrome or a browser