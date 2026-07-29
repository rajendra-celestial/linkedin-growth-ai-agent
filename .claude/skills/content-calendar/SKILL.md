---
name: content-calendar
description: Build a 30/90/365-day LinkedIn content calendar with themes and content types per day. Use when the user asks for a content calendar or posting schedule.
---

# Content Calendar

Uses the content type catalog in [_shared/content-types.md](../_shared/content-types.md).

## Steps

1. Confirm horizon: 30, 90, or 365 days, and start date.
2. Use the content-strategy pillars (see `content-strategy` skill) to weight the rotation — don't just cycle content types evenly if one pillar matters more.
3. Each entry needs: date, theme (human-readable), and a content type. Avoid scheduling the same content type on consecutive days.
4. For longer horizons (90/365), group into weekly/monthly themes so the plan reads as a narrative, not a random grid.
5. Write the plan as a markdown table to `content/ideas/calendar-<horizon>-<start-date>.md` (date, theme, content type per row) so `content-writing` can be asked to fulfill each date in later sessions.
