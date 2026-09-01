# Baseline v1.0

**Date:** 2026-09-01  
**Source:** Assessment Week, August 2026  
**Purpose:** Fix the starting engineering level before the beginning of the long-term learning roadmap.

---

## Overall profile

Current profile:

**Network / Security-oriented infrastructure beginner with good engineering intuition, but uneven fundamentals.**

Strongest current areas:

- Networks and Network Security
- Cybersecurity fundamentals and security reasoning
- Git
- General troubleshooting logic

Main foundational gaps:

- Computer Science fundamentals
- Python hands-on fluency
- Linux systems knowledge
- Bash and SQL

Mostly new or weakly explored areas:

- Windows Enterprise / Active Directory
- PowerShell
- Kubernetes
- Infrastructure as Code
- Observability
- Cloud architecture

---

## Assessment Week Summary

| Area | Score | Rank | Status |
|---|---:|---:|---|
| Computer Science Fundamentals | 24.75% | 0.8 / 5 | Rebuild |
| Programming & Automation | 62.4% | 1.8 / 5 | Restore + practice |
| Linux & Systems | 43.7% | 1.3 / 5 | Systematize |
| Networks & Network Security | 70.8% | 2.3 / 5 | Current technical foundation |
| Windows & Enterprise Infrastructure | 36.2% | 0.9 / 5 | Mostly new branch |
| Cybersecurity Engineering | 60.7% | 1.9 / 5 | Engineer existing foundation |
| DevOps, Cloud & Infrastructure Security | 18.7% raw | 0.7 / 5 | Mostly new branch |

> DevOps/Cloud raw score is not directly comparable with the other exams because the exam was intentionally stopped when the boundary of current knowledge became clear.

---

# 1. Computer Science Fundamentals

**Rank:** 0.8 / 5  
**Priority:** Critical  
**Learning mode:** Rebuild

### Current state

Recognition is significantly stronger than active recall.

Some concepts are familiar from previous education, but the fundamental model is fragmented and cannot yet be reliably reproduced or used independently.

### Main gaps

- Big O
- basic algorithms
- binary search
- data structures
- memory
- virtual memory
- processes and threads
- concurrency
- CPU / cache / interrupts / I/O

### Target

Bring the foundation to at least **1.7–2.0 / 5** during Phase I.

---

# 2. Programming & Automation

**Rank:** 1.8 / 5  
**Priority:** High  
**Learning mode:** Restore + hands-on practice

### Stronger areas

- Git
- HTTP fundamentals
- automation decomposition
- general programming logic

### Main gaps

- Python syntax fluency
- collections
- files and exceptions
- Bash pipelines
- SQL aggregation
- reliable API clients
- idempotency
- retries / timeouts
- robust automation

### Important subskills

- Git: ~2.4 / 5
- Python: ~1.5 / 5
- Bash: ~1.7 / 5
- SQL: ~1.0 / 5
- HTTP / REST: ~1.8 / 5

### Target

Move Python and practical automation toward **2.2–2.5 / 5**.

Git should become the default environment for all future work rather than a separate subject.

---

# 3. Linux & Systems

**Rank:** 1.3 / 5  
**Priority:** Critical / High  
**Learning mode:** Systematize

### Stronger areas

- SSH
- basic networking
- general troubleshooting logic

### Main gaps

- users / groups / permissions
- process signals
- systemd
- journald
- filesystems
- disks
- inode
- mount / fstab
- system diagnostics

### Target

Build a coherent Linux systems model and reach **2.0–2.3 / 5** during Phase I.

Linux should become the main operating environment for future labs.

---

# 4. Networks & Network Security

**Rank:** 2.3 / 5  
**Priority:** Maintain and deepen  
**Learning mode:** Use as foundation

### Stronger areas

- subnetting
- routing
- VLAN
- DNS
- DHCP
- NAT / PAT
- layered troubleshooting

### Main gaps

