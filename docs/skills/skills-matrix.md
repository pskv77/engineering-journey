# Skills Matrix v1.0

Date: 2026-09-01

Status: Initial baseline

This document converts the August 2026 Assessment Week results into a working engineering skills matrix.

Ranks use the 0–5 independence scale defined in `docs/skills/README.md`.

The matrix is not intended to be static.

Ranks should be updated only when new practical evidence exists.

# Summary

| Area | Current Rank | Learning State | Priority | Phase I Target |
| --- | ---: | --- | --- | ---: |
| Computer Science | 0.8 | Rebuild | P0 | 1.7–2.0 |
| Python | 1.5 | Restore | P0 | 2.2–2.5 |
| Git | 2.4 | Maintain / Deepen | P1 | 2.7–3.0 |
| Linux | 1.3 | Systematize | P0 | 2.0–2.3 |
| Bash | 1.7 | Restore | P1 | 2.0+ |
| Networks | 2.3 | Maintain / Deepen | Continuous | 2.5+ |
| Cybersecurity | 1.9 | Deepen | Continuous | 2.3+ |
| SQL | 1.0 | Restore / Build | P1 | 1.8–2.0 |
| HTTP / API | 1.8 | Deepen | P1 | 2.1–2.3 |
| Docker | 1.2 | Restore / Build | P1 | 2.0–2.3 |
| Nginx | 1.5 | Restore / Build | P1 | 2.0+ |
| PowerShell | 0.2 | New branch | Parallel | 1.0+ |
| Windows Infrastructure | 0.9 | New branch | P2 | Later phase |
| Active Directory | <1.0 | New branch | P2 | Later phase |
| CI/CD | ~1.1 | Build | P2 | Later phase |
| Observability | 0.2 | New branch | P2 | Later phase |
| Infrastructure as Code | 0.4 | New branch | P2 | Later phase |
| Kubernetes | 0.4 | New branch | P2 | Later phase |
| Cloud Infrastructure | 0.2 | New branch | P2 | Later phase |

# Priority model

## P0 — Foundational debt

These areas limit progress in many later technologies.

Current P0:

- Computer Science;
- Python;
- Linux.

They should be addressed first.

## P1 — Engineering core

These skills convert foundational knowledge into practical engineering capability.

Current P1:

- Git;
- Bash;
- SQL;
- HTTP / API;
- automation;
- Docker;
- Nginx.

## P2 — Expansion

These areas depend on earlier foundations.

Current P2:

- Windows enterprise infrastructure;
- Active Directory;
- CI/CD;
- monitoring and observability;
- Infrastructure as Code;
- Kubernetes;
- cloud infrastructure.

## Continuous

These areas remain active across the entire roadmap:

- networking;
- cybersecurity.

# Computer Science

Current rank: 0.8

Learning state: Rebuild

Assessment result: 24.75 / 100

## Current strengths

- some recognition of basic concepts;
- previous exposure to algorithms and operating systems;
- ability to recognize some correct answers.

## Main gaps

- Big O;
- algorithm complexity;
- data structures;
- hash tables;
- memory;
- virtual memory;
- processes;
- threads;
- concurrency;
- race conditions;
- CPU / cache / interrupts / I/O mental models.

## Phase I evidence required

- implement basic structures and algorithms;
- explain complexity;
- reason about memory behavior;
- explain process vs thread;
- diagnose basic concurrency examples;
- complete cumulative assessment without relying on recognition alone.

Target: 1.7–2.0

# Python

Current rank: approximately 1.5

Learning state: Restore

## Current strengths

- programming logic;
- ability to understand existing code;
- reasonable engineering intuition;
- prior use of Python.

## Main gaps

- active syntax recall;
- data structures;
- functions;
- modules;
- files;
- exceptions;
- JSON / CSV;
- logging;
- tests;
- writing complete programs independently.

## Phase I evidence required

- multiple independent scripts;
- file processing;
- API client;
- error handling;
- logging;
- database integration;
- project code;
- tests where appropriate.

Target: 2.2–2.5

# Git

Current rank: 2.4

Learning state: Maintain / Deepen

## Current strengths

- repository setup;
- branches;
- commits;
- push / pull;
- pull requests;
- merge workflow;
- basic troubleshooting.

## Main development areas

- conflict resolution;
- rebase concepts;
- history inspection;
- restore / reset distinctions;
- cherry-pick;
- more deliberate commit structure;
- advanced collaboration workflow.

## Phase I evidence required

Git should be used throughout all work rather than trained in isolation.

Target: 2.7–3.0

# Linux

Current rank: 1.3

Learning state: Systematize

Assessment result: 43.7 / 100

## Stronger areas

- SSH;
- basic networking;
- some operational intuition.

## Main gaps

- users and groups;
- permissions;
- sudo;
- processes;
- signals;
- systemd;
- journal;
- filesystems;
- disks;
- mounts;
- inode model;
- systematic troubleshooting.

## Phase I evidence required

- administer Linux VMs;
- configure permissions;
- manage services;
- troubleshoot failed services;
- work with disks and filesystems;
- use SSH safely;
- inspect sockets and networking;
- deploy the evolving project.

