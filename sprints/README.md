# Learning Sprints

This directory contains all structured learning sprints.

A sprint is the main unit of the learning system.

Most standard sprints are planned for approximately two weeks and combine:

- theory;
- hands-on practice;
- labs;
- integration with previous skills;
- a small project or engineering task;
- assessment;
- retrospective;
- skill-rank updates.

## Core principle

A sprint is not considered complete because a course or set of videos was finished.

A sprint is complete when the target skills can be demonstrated through practical evidence.

## Typical sprint lifecycle

### 1. Planning

Before the sprint starts, define:

- target skills;
- current ranks;
- target ranks;
- prerequisites;
- learning resources;
- labs;
- integration task;
- final assessment criteria.

### 2. Fundamentals

Study the minimum theory required to understand the mechanisms.

The preferred balance is approximately:

- 20% theory;
- 80% practice.

Theory should support practical work rather than exist independently.

### 3. Practice

Complete small focused exercises.

Examples:

- write code;
- configure a service;
- inspect system state;
- troubleshoot failures;
- analyze logs;
- modify infrastructure;
- explain technical behavior.

### 4. Labs

Labs should introduce realistic conditions and failure modes.

Whenever possible, tasks should require:

observe → form hypothesis → gather evidence → change → verify

rather than blindly following a sequence of commands.

### 5. Integration

New skills must reuse previous skills.

Examples:

- Python code is stored in Git;
- Python applications run on Linux;
- Linux services use networking knowledge;
- applications later use SQL and APIs;
- the same applications are eventually containerized;
- CI/CD builds the existing application;
- monitoring observes the same system;
- Kubernetes later deploys familiar workloads.

The goal is cumulative engineering development.

### 6. Sprint project

Each sprint should produce some useful artifact.

Possible outputs include:

- source code;
- configuration;
- scripts;
- documentation;
- diagrams;
- troubleshooting reports;
- infrastructure definitions;
- improvements to an existing project.

Whenever possible, the sprint project should extend an earlier project rather than create an unrelated disposable exercise.

### 7. Assessment

At the end of the sprint, practical ability is checked.

A sprint assessment may include:

- short theory questions;
- implementation;
- troubleshooting;
- explanation of decisions;
- an engineering case.

Previous skills may also appear in the assessment.

### 8. Retrospective

After the assessment, record:

- what improved;
- what remained weak;
- what was unexpectedly difficult;
- which learning methods worked;
- which topics require recheck;
- whether the roadmap needs adjustment.

### 9. Skill update

Ranks are updated only when supported by evidence.

The update should record:

- previous rank;
- new rank;
- evidence;
- remaining gaps;
- recheck date.

## Sprint directory structure

A typical sprint may look like this:

    sprint-01/
    ├── README.md
    ├── plan.md
    ├── progress.md
    ├── labs/
    ├── project/
    ├── notes/
    └── retrospective.md

The exact structure may change when a sprint requires something different.

## Sprint README

Each sprint should have its own `README.md`.

It should contain at minimum:

- sprint name;
- dates;
- purpose;
- target skills;
- current ranks;
- target ranks;
- expected outputs;
- completion criteria.

## Branching

Development during a sprint should normally happen outside `main`.

Example branch:

    sprint/01-cs-python

Individual experiments or larger tasks may use additional branches.

Completed and reviewed work is merged into `main`.

## Rechecks

Sprint completion is not proof of long-term retention.

Important skills should be rechecked approximately 4–6 weeks later and again through cumulative assessments.

## Sprint 0

`sprint-00` is different from normal learning sprints.

Its purpose is to build the learning infrastructure itself:

- Git workflow;
- repository structure;
- Baseline v1.0;
- Roadmap v1.0;
- skills tracking;
- course tracking;
- homelab planning;
- assessment structure.

Sprint 0 prepares the environment in which the later learning sprints will operate.