- exact packet flow
- ARP / MAC / IP transformation
- STP / LACP / MLAG distinction
- VRRP
- inter-VLAN routing details
- stateful firewall mechanics
- VPN internals

### Target

Do not relearn networking from zero.

Maintain through practical labs and use networking as a supporting layer in Linux, Docker, Kubernetes, cloud and security exercises.

---

# 5. Windows & Enterprise Infrastructure

**Rank:** 0.9 / 5  
**Priority:** High  
**Learning mode:** Mostly new branch

### Existing knowledge

Basic recognition exists for:

- Active Directory
- DNS
- Kerberos
- services
- domain concepts

### Main gaps

- PowerShell
- AD objects
- OU / groups
- GPO
- Kerberos flow
- NTFS / SMB permissions
- Windows troubleshooting
- hardening

### Critical subskill

**PowerShell: ~0.2 / 5**

### Target

Start PowerShell as a parallel micro-track early.

Build the full Windows / AD branch later using virtual machines in the homelab.

---

# 6. Cybersecurity Engineering

**Rank:** 1.9 / 5  
**Priority:** High  
**Learning mode:** Deepen existing foundation

### Stronger areas

- IAM / access control
- Broken Access Control / IDOR
- security fundamentals
- detection concepts
- incident response logic
- compliance

### Main gaps

- PKI / TLS
- formal threat / risk modeling
- investigation depth
- evidence collection
- scope analysis
- containment planning
- offensive / CTF practice

### Important subskills

- Security fundamentals / risk: 2.0
- PKI / TLS: 1.4
- IAM / access control: 2.2
- Web / AppSec: 2.1
- Detection / SIEM: 2.0
- Incident response: 1.8
- Offensive / CTF: 1.3
- Compliance: 2.6

### Target

Do not repeat cybersecurity from zero.

Convert the academic and conceptual base into engineering practice.

---

# 7. DevOps, Cloud & Infrastructure Security

**Rank:** 0.7 / 5  
**Priority:** High / Critical depending on subskill  
**Learning mode:** Mostly new branch

### Existing foundation

Some previous exposure exists to:

- Docker
- Dockerfile
- Docker Compose
- Nginx
- basic CI concepts

### Current subskills

- Docker / containerization: 1.2
- Nginx / reverse proxy: 1.5
- CI/CD / registry: 1.1
- Kubernetes: 0.4
- Infrastructure as Code: 0.4
- Monitoring / observability: 0.2
- Cloud architecture: 0.2
- Infrastructure security: 0.8

### Important distinction

Kubernetes, IaC, observability and cloud are not primarily forgotten skills.

They are areas that have not yet been systematically learned or practiced.

### Target

Build this branch gradually:

Docker → Nginx → CI/CD → Observability → IaC → Kubernetes → Cloud → Infrastructure Security.

---

# Learning Priorities

## P0 — Foundation

- Computer Science
- Python
- Linux

## P1 — Engineering Core

- Git
- Bash
- SQL
- API
- Docker
- Nginx
- CI/CD

## P2 — Expansion

- PowerShell
- Windows / AD
- Observability
- IaC
- Kubernetes
- Cloud

## Continuous overlays

- Networks
- Cybersecurity

---

# Core Learning Principles

1. Theory approximately 20%, practice approximately 80%.
2. Every new skill must reuse previous skills.
3. Git is the default working environment.
4. Labs and projects are preferred over isolated memorization.
5. New technologies should be introduced only when prerequisite mental models are ready.
6. Ranks grow based on independent ability, not course completion.
7. Every major skill must eventually be tested through:
   - explanation;
   - implementation;
   - troubleshooting;
   - integration.
8. Rechecks are required after several weeks.
9. Courses are supporting resources, not the roadmap itself.
10. The homelab is the primary infrastructure practice environment.

---

# Starting Point

This document is the official **Point A** of the engineering roadmap.

Future baseline versions should be compared against this file rather than replacing it.

