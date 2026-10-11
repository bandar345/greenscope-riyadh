# GreenScope Riyadh 🌳

**An AI-Based Decision Support Platform for Monitoring and Prioritizing Urban Vegetation Enhancement in Riyadh**

IS 498 Graduation Project · Project No. 15 · Department of Information Systems · CCIS · King Saud University · Fall 2026–27 (1448H)

| | |
|---|---|
| Supervisor | Dr. Abdulaziz Almaslukh |
| Team | **بذرة (Bathra)** |
| Members | Bandar Alshahrani (@bandar345) · Faisal (@FaisalMym) · Mohammed Alkahtani (@Mohammedk05) |

## What the platform does
1. Measures vegetation cover per Riyadh neighbourhood from satellite imagery (Sentinel-2 / Dynamic World).
2. Combines vegetation, population density (WorldPop) and land-surface temperature (Landsat) into a weighted priority score.
3. Estimates the cooling impact of added vegetation with a machine-learning model.
4. Tracks change over successive snapshots against Green Riyadh targets.

## Repository structure
```
docs/        Proposal, report chapters, meeting log, risks, Gantt
design/      Diagrams (use case, ERD, architecture), UI mockups
research/    Literature table, data-source table, interview needs (no names)
ai-log/      AI usage disclosure log (Handbook §9.3 / Appendix B)
notebooks/   Earth Engine & analysis notebooks
src/         Platform source code
data/        Small samples only — large data is NOT committed (see data/README.md)
```

## How we work
See [CONTRIBUTING.md](CONTRIBUTING.md) — every task is an Issue, every change goes through a branch and a Pull Request.

.
