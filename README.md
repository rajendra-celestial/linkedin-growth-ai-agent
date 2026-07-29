# LinkedIn Growth AI Agent

A Claude Code skills package that turns Claude into a LinkedIn ghostwriter and growth strategist. No app to run, no API key to manage, no database to set up — just skills Claude reads during your conversation, and a plain-markdown content archive it reads and writes to.

Prepared by [rajendragupta.xyz](https://rajendragupta.xyz) and [celestialitverse.com](https://celestialitverse.com).

## How it works

1. Open this folder in Claude Code.
2. Talk to Claude naturally: *"analyse my LinkedIn profile"*, *"write me an educational post about hiring your first AI engineer"*, *"build me a 30-day content calendar"*, *"give me 5 comment ideas for this post"*.
3. Claude matches your request to the right skill in `.claude/skills/` and follows its instructions.
4. Generated content is written to the `/content` archive as dated markdown files — readable, editable, git-friendly.

## What's included

- **Profile analysis** — headline, About, experience, skills, company/products → niche, ICP, authority level, tone, writing style, positioning, content pillars.
- **Content writing** — 39 content types (daily posts, stories, carousels, polls, case studies, thought leadership, video/reel scripts, and more), each with a hook, body, CTA, hashtags, and SEO keywords. Full catalog in [.claude/skills/_shared/content-types.md](.claude/skills/_shared/content-types.md).
- **Content calendar** — 30/90/365-day plans with themed rotation.
- **Hook & CTA libraries** — [content/hooks/hook-library.md](content/hooks/hook-library.md) and [content/cta/cta-library.md](content/cta/cta-library.md), curated and meant to grow over time.
- **22 Claude Code skills** — see the full list in [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md).

## Project structure

```
.claude/skills/          22 skills + a shared content-type reference
content/                 The archive: profile analysis, posts by lifecycle stage, hook/CTA libraries
docs/                    Architecture and roadmap
```

## Documentation

- [Architecture](docs/ARCHITECTURE.md)
- [Roadmap](docs/ROADMAP.md) — including what was deliberately left out and why
- [Content archive guide](content/README.md)
- [Contributing](CONTRIBUTING.md)

## Credits

Prepared by [rajendragupta.xyz](https://rajendragupta.xyz) and [celestialitverse.com](https://celestialitverse.com).

## License

MIT — see [LICENSE](LICENSE).
