# Contributing

This is a Claude Code skills package — there's no build, no install, no dependencies. Contributing means editing markdown.

## Adding or improving a skill

1. Create (or edit) `.claude/skills/<skill-name>/SKILL.md` with `name` and `description` frontmatter. The description is what Claude Code matches against user requests, so make it specific about *when* to use the skill.
2. Ground instructions in the actual repo: link to [.claude/skills/_shared/content-types.md](.claude/skills/_shared/content-types.md), [content/hooks/hook-library.md](content/hooks/hook-library.md), [content/cta/cta-library.md](content/cta/cta-library.md), or other skills rather than repeating their content.
3. Keep it actionable: numbered steps and concrete rules, not generic marketing advice Claude already knows.

## Adding a new content type

1. Add a row to the table in `.claude/skills/_shared/content-types.md` (guidance + target `/content` subfolder).
2. If it needs its own dedicated skill (rather than being covered by `content-writing`), add one following the pattern above.

## Growing the hook/CTA libraries

Add new entries to `content/hooks/hook-library.md` or `content/cta/cta-library.md` under the matching category. Prefer promoting hooks/CTAs that a user reports actually performed well over inventing more generic ones.

## Reporting bugs / requesting features

Use the issue templates in `.github/ISSUE_TEMPLATE/`.
