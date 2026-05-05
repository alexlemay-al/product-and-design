# product-and-design

Resources, skills, and scheduled tasks for Boosted.ai's product and design workflows.

## Scheduled Tasks

### `daily-linkedin-draft`

Runs every day at 9am ET. Generates a LinkedIn post draft for Boosted.ai / Alfa and publishes it to Notion for team review.

**What it does:**
- Reads brand guidelines and content strategy from Notion
- Pulls today's top financial market news
- Writes a post in Boosted.ai's brand voice (~150 words, analyst-to-analyst)
- Chooses the right visual format (video, product screenshot, or text only)
- Matches to the Alfa use-case video library or generates a new HTML video draft
- Creates a Notion draft page under the AI-Driven Social Marketing Engine

**To install this task in your own Claude Code:**
1. Copy `scheduled-tasks/daily-linkedin-draft/SKILL.md` to `~/.claude/scheduled-tasks/daily-linkedin-draft/SKILL.md`
2. Open Claude Code and go to the Scheduled section in the sidebar
3. The task will appear — set it to run at 9am ET

**Output lands here:** [AI-Driven Social Marketing Engine](https://www.notion.so/AI-Driven-Social-Marketing-Engine-34f448cd498a8164b91be91e2c0b7778) in Notion.
