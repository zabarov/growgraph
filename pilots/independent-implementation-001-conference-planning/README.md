# Independent Implementation Pilot 001: Conference Planning

Status: pilot fixture

## Purpose

This pilot tests whether a valid GrowGraph package can be created using only
the public repository materials.

## Domain

Synthetic conference planning workflow.

No private company, customer, employee or internal project material is used.

## Research Question

Can a developer create a valid Level 1 GrowGraph package for a small workflow
using only public GrowGraph docs, schemas and examples?

## Files

- `graph-seed.json`
- `growgraph-package.json`
- `graph/objects.json`
- `graph/relations.json`
- `gates/results.json`
- `results/`
- `reports/pilot-report.md`

## Commands

Run from repository root:

```bash
node packages/cli/validate-growgraph.js seed pilots/independent-implementation-001-conference-planning/graph-seed.json
node packages/cli/validate-growgraph.js pilots/independent-implementation-001-conference-planning
node packages/cli/readiness-score.js pilots/independent-implementation-001-conference-planning --target-mode pilot
node packages/cli/context-pack.js pilots/independent-implementation-001-conference-planning --task-id task.prepare_speaker_schedule
```
