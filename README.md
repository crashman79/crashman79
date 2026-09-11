# crashman79

Builder of practical Linux and Python tools for automation, audio workflows, and operational reliability.

[Website](https://crash-landing.net) | [SCUM DB](https://scum-db.com) | [Support on Ko-fi](https://ko-fi.com/crashman79)

## Portfolio Highlights

### SCUM DB
My largest project: a data platform for SCUM game objects, metadata, and lookup workflows.

- **Live site**: https://scum-db.com
- **Focus**: reliable ingestion, clean categorization, and fast player-facing search for the SCUM survival game

#### Pipeline Overview
The SCUM DB pipeline processes game data from extraction through player-facing publication. The modular script-based pipeline (run via `scripts/run_pipeline_v3.py`) consists of several coordinated stages:

- **Seed**: Initialize the items database from extraction output (`seed_validated_items.py`)
- **Extract**: Pull properties and metadata from game asset files (`extract_properties.py`, `extract_vehicle_specs.py`)
- **Discover**: Identify and categorize game objects — vehicles, buildables, ammunition, weapons, attachments, deconstruction recipes, and more
- **Classify**: Assign items to categories (melee/range weapons, clothing, consumables, equipment, materials, books, others, fortifications) using rule-based classification
- **Enrich**: Add derived data — confidence scores, variant groups, display categories, nutrition/cooking data, medical properties, vehicle part enrichment, and DLC integration
- **Publish**: Generate search documents, variant mappings, compatibility tables, and make data available via the API and site

Script counts per rough phase: 20+ discovery scripts, 25+ classification scripts, 40+ enrichment scripts, 10+ publish/post-processing scripts. The pipeline uses a dependency DAG (`scripts/utilities/pipeline_dependencies.py`) to ensure proper ordering, with parallel wave execution available in v3.

Operational model: automated updates (driven by the 6-hour game update timer on `sdbext`), staged processing with dependency resolution, and monitored release flow (blue/green deployments via Next.js/Express).

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

| Metric | Value |
|---|---:|
| Total Repos (Owned) | 21 |
| Public Repos | 5 |
| Private Repos | 16 |
| Followers | 0 |
| Following | 1 |
| Commit Contributions | 363 |
| PR Contributions | 1 |
| Issue Contributions | 0 |
| Repositories Contributed To | 10 |

*Data reflects all repositories under this GitHub account.*

<!--STATS_END-->

### Project Highlights

- **SCUM DB**: Comprehensive SCUM game data platform — from PAK extraction through player-facing searchable database
- Pipeline processes 100+ game object categories via modular scripts with dependency DAG orchestration
- Script coverage across extraction, discovery, classification, enrichment, and publish stages
- Designed for reliable player-facing search and metadata lookup, with automated 6-hour update cycle

## Support

If my work is useful to you, support helps me keep building and maintaining these projects.

- Ko-fi: https://ko-fi.com/crashman79