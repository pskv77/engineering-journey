# Engineering Roadmap v1.0

Date: 2026-09-01

Status: Active

This document defines the initial long-term engineering learning roadmap based on the August 2026 Assessment Week.

The roadmap is expected to evolve as practical experience, assessment results and professional interests develop.

## Starting point

Current overall profile:

Network / Security-oriented infrastructure beginner with good engineering intuition, but uneven technical fundamentals.

The strongest current areas are:

- networking;
- network security;
- cybersecurity fundamentals;
- Git;
- practical infrastructure reasoning.

The largest foundational gaps are:

- Computer Science fundamentals;
- active Python programming;
- Linux system fundamentals;
- Bash;
- SQL.

Several areas are mostly new engineering branches:

- PowerShell;
- Windows enterprise infrastructure;
- Active Directory;
- Infrastructure as Code;
- Kubernetes;
- observability;
- cloud infrastructure.

## Long-term direction

The initial direction is:

Infrastructure + Security + Automation

Possible future professional trajectories include:

- Infrastructure Security;
- Security Engineering;
- DevSecOps;
- Cloud Security;
- Infrastructure Engineering with strong security specialization.

A final specialization is intentionally not selected yet.

The first objective is to build a broad engineering foundation and obtain enough practical experience to make that decision based on evidence.

# Learning architecture

The learning system is cumulative.

Technologies are not studied as isolated subjects.

New skills should reuse previously acquired skills.

Example progression:

    CS fundamentals
        ↓
    Python
        ↓
    Linux + Bash
        ↓
    APIs + SQL + Automation
        ↓
    Docker + Nginx
        ↓
    CI/CD
        ↓
    Monitoring + IaC
        ↓
    Kubernetes
        ↓
    Cloud
        ↓
    Infrastructure Security / DevSecOps

Networking and cybersecurity remain active throughout the entire roadmap.

PowerShell and Windows form a parallel branch that later joins infrastructure engineering.

# Phase I — Engineering Foundation

Estimated duration:

Approximately 12–14 weeks after completion of Sprint 0.

Primary objective:

Build a reliable lower technical layer before moving into modern infrastructure platforms.

## Sprint 0 — Learning Infrastructure

Purpose:

Build the environment in which future learning will happen.

Main outcomes:

- Git and GitHub workflow;
- repository architecture;
- Assessment Week archive;
- Baseline v1.0;
- ranking system;
- Roadmap v1.0;
- learning rules;
- skills matrix;
- HomeLab requirements;
- sprint workflow.

Sprint 0 does not attempt to improve technical ranks significantly.

Its goal is to create the engineering learning system itself.

## Sprint 1 — CS Foundations through Python

Primary areas:

- computational thinking;
- algorithmic complexity;
- arrays and lists;
- stacks and queues;
- hash tables;
- searching;
- sorting;
- memory basics;
- processes and threads introduction.

Python is used as the practical language for implementing concepts.

Expected practice:

- small implementations;
- complexity analysis;
- debugging;
- Git usage;
- tests where appropriate.

Target:

Computer Science approximately Rank 1.7–2.0.

Python begins active restoration.

## Sprint 2 — Python Engineering Foundations

Primary areas:

- Python syntax;
- collections;
- functions;
- modules;
- files;
- exceptions;
- JSON;
- CSV;
- logging;
- basic testing;
- command-line utilities.

Goal:

Move from conceptual understanding to active programming ability.

Expected output:

A small useful Python application that later becomes part of the main evolving project.

Target:

Python approximately Rank 2.2–2.5.

Git approximately Rank 2.7–3.0 through continued use.

## Sprint 3 — Linux Fundamentals + Bash

Primary areas:

- users;
- groups;
- permissions;
- sudo;
- processes;
- signals;
- filesystem hierarchy;
- disks;
- filesystems;
- mounts;
- basic Bash;
- pipes;
- redirection;
- environment variables.

Practice should happen primarily inside the HomeLab.

Expected tasks include both configuration and troubleshooting.

Target:

Linux approximately Rank 1.7–2.0.

Bash approximately Rank 1.7–2.0.

## Sprint 4 — Linux Systems & Networking

Primary areas:

- systemd;
- journalctl;
- services;
- SSH;
- sockets;
- routing;
- DNS;
- storage;
- system troubleshooting;
- Linux networking tools.

The Python application from earlier sprints should become a Linux service.

Expected troubleshooting scenarios:

- failed service;
- wrong permissions;
- occupied port;
- DNS failure;
- routing issue;
- broken configuration;
- SSH problem.

Target:

Linux approximately Rank 2.0–2.3.

Networking should remain at approximately Rank 2.5+.

## Sprint 5 — API + SQL + Automation

Primary areas:

- HTTP;
- REST;
- authentication;
- query parameters;
- pagination;
- timeouts;
- retries;
- error handling;
- PostgreSQL;
- SQL SELECT;
- JOIN;
- GROUP BY;
- HAVING;
- ORDER BY;
- automation reliability;
- idempotency;
- logging.

Expected project evolution:

    external API
        ↓
    Python collector
        ↓
    PostgreSQL
        ↓
    processing
        ↓
    report or API output

Target:

SQL approximately Rank 1.8–2.0.

API / HTTP approximately Rank 2.1–2.3.

Automation approximately Rank 2.0+.

## Sprint 6 — Docker + Compose + Nginx

Primary areas:

