# crashman79

Builder of practical Linux and Python tools for automation, audio workflows, and operational reliability.

[Website](https://crash-landing.net) | [SCUM DB](https://scum-db.com) | [Support on Ko-fi](https://ko-fi.com/crashman79)

## Portfolio Highlights

### SCUM DB
The largest project in my portfolio: a database of objects in the PC game SCUM.  Focused on parsing metadata from available game files and displaying this in a useful way to players.

- Live site: https://scum-db.com
- Focus: data organization, usability, and long-term maintainability

#### SCUM DB: Operations Snapshot
| Area | Snapshot |
|---|---|
| Pipeline stages | 5 stages: ingest -> validate -> normalize -> enrich -> publish |
| Automation actions | 7+ automated actions per update cycle (checks, build, deploy gates) |
| Runtime architecture | 3-tier model: edge delivery, app/API layer, data services |
| Reliability controls | 4 core controls: retries, health checks, job idempotency, alerting |
| Observability signals | 4 tracked signal groups: latency, errors, throughput, availability |

Behind the scenes, the platform uses staged processing, guarded releases, and monitored background jobs to keep updates consistent and dependable.

#### Pipeline Stages and Utility Script Groups

| Stage | Script group size | Collective operation |
|---|---|---|
| Ingest | 20+ scripts | Coordinate source checks, extraction indexing, seed loading, and run orchestration for new game data. |
| Validate | 15+ scripts | Run integrity checks, schema/relationship guards, confidence validation, and category consistency gates. |
| Normalize | 25+ scripts | Standardize records into canonical entities, consistent keys, and stable data types across item domains. |
| Enrich | 40+ scripts | Add relationships, metadata overlays, derived display/search fields, and domain-specific augmentations. |
| Publish | 10+ scripts | Apply transactional updates, refresh API-facing views, and propagate the latest dataset to user-facing endpoints. |

When a SCUM patch adds or changes items, this staged script flow processes the update end-to-end and publishes the refreshed dataset so API-backed pages and category views reflect the latest data.

### What I Build
- Linux automation and systems tooling
- Audio routing and workflow utilities
- Backend-powered apps with clear, practical interfaces

## Tech Stack Snapshot
Python | Linux | Shell | TypeScript | Web UI | API Integrations

## Private + Public Repo Stats
<!--STATS_START-->
### Snapshot

| Metric | Value |
|---|---:|
| Total Repos (Owned) | 16 |
| Public Repos | 5 |
| Private Repos | 11 |
| Followers | 1 |
| Following | 1 |
| Commit Contributions | 181 |
| PR Contributions | 1 |
| Issue Contributions | 3 |
| Repositories Contributed To | 8 |
| Private Contribution Events (restricted) | 0 |

_Last updated: 2026-04-17T14:00:54.945Z_
<!--STATS_END-->

## GitHub Dashboard
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=crashman79&show_icons=true&include_all_commits=true&count_private=true&rank_icon=github)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=crashman79&layout=compact&langs_count=8)

## Support
If my work is useful to you, support helps me keep building and maintaining these projects.

- Ko-fi: https://ko-fi.com/crashman79
