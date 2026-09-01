# Skill Dependency Map

This document describes the main dependencies between the technical areas in the engineering roadmap.

It explains why the learning sequence is structured in its current order.

# Primary engineering chain

    Computer Science
          ↓
        Python
          ↓
    Linux + Bash
          ↓
    API + SQL + Automation
          ↓
    Docker + Nginx
          ↓
         CI/CD
          ↓
    Monitoring / Observability
          ↓
    Infrastructure as Code
          ↓
      Kubernetes
          ↓
        Cloud
          ↓
    Infrastructure Security
          ↓
       DevSecOps

The chain is not strictly linear.

Earlier skills remain active while later skills are introduced.

# Computer Science

Computer Science provides mental models for:

- algorithms;
- complexity;
- data structures;
- memory;
- processes;
- concurrency;
- operating system behavior.

It supports later programming and systems work.

# Python

Python becomes the primary automation language.

It is used for:

- scripting;
- API clients;
- data processing;
- automation;
- infrastructure tooling;
- security tooling;
- tests;
- later cloud and DevOps automation.

# Linux

Linux becomes the primary runtime environment for infrastructure practice.

It provides the environment for:

- processes;
- services;
- permissions;
- networking;
- SSH;
- Nginx;
- databases;
- Docker;
- monitoring;
- Kubernetes.

# API + SQL + Automation

These skills connect programming with real systems.

They introduce:

- external services;
- persistent data;
- retries;
- failures;
- authentication;
- automation reliability.

This creates more realistic applications for later infrastructure work.

# Docker + Nginx

Docker introduces deployment isolation and repeatability.

Nginx introduces:

- reverse proxies;
- service exposure;
- HTTP infrastructure;
- TLS termination concepts.

Together they create the bridge from application development to infrastructure engineering.

# CI/CD

CI/CD automates:

- testing;
- building;
- validation;
- artifact creation;
- deployment.

It should operate on an already understood application and container environment.

# Monitoring and Observability

Observability introduces evidence-driven operations.

Main concepts include:

- metrics;
- logs;
- traces;
- alerts;
- health;
- service-level behavior.

Troubleshooting increasingly becomes based on telemetry rather than guessing.

# Infrastructure as Code

IaC introduces reproducible infrastructure creation and change management.

It should be learned after infrastructure components themselves are understood.

# Kubernetes

Kubernetes combines many earlier topics:

- containers;
- networking;
- services;
- configuration;
- storage;
- health checks;
- orchestration;
- security;
- observability.

It should therefore not be treated as an entry-level isolated technology.

# Cloud

Cloud infrastructure builds on:

- networking;
- Linux;
- IAM;
- automation;
- IaC;
- containers;
- observability.

The objective is to understand cloud architecture rather than simply memorize provider interfaces.

# Horizontal track — Networking

Networking crosses nearly every stage:

    Networking ─────────────────────────────────────────────►

It is reused in:

- Linux;
- APIs;
- DNS;
- Nginx;
- Docker;
- CI/CD;
- Kubernetes;
- cloud;
- infrastructure security.

# Horizontal track — Security

Security is also continuous:

    Security ───────────────────────────────────────────────►

Security concerns should appear in every stage:

- permissions;
- authentication;
- authorization;
- secrets;
- segmentation;
- encryption;
- logging;
- monitoring;
- hardening;
- supply-chain security.

# Parallel Windows branch

Windows infrastructure develops in parallel:

    PowerShell
        ↓
    Windows Administration
        ↓
    Active Directory
        ↓
    Enterprise Identity
        ↓
    Infrastructure Security

PowerShell begins before the dedicated Windows phase.

This prevents learning both the automation language and enterprise platform simultaneously from zero.

# Main principle

A technology should normally be introduced when its prerequisites are sufficiently stable to make practical work meaningful.

The goal is not to complete the dependency graph as quickly as possible.

The goal is to create durable engineering capability.
