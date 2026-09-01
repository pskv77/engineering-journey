# Sprint 00 — Learning Infrastructure

Status: Completed after final documentation review

Start: August 2026

Formalization: September 2026

## Purpose

Sprint 0 exists to create the engineering learning system before structured technical learning begins.

This sprint is different from later two-week technical sprints.

Its objective is not primarily to increase technical ranks.

Its objective is to establish:

- an accurate starting point;
- a repeatable Git workflow;
- a documented roadmap;
- a skill measurement system;
- assessment storage;
- a HomeLab specification;
- a structure for future practical work.

# Inputs

The main input was Assessment Week completed in August 2026.

Seven areas were assessed:

1. Computer Science Fundamentals
2. Programming & Automation
3. Linux & Systems
4. Networks & Network Security
5. Windows & Enterprise Infrastructure
6. Cybersecurity Engineering
7. DevOps, Cloud & Infrastructure Security

The results established Baseline v1.0.

# Completed work

## Git and GitHub

Completed:

- Git identity configured;
- GitHub SSH authentication verified;
- private engineering repository created;
- repository structure established;
- branch-based workflow practiced;
- commits created;
- pull requests reviewed;
- changes merged into `main`;
- stale branches cleaned up;
- macOS `.DS_Store` files excluded through `.gitignore`.

## Repository architecture

Created major areas for:

- documentation;
- baseline;
- roadmap;
- skills;
- retrospectives;
- assessments;
- sprints;
- labs;
- projects;
- courses;
- HomeLab.

## Baseline archive

Original Assessment Week artifacts were archived under:

    assessments/baseline-2026-08/

The archive contains:

- seven assessment documents;
- assessment tracker versions;
- final Assessment Week tracker.

Baseline interpretation is documented separately under:

    docs/baseline/

## Skill system

Created:

- 0–5 independence-based rank model;
- confidence model;
- learning-state classification;
- initial skills matrix;
- evidence-based rank update rules.

## Roadmap

Created Roadmap v1.0 including:

- Phase I;
- Sprint 1–6;
- continuous networking track;
- continuous security track;
- parallel PowerShell track;
- external-course integration;
- Comprehensive Control #1;
- broad future phases.

## Learning rules

Documented operating rules covering:

- theory / practice balance;
- cumulative learning;
- Git usage;
- labs;
- projects;
- troubleshooting;
- assessments;
- rechecks;
- security;
- sustainable workload;
- roadmap revision.

## HomeLab

Defined HomeLab v1 requirements before implementation.

Physical deployment is intentionally separated from repository planning.

# Sprint 0 outputs

The major outputs are:

    docs/baseline/baseline-v1.md
    docs/roadmap/roadmap-v1.md
    docs/roadmap/dependency-map.md
    docs/roadmap/learning-rules.md
    docs/skills/skills-matrix.md
    homelab/architecture/homelab-v1-requirements.md

# Exit criteria

Sprint 0 is complete when:

- `main` contains the final planning documentation;
- Assessment Week is archived;
- Baseline v1 exists;
- Roadmap v1 exists;
- skills matrix exists;
- learning rules exist;
- HomeLab v1 requirements exist;
- Git working tree is clean;
- the planning branch has been reviewed and merged.

# Next stage

After Sprint 0:

1. deploy HomeLab v1 according to the requirements;
2. validate the environment;
3. document the resulting physical / virtual architecture;
4. start Sprint 1 — CS Foundations through Python.

The HomeLab deployment itself is treated as implementation work based on the specification created during Sprint 0.

# Retrospective

Sprint 0 established an important distinction between:

- learning infrastructure;
- technical learning;
- infrastructure implementation.

The repository is the source of truth for planning and evidence.

The HomeLab is the primary practical environment.

The roadmap connects the two.