Target: 2.0–2.3

# Bash

Current rank: approximately 1.7

Learning state: Restore

## Main gaps

- syntax fluency;
- pipelines;
- variables;
- loops;
- conditions;
- exit codes;
- robust scripting.

## Evidence required

- administration scripts;
- pipelines;
- log processing;
- automation around Linux tasks.

Target: 2.0+

# Networks

Current rank: 2.3

Learning state: Maintain / Deepen

Assessment result: 70.8 / 100

This is the strongest current technical area.

## Current strengths

- subnetting;
- routing logic;
- DNS / DHCP / NAT;
- network troubleshooting;
- practical operational experience.

## Development areas

- packet flow precision;
- MAC rewriting vs IP forwarding;
- STP / LACP / VRRP distinctions;
- stateful firewall behavior;
- deeper secure network architecture.

## Strategy

Do not restart networking from zero.

Use networking continuously inside other technical areas.

Target: 2.5+

# Cybersecurity

Current rank: 1.9

Learning state: Deepen

Assessment result: 60.7 / 100

## Current strengths

- security fundamentals;
- IAM intuition;
- web authorization concepts;
- SIEM concepts;
- compliance;
- general incident-response reasoning.

## Main gaps

- PKI;
- certificate chains;
- TLS;
- evidence-driven incident response;
- formal threat / risk models;
- deeper offensive understanding.

## Strategy

Security becomes a permanent overlay on infrastructure work.

Target: 2.3+

# SQL

Current rank: 1.0

Learning state: Restore / Build

## Main gaps

- aggregation;
- GROUP BY;
- HAVING;
- JOIN;
- ordering aggregate results;
- practical database usage.

## Evidence required

- PostgreSQL deployment;
- schema creation;
- queries;
- Python integration;
- reporting;
- troubleshooting database connectivity.

Target: 1.8–2.0

# HTTP / API

Current rank: 1.8

Learning state: Deepen

## Main gaps

- authentication patterns;
- authorization distinctions;
- query parameters;
- pagination;
- timeouts;
- retries;
- reliable API consumption.

Target: 2.1–2.3

# Docker

Current rank: 1.2

Learning state: Restore / Build

## Existing exposure

- containers;
- Dockerfiles;
- Docker Compose.

## Main gaps

- image layers;
- runtime model;
- storage;
- networks;
- health checks;
- registry workflow;
- security.

Target: 2.0–2.3

# Nginx

Current rank: approximately 1.5

Learning state: Restore / Build

## Development areas

- reverse proxy;
- upstreams;
- headers;
- logging;
- TLS termination;
- troubleshooting.

Target: 2.0+

# PowerShell

Current rank: 0.2

Learning state: New branch

This is currently one of the weakest practical skills.

PowerShell begins as a parallel micro-track before the dedicated Windows phase.

Initial topics:

- syntax;
- objects;
- pipeline;
- Get-Help;
- processes;
- services;
- files;
- event logs.

# Windows Infrastructure

Current rank: 0.9

Learning state: New branch

Assessment result: 36.2 / 100

Major development areas:

- Windows Server concepts;
- services;
- event logs;
- DNS;
- NTFS;
- SMB;
- GPO;
- authentication;
- enterprise troubleshooting.

Dedicated development occurs primarily after Phase I.

# Active Directory

Learning state: New branch

Development areas include:

- domain architecture;
- users;
- groups;
- OU;
- DNS;
- Kerberos;
- NTLM;
- GPO;
- permissions;
- identity lifecycle;
- enterprise security.

# CI/CD

Current rank: approximately 1.1

Learning state: Build

Existing conceptual exposure exists, but independent practical capability is limited.

This becomes a major topic after Docker fundamentals are stable.

# Observability

Current rank: 0.2

Learning state: New branch

Future development areas:

- logs;
- metrics;
- traces;
- dashboards;
- alerting;
- service health;
- evidence-driven troubleshooting.

# Infrastructure as Code

Current rank: 0.4

Learning state: New branch

Future development areas:

- declarative infrastructure;
- state;
- plans;
- reproducibility;
- change control;
- Terraform or equivalent tooling.

# Kubernetes

Current rank: 0.4

Learning state: New branch

Kubernetes is intentionally deferred.

It depends on understanding:

- Linux;
- networking;
- containers;
- services;
- health checks;
- storage;
- configuration;
- observability.

# Cloud Infrastructure

Current rank: 0.2

Learning state: New branch

Cloud learning will focus on architecture and mechanisms rather than memorizing a provider UI.

Future areas:

- compute;
- networking;
- IAM;
- storage;
- managed services;
- resilience;
- observability;
- IaC;
- security.

# Evidence rules

Rank updates require concrete evidence.

Examples:

- assessment;
- lab;
- project;
- troubleshooting task;
- independent explanation;
- work task where appropriate.

Course completion alone is not enough.

# Review cycle

The matrix should be reviewed:

- after every sprint assessment;
- after 4–6 week rechecks;
- after comprehensive controls;
- after major new work experience;
- when a new roadmap version is created.
