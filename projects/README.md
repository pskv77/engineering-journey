# Projects

This directory contains larger engineering projects that combine multiple skills.

Unlike labs, projects are not focused on a single isolated mechanism.

A project should gradually integrate:

- programming;
- Linux;
- networking;
- databases;
- APIs;
- automation;
- containers;
- delivery;
- monitoring;
- infrastructure;
- security.

## Core principle

Whenever possible, new technologies should extend an existing project instead of creating another unrelated disposable project.

The purpose is to build cumulative engineering experience.

## Labs vs Projects

A lab answers a focused question.

Example:

- how Docker port publishing works;
- how Linux signals work;
- how SQL GROUP BY works.

A project combines many of these mechanisms into one working system.

Example:

- Python application;
- PostgreSQL database;
- Linux service;
- Nginx reverse proxy;
- Docker Compose;
- CI/CD;
- monitoring;
- later Kubernetes and cloud deployment.

## Main evolving project

The learning roadmap should maintain at least one primary project that grows together with the engineering skill set.

The exact idea may change, but the expected evolution is approximately:

    Stage 1
    Python CLI application

        ↓

    Stage 2
    Files / JSON / logging

        ↓

    Stage 3
    HTTP API integration

        ↓

    Stage 4
    PostgreSQL

        ↓

    Stage 5
    Linux service

        ↓

    Stage 6
    Nginx reverse proxy

        ↓

    Stage 7
    Docker / Docker Compose

        ↓

    Stage 8
    CI/CD

        ↓

    Stage 9
    Monitoring / observability

        ↓

    Stage 10
    Infrastructure as Code

        ↓

    Stage 11
    Kubernetes

        ↓

    Stage 12
    Cloud

        ↓

    Stage 13
    Infrastructure / DevSecOps security

This sequence is not fixed.

The roadmap may change depending on learning results and professional priorities.

## Project requirements

A meaningful project should gradually include:

- clear purpose;
- architecture documentation;
- source code;
- configuration;
- Git history;
- testing where appropriate;
- logging;
- deployment instructions;
- troubleshooting notes;
- security considerations.

## Documentation

A project directory should normally contain a `README.md`.

A larger project may use:

    project-name/
    ├── README.md
    ├── docs/
    ├── src/
    ├── tests/
    ├── scripts/
    ├── configs/
    └── infrastructure/

The exact structure depends on the project.

## Git workflow

Project work should normally happen through branches.

Examples:

    feature/api-client
    feature/postgresql-storage
    feature/docker-compose
    fix/database-timeout
    security/reduce-container-privileges

Changes should be reviewed before they are merged into the stable version.

## Security

Projects must not contain:

- real passwords;
- real API tokens;
- private keys;
- confidential company data;
- production configurations containing sensitive information.

Use test data and secret-management mechanisms appropriate for the current learning stage.

## Portfolio

The private learning repository may contain unfinished work, failed experiments and internal notes.

Later, selected mature projects may be cleaned up and published separately as portfolio projects.

The learning repository is the workshop.

The public portfolio is the showcase.
