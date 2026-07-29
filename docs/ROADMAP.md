# Roadmap

## Shipped

- 22 Claude Code skills covering profile analysis, content strategy, writing (39 content types), hook/CTA generation, headlines, comments, hashtags, trend research, competitor analysis, lead generation, personal branding, LinkedIn SEO, GEO optimisation, audience research, content calendars, repurposing, newsletters, DMs, connection requests, cold outreach, sales posts, and thought leadership.
- A curated hook library (`content/hooks/hook-library.md`) and CTA library (`content/cta/cta-library.md`), organized by category, meant to grow over time as posts perform well.
- A plain-file `/content` archive with a defined folder-per-lifecycle-stage convention (`drafts` → `approved` → `published`).

## Explicitly not built

These were part of the original brief but don't belong in a Claude Code skills package — they require infrastructure this package intentionally doesn't have:

- **Direct LinkedIn publishing/scheduling** — needs LinkedIn Marketing API access + OAuth + a running scheduler process.
- **Live trend/news discovery** — needs an integration to a search or news API; can be approximated in a Claude Code session using web search if the environment provides it, but isn't automated/scheduled here.
- **Automated analytics ingestion** — needs LinkedIn API access to pull real follower/engagement numbers; you'd report numbers to Claude manually today.
- **Notion / Google Sheets / Slack / Discord / Telegram / webhook integrations** — these make sense for a always-on service, not a conversational tool.
- **A hosted dashboard UI** — if you want a always-on, no-Claude-Code-required product with a login and a database, that's a genuinely different project (a small Next.js + Postgres app), not an extension of this skills package. Worth scoping separately if/when you need it — it doesn't belong bundled in here by default.

## Possible next steps for this package

- [ ] Add a `virality-scoring` skill that reasons about a draft's likely performance using known LinkedIn engagement heuristics (purely advisory — no real data).
- [ ] Add a `content-audit` skill that reviews everything in `content/published/` for pillar/tone consistency over time.
- [ ] Expand the hook/CTA libraries as real posts get published and reported back.
