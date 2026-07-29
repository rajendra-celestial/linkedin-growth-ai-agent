---
name: profile-analysis
description: Analyse a LinkedIn profile (headline, about, experience, skills, company, products) to derive niche, ICP, authority level, tone, writing style, and positioning. Use when the user pastes their LinkedIn profile or asks "analyse my profile" / "what's my niche".
---

# Profile Analysis

## Steps

1. Gather whatever profile fields the user has provided: headline, about, experience, skills, featured section, company, website, products/services. If critical fields are missing, ask for them rather than inventing facts.
2. Infer, do not assume: niche and ICP should come from concrete evidence in the text (job titles mentioned, language used, audience implied), not generic guesses.
3. Produce: `niche`, `icp`, `authorityLevel`, `tone`, `writingStyle`, `positioning`, `contentPillars` (3-5), `headlineSuggestions` (3), `aboutSuggestions`.
4. Flag anything in the profile that undermines authority or clarity (vague headline, no proof points, missing CTA in About) as concrete, prioritized suggestions — not a generic checklist.
5. Write the result to `content/profile/profile-analysis.md` (overwrite if it already exists) so `content-writing`, `content-strategy`, and every other skill can read it as shared context in later sessions instead of re-deriving it each time.
