# 2026-06-20 Dynamic Widgets Refresh

Presentation upgrade of the profile README. Text content (about, research
interests, experience) was preserved; only the visual presentation and the
explicitly requested facts changed.

Changes:

- Removed the hand-drawn pencil-sketch banner (`banner.png`).
- Retired the self-hosted `lowlighter/metrics` system: deleted
  `.github/workflows/metrics.yml` and the committed SVGs (`github-metrics.svg`,
  `metrics.plugin.habits.svg`, `metrics.plugin.languages.svg`).
- Switched to live hotlinked GitHub widgets (academic, restrained styling):
  - github-readme-stats stats card + top-languages (the ability chart).
  - streak-stats contribution streak.
  - github-readme-activity-graph contribution graph (the commit graph).
  - skillicons.dev tech-stack icon row.
  - shields.io contact badges + komarev profile-views counter.
  - All stat cards use `<picture>` + `prefers-color-scheme` so they stay legible
    in both GitHub light and dark mode.
- Updated schools: removed the "incoming at OSU / ASU" list; the user is
  transferring to the University of Minnesota Twin Cities, College of Science
  and Engineering (CSE). Added an Education entry — B.S. (Transfer), Computer
  Science & Electrical Engineering double major, Sep 2026 - Present — and
  annotated the TU Delft x TU/e entry as ending in 2026 on transfer.

Factual boundary preserved: all widgets render real GitHub data; no invented
affiliations, dates, publications, awards, metrics, or endorsements.

Note: dynamic widgets depend on third-party services (Vercel / Heroku / demolab)
and can occasionally rate-limit or 5xx; this is the accepted trade-off for the
fully dynamic model.
