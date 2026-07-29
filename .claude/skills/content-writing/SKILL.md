---
name: content-writing
description: Write a complete LinkedIn post (hook, body, CTA, hashtags, keywords) for a specific content type and topic. Use when the user asks to write, draft, or generate a LinkedIn post, carousel, poll, or script.
---

# Content Writing

See the content type catalog in [_shared/content-types.md](../_shared/content-types.md) for the full list of 39 types and guidance per type.

## Rules every post must follow

- First line is an attention hook (see `hook-generation` skill and [content/hooks/hook-library.md](../../../content/hooks/hook-library.md)) — never a generic opener.
- Body reads like a real person: concrete details, short paragraphs, line breaks for scannability, no "in today's fast-paced world" filler.
- Ends with one clear CTA (see [content/cta/cta-library.md](../../../content/cta/cta-library.md)).
- Include natural keyword usage for LinkedIn SEO (see `linkedin-seo` skill) without stuffing.
- Match the author's tone/writing style from `content/profile/profile-analysis.md`, if it exists.

## Steps

1. Confirm the content type and topic with the user.
2. Draft hook → body → CTA → 3-5 hashtags → 3-6 keywords.
3. Assemble the full post as `hook\n\nbody\n\ncta\n\n#hashtag1 #hashtag2 ...` and write it to the matching `/content/<folder>` subdirectory (see the catalog table) as a dated markdown file, e.g. `content/daily/2026-07-29-mistake-i-made-scaling.md`, with a short frontmatter block (`type`, `status`, `hashtags`, `keywords`, `createdAt`).
