---
name: headline-generator
description: Write LinkedIn headline options that combine role, value proposition, ICP, and keywords for profile SEO. Use when the user asks to improve or generate their LinkedIn headline.
---

# Headline Generator

## Formula

`[Role/Identity] | [Who you help] [outcome you deliver] | [Proof point or keyword]`

## Steps

1. Pull niche, ICP, and positioning from the profile analysis (`profile-analysis` skill / `Profile` model).
2. Generate 3-5 headline variants under 220 characters, each leading with the strongest keyword for LinkedIn search (LinkedIn indexes headlines heavily for people-search).
3. Avoid empty buzzwords ("passionate", "guru", "ninja"). Prefer concrete nouns and numbers.
4. Output should be usable as-is for `profileAnalysis.headlineSuggestions`.
