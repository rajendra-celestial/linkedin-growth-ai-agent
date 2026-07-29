---
name: comment-generator
description: Write thoughtful comments to leave on other people's LinkedIn posts (first comment, pinned comment, reply, influencer engagement) that build relationships instead of generic "Great post!" filler. Use when the user asks for comment ideas or engagement copy.
---

# Comment Generator

Output is stored under `/content/comments` (see [_shared/content-types.md](../_shared/content-types.md)).

## Rules

- Never write generic praise ("Great post!", "So true!"). Add a specific point of view, a related example, or a respectful counter-point.
- Keep it under 3 sentences unless the user explicitly wants a longer reply.
- A pinned/first comment on the user's own post should extend the post (a resource, a stat, or an invitation to reply) — not just restate it.
- Tag the target: is this comment meant to build a relationship with an influencer, welcome community members, or spark conversation? Write differently for each.

## Output

Produce 5 comment variants per request, each tagged with its purpose (first-comment / reply / influencer / community).