- container concepts;
- images;
- layers;
- Dockerfile;
- containers;
- registry;
- volumes;
- networks;
- port publishing;
- Docker Compose;
- health checks;
- Nginx;
- reverse proxy;
- TLS termination concepts.

The existing project should be containerized instead of creating an unrelated project.

Security requirements should include:

- non-root containers where appropriate;
- minimal port exposure;
- secrets kept outside source code;
- dependency and image hygiene;
- explicit network boundaries.

Target:

Docker approximately Rank 2.0–2.3.

Nginx approximately Rank 2.0+.

# Parallel tracks

## Git

Git is used continuously in every sprint.

Git is not a separate future learning topic.

Expected practice:

- branches;
- commits;
- pull requests;
- review;
- merge;
- history inspection;
- troubleshooting mistakes;
- gradually more advanced workflows.

## Networking

Networking is currently the strongest technical foundation and should not be relearned from zero.

Instead, every sprint should contain at least one networking-oriented task.

Examples:

- sockets;
- routing;
- DNS;
- service ports;
- firewall rules;
- Docker networking;
- reverse proxies;
- load balancing;
- Kubernetes networking;
- cloud networking.

## Cybersecurity

Security is a permanent engineering overlay.

Every technology should include relevant security questions.

Examples:

- permissions;
- least privilege;
- authentication;
- authorization;
- secrets;
- network segmentation;
- TLS;
- hardening;
- logging;
- monitoring;
- attack surface;
- secure defaults.

Existing security knowledge should gradually become more technical and evidence-driven.

## PowerShell

PowerShell starts early as a small parallel track.

Initial frequency:

Approximately two short sessions per week.

Initial topics:

- syntax;
- objects;
- pipeline;
- Get-Help;
- files;
- processes;
- services;
- event logs.

The objective is to prevent the later Windows / Active Directory phase from requiring simultaneous learning of both enterprise Windows and PowerShell from zero.

## External courses

External courses are supplementary resources.

Approximate learning distribution:

- 60–70% labs and projects;
- 20–25% structured courses and external learning;
- 10–15% assessments, documentation and retrospectives.

Yandex Practicum may be used when its modules support the current roadmap objective.

The roadmap must not be reorganized merely because a particular course exists.

# Comprehensive Control #1

After Sprint 6, perform the first major cumulative assessment.

The control should combine:

- CS;
- Python;
- Git;
- Linux;
- Bash;
- networking;
- HTTP/API;
- SQL;
- Docker;
- Nginx;
- cybersecurity.

The assessment should include a realistic engineering scenario rather than isolated questions only.

Possible structure:

    inspect unfamiliar system
        ↓
    identify failures
        ↓
    read logs
        ↓
    diagnose networking
        ↓
    modify application or automation
        ↓
    repair service
        ↓
    repair container deployment
        ↓
    verify security properties
        ↓
    document findings

The results of Comprehensive Control #1 determine whether Phase II begins immediately or whether selected Phase I skills require another cycle.

# Phase II — Infrastructure Engineering

Phase II is intentionally less detailed until Phase I results are available.

Expected areas:

- CI/CD;
- deeper PowerShell;
- Windows administration;
- Active Directory;
- monitoring;
- observability;
- Infrastructure as Code;
- infrastructure automation;
- secrets management;
- advanced Linux operations.

The exact order will be revised after Comprehensive Control #1.

# Phase III — Modern Infrastructure & Cloud

Expected areas:

- Kubernetes;
- container orchestration;
- cloud architecture;
- cloud networking;
- IAM;
- cloud security;
- Infrastructure as Code at larger scale;
- observability;
- resilient infrastructure.

These topics should not be rushed before the foundations are reliable.

# Phase IV — Security Specialization

The specialization phase will be designed after significant hands-on exposure to infrastructure engineering.

Possible directions:

- Infrastructure Security;
- DevSecOps;
- Cloud Security;
- Security Engineering;
- Detection and Response engineering;
- security-focused platform engineering.

The decision should be based on:

- practical performance;
- professional opportunities;
- interest after hands-on experience;
- assessment results;
- university experience;
- work experience.

# Phase I target profile

By the end of Phase I, the expected profile is approximately:

| Area | Initial | Phase I target |
| --- | ---: | ---: |
| Computer Science | 0.8 | 1.7–2.0 |
| Python | ~1.5 | 2.2–2.5 |
| Git | 2.4 | 2.7–3.0 |
| Linux | 1.3 | 2.0–2.3 |
| Bash | ~1.7 | 2.0+ |
| Networks | 2.3 | 2.5+ |
| Cybersecurity | 1.9 | 2.3+ |
| SQL | 1.0 | 1.8–2.0 |
| HTTP / API | 1.8 | 2.1–2.3 |
| Docker | 1.2 | 2.0–2.3 |
| Nginx | ~1.5 | 2.0+ |

Targets are directional rather than mathematical guarantees.

Rank changes require practical evidence.

# Workload

Typical target:

8–10 hours per week.

Minimum sustainable difficult week:

5–6 hours.

High-capacity week:

10–12 hours.

Consistency is more important than occasional extreme workloads.

# Roadmap revision

Roadmap v1.0 is not permanent.

It should be reconsidered after:

- sprint assessments;
- 4–6 week rechecks;
- Comprehensive Control #1;
- major changes in work responsibilities;
- meaningful university experience;
- completion of major projects.

New roadmap versions should be created rather than silently rewriting the historical starting plan.
