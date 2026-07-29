# Architecture

There is no app, server, or database here. This repository is a **Claude Code skills package**: a set of instructions Claude reads and follows during a conversation, plus a plain-file archive Claude reads and writes to as it works.

```mermaid
flowchart TD
    U[You, in a Claude Code conversation] -->|"analyse my profile" / "write a post" / etc.| C[Claude]
    C -->|reads| S[".claude/skills/*/SKILL.md"]
    C -->|reads/writes| CONTENT["/content/** (profile, posts, hooks, CTAs, calendar)"]
    C -->|reads| SHARED[".claude/skills/_shared/content-types.md"]
```

## Why this shape

- **No backend**: Claude Code already *is* the LLM. Standing up a separate app with its own AI provider key and database would duplicate what Claude Code provides for free, and would require you to manage infrastructure just to run a set of writing instructions.
- **Skills over prompts**: each `.claude/skills/<name>/SKILL.md` is a focused, reusable instruction set with `name`/`description` frontmatter so Claude Code can find and load the right one automatically based on what you ask for (e.g. asking to "write a post" triggers `content-writing`; asking "what's my niche" triggers `profile-analysis`).
- **Files over a database**: `/content` is the single source of truth. Profile analysis, generated posts, the hook/CTA libraries, and calendar plans are all markdown — readable without any tool, diffable in git, and portable to any other system (Notion, Sheets, a future app) without a migration.
- **Shared reference over duplication**: `.claude/skills/_shared/content-types.md` holds the content-type catalog (39 types → guidance → `/content` folder) once, so every skill that needs it links to the same source instead of repeating (and drifting from) its own copy.

## Layout

```
.claude/skills/
  _shared/content-types.md   Content type catalog + folder mapping (shared reference)
  profile-analysis/          Analyse a LinkedIn profile → niche, ICP, tone, positioning
  content-strategy/          Turn profile analysis into content pillars + cadence
  content-writing/           Write a complete post (hook, body, CTA, hashtags, keywords)
  hook-generation/           Generate/curate scroll-stopping hooks
  headline-generator/        LinkedIn headline options
  comment-generator/         Comments for other people's posts
  hashtag-generator/         3-5 relevant hashtags per post
  trend-research/            Surface current trends for TRENDING_TOPIC/AI_NEWS posts
  competitor-analysis/       Competitor positioning + content gaps
  lead-generation/           Persona-targeted content with a soft conversion path
  personal-branding/         Consistency check against stated positioning
  linkedin-seo/              Keyword placement for LinkedIn search
  geo-optimisation/          Structuring content for AI answer engines
  audience-research/         Who's actually engaging, and what they ask
  content-calendar/          30/90/365-day calendar plans
  content-repurposing/       Turn one asset into multiple LinkedIn formats
  newsletter-writer/         Newsletter editions / teaser posts
  dm-writer/                 Direct message copy
  connection-request-writer/ Connection request notes (<300 chars)
  cold-outreach/             First-touch outreach messages
  sales-posts/               Soft-sell posts
  thought-leadership/        Opinionated, authority-building posts

content/                     The archive — see content/README.md
docs/                        This file + ROADMAP.md
```

## Not implemented (by design)

A hosted web app with its own AI provider integration and Postgres database was considered and explicitly ruled out for this package — see [docs/ROADMAP.md](ROADMAP.md) if that's ever wanted as a *separate* product later.
