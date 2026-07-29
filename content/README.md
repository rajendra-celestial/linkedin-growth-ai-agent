# Content Archive

Every LinkedIn asset Claude produces for you lives here as plain markdown — no database, no app, just files you can read, edit, commit, and search.

| Folder | What goes here |
|---|---|
| `profile/` | Your saved profile analysis (`profile-analysis.md`) — niche, ICP, tone, positioning. Read by most other skills. |
| `daily/` | Daily posts, stories, educational posts, founder/sales posts, and most other single-post content types. |
| `weekly/` | Weekly recap posts. |
| `monthly/` | Monthly insights posts. |
| `ideas/` | Case studies, lessons learned, FAQs, mistakes, tips, frameworks, customer stories, newsletter ideas, podcast notes, calendar plans, trend research notes — anything that's a raw idea or reference before it becomes a finished post. |
| `drafts/` | Work-in-progress posts not yet ready for review. |
| `approved/` | Posts reviewed and approved, ready to schedule/publish. |
| `published/` | Posts you've confirmed are live on LinkedIn. Move a file here manually (or ask Claude to) once it's posted. |
| `carousel/` | Carousel outlines, individual slide copy, and infographic structures. |
| `videos/` | Video and Reel scripts. |
| `polls/` | Poll questions and options. |
| `comments/` | Comment ideas for engaging on other people's posts. |
| `cta/` | `cta-library.md` — the curated CTA reference. |
| `hooks/` | `hook-library.md` — the curated hook reference. |

## Conventions

- Generated posts are named `<YYYY-MM-DD>-<slug>.md`, e.g. `content/daily/2026-07-29-mistake-i-made-scaling.md`.
- Each post file starts with a short frontmatter block (`type`, `status`, `hashtags`, `keywords`, `createdAt`) followed by the full post text.
- Moving a post between folders (`drafts` → `approved` → `published`) is how you track its lifecycle — there's no separate status database.

See the skills in [.claude/skills/](../.claude/skills/) for how each type of content gets written here.
