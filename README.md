# crashman79

Builder of practical Linux and Python tools for automation, audio workflows, and operational reliability.

[Website](https://crash-landing.net) | [SCUM DB](https://scum-db.com) | [Support on Ko-fi](https://ko-fi.com/crashman79)

## Portfolio Highlights

### SCUM DB
My largest project: a data platform for SCUM game objects, metadata, and lookup workflows.

- **Live site**: https://scum-db.com
- **Focus**: reliable ingestion, clean categorization, and fast player-facing search for the SCUM survival game

#### Pipeline Overview
The SCUM DB pipeline processes game data from extraction through player-facing publication using a modular script-based pipeline (run via `scripts/run_pipeline_v3.py`). The pipeline uses a dependency DAG to orchestrate script execution across multiple waves of parallel processing.

The workflow covers the full data lifecycle: initializing the items database, extracting properties from game assets, discovering and categorizing game objects, classifying items into types (weapons, clothing, consumables, etc.), enriching with derived data (confidence scores, variant groups, display categories), and publishing results for API and site consumption.

Script counts per rough phase: 20+ discovery scripts, 25+ classification scripts, 40+ enrichment scripts, 10+ publish/post-processing scripts. The dependency resolution ensures proper ordering, with parallel wave execution available in v3.

Operational model: automated updates, staged processing with dependency resolution, and monitored release flow.

### What I Build

| Area | What I deliver |
|---|---|
| Linux and automation | System tooling, process orchestration, and reliability-focused utilities |
| Audio workflows | PipeWire/PulseAudio routing tools and quality-of-life automation |
| Data-backed apps | Backend + API integrations with practical, user-friendly interfaces |

### Project Style
- Small focused utilities that do one job well
- Production-minded scripts with observability and recovery paths
- Clear operator workflows over complex setup

### Tech Stack
Python | Linux | Shell | TypeScript | Web UI | API Integrations

## GitHub Overview

### Repo Stats Snapshot
<!--STATS_START-->
### Snapshot

| Metric | Value |
|---|---:|
| Total Repos (Owned) | 21 |
| Public Repos | 5 |
| Private Repos | 16 |
| Followers | 0 |
| Following | 1 |
| Commit Contributions | 371 |
| PR Contributions | 2 |
| Issue Contributions | 0 |
| Repositories Contributed To | 10 |
| Private Contribution Events (restricted) | 0 |

_Last updated: 2026-09-14T08:09:20.051Z_
<!--STATS_END-->

### Project Highlights

- **SCUM DB**: Comprehensive SCUM game data platform — from PAK extraction through player-facing searchable database
- Pipeline processes 100+ game object categories via modular scripts with dependency DAG orchestration
- Script coverage across extraction, discovery, classification, enrichment, and publish stages
- Designed for reliable player-facing search and metadata lookup, with automated 6-hour update cycle

## Support

If my work is useful to you, support helps me keep building and maintaining these projects.

- Ko-fi: https://ko-fi.com/crashman79