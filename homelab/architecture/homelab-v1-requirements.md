# HomeLab v1 — Requirements

Version: 1.0

Date: 2026-09-01

Status: Design specification

This document defines the requirements for the first version of the engineering HomeLab.

It describes what the environment must support.

It intentionally does not lock the implementation to a specific hypervisor or product before compatibility and technical constraints are verified.

# 1. Purpose

The HomeLab is the primary hands-on systems environment for the engineering roadmap.

It must support practical learning in:

- Linux;
- Bash;
- networking;
- Python services;
- Windows;
- PowerShell;
- security;
- databases;
- Nginx;
- Docker;
- monitoring;
- automation;
- later Active Directory;
- later Infrastructure as Code;
- later Kubernetes.

The environment should evolve together with the roadmap.

# 2. Physical host

Primary host:

- Apple MacBook Pro;
- Apple M3 Pro;
- Apple Silicon / ARM architecture.

The implementation must take ARM compatibility into account.

Before selecting the virtualization platform and guest operating systems, current compatibility must be verified.

In particular, assumptions about x86-only operating systems or Windows Server support must not be made without verification.

# 3. Design principles

HomeLab v1 should be:

- small;
- understandable;
- reproducible;
- isolated;
- easy to reset;
- easy to extend;
- documented;
- resource-conscious;
- safe for experimentation.

Complexity should be introduced gradually.

The first version should not attempt to simulate an enterprise datacenter.

# 4. Initial capabilities

HomeLab v1 must allow:

- creation of multiple virtual machines;
- communication between selected VMs;
- isolation from production/company infrastructure;
- controlled Internet access;
- private internal networking;
- static IP addressing where useful;
- SSH access to Linux systems;
- administrative access to Windows systems;
- service deployment;
- DNS experiments;
- routing experiments;
- firewall experiments;
- intentionally broken configurations;
- snapshots or equivalent rollback capability.

# 5. Initial machine roles

The initial environment should support at least the following logical roles.

## Linux Server

Purpose:

- Linux administration;
- systemd;
- SSH;
- networking;
- Python services;
- Nginx;
- PostgreSQL;
- later Docker.

Example logical hostname:

    lab-linux-01

## Linux Client / Utility Host

Purpose:

- client-side testing;
- SSH;
- DNS testing;
- network diagnostics;
- API calls;
- traffic generation;
- troubleshooting.

Example logical hostname:

    lab-linux-02

This machine may initially be lightweight.

## Windows Workstation

Purpose:

- Windows administration;
- PowerShell;
- networking;
- event logs;
- remote administration;
- later domain membership.

Example logical hostname:

    lab-win-01

The exact Windows edition must be compatible with the selected Apple Silicon virtualization approach.

# 6. Future machine roles

The architecture must allow later addition of:

- directory-services server;
- DNS server;
- firewall/router VM;
- monitoring server;
- CI runner;
- additional Docker host;
- Kubernetes nodes;
- security monitoring components.

Not all of these should be deployed in HomeLab v1.

# 7. Windows / Active Directory constraint

The long-term roadmap requires practical Windows enterprise and Active Directory experience.

However, the physical host uses Apple Silicon.

Therefore:

- HomeLab v1 must not assume that a traditional x86 Windows Server VM can run locally;
- the exact AD implementation approach must be selected after compatibility research;
- possible solutions may include a supported ARM-compatible approach, external x86 virtualization, cloud resources, or another suitable lab method.

The requirement is to preserve the ability to introduce realistic directory-services practice later.

The implementation mechanism is deferred.

# 8. Network architecture

The HomeLab should initially support at least two logical network types.

## External / NAT network

Purpose:

- package installation;
- updates;
- controlled Internet access;
- external API access.

## Internal lab network

Purpose:

- communication between lab machines;
- static addressing;
- service discovery;
- network troubleshooting;
- isolation from the normal home/work network.

Initial implementation may remain simple.

The architecture must allow later segmentation.

# 9. Future segmentation

The future logical design may evolve toward:

    USERS
    10.10.10.0/24

    SERVERS
    10.10.20.0/24

    DMZ
    10.10.30.0/24

    MANAGEMENT
    10.10.40.0/24

These networks are planning placeholders.

They should not be created merely to satisfy the diagram.

Segmentation should be introduced when corresponding networking/security labs begin.

# 10. Addressing

HomeLab addressing must be:

- private;
- documented;
- predictable;
- separated from corporate networks;
- preferably separated from the user's normal LAN addressing.

Every persistent VM should eventually have documented:

- hostname;
- IP;
- subnet;
- gateway;
- DNS configuration;
- role.

# 11. Naming convention

Recommended machine naming:

    lab-<platform>-<number>

Examples:

    lab-linux-01
    lab-linux-02
    lab-win-01

Future role-specific names may include:

    lab-dc-01
    lab-mon-01
    lab-k8s-01

Names should remain understandable without external context.

# 12. Resource requirements

The HomeLab must be designed to avoid unnecessary pressure on the MacBook.

Requirements:

- VMs should receive only the CPU and RAM they actually need;
- unused VMs should normally remain powered off;
- heavy multi-node systems should be introduced only when required;
- the lab should remain usable during normal laptop operation.

Before implementation, available RAM, storage and expected VM requirements should be reviewed.

# 13. Storage

The implementation should define:

- where VM files are stored;
- approximate storage allocation;
- thin / dynamic allocation where appropriate;
- cleanup policy;
- snapshot policy.

Large disposable artifacts should not be committed into Git.

# 14. Snapshots and rollback

The environment must support recovery from destructive experiments.

Important milestones should allow rollback.

Example snapshot points:

    clean-install
    base-configured
    networking-working
    service-working
    pre-security-lab

Snapshots must not replace documentation or backups.

They are primarily for controlled experimentation.

# 15. Reproducibility

Manual configuration is acceptable during early learning because understanding the mechanism is important.

Over time, repeated setup should become increasingly automated.

Expected progression:

    manual installation
        ↓
    documented configuration
        ↓
    scripts
        ↓
    configuration automation
        ↓
    Infrastructure as Code where appropriate

# 16. Linux requirements

Linux VMs must allow practice with:

- users;
- groups;
- permissions;
- sudo;
- processes;
- signals;
- services;
- systemd;
- journal;
- filesystems;
- storage;
- SSH;
- routing;
- DNS;
- sockets;
- firewall;
- package management;
- Bash;
- Python.

The selected distribution should be common, well documented and suitable for server practice.

# 17. Windows requirements

The Windows environment should eventually allow practice with:

- PowerShell;
- users and groups;
- services;
- event logs;
- networking;
- firewall;
- NTFS permissions;
- SMB;
- remote administration;
- enterprise identity concepts;
- later domain membership.

# 18. Application requirements

The HomeLab must support deployment of the evolving learning project.

Expected progression:

    Python application
        ↓
    Linux service
        ↓
    PostgreSQL
        ↓
    Nginx
        ↓
    Docker Compose
        ↓
    CI/CD
        ↓
    monitoring
        ↓
    later Kubernetes

This allows the same system to be observed at multiple infrastructure layers.

# 19. Troubleshooting requirements

The lab must allow intentionally broken scenarios.

Examples:

- failed DNS resolution;
- incorrect IP configuration;
- wrong route;
- blocked port;
- firewall error;
- broken SSH access;
- wrong filesystem permissions;
- failed systemd service;
- occupied port;
- invalid Nginx configuration;
- database connectivity failure;
- Docker networking failure.

The standard diagnostic process should be:

    symptom
        ↓
    hypothesis
        ↓
    evidence
        ↓
    diagnosis
        ↓
    remediation
        ↓
    verification

# 20. Security requirements

The lab must remain separate from production/company environments.

Never use:

- production passwords;
- company credentials;
- confidential company files;
- production private keys;
- real customer data.

Use synthetic data and credentials.

Security practices should gradually include:

- least privilege;
- SSH key authentication;
- firewall rules;
- segmentation;
- secrets handling;
- TLS;
- service hardening;
- logging;
- non-root container execution.

# 21. Git documentation

The HomeLab itself is not stored inside Git as VM disk images.

Git stores the engineering description of the HomeLab.

Expected documentation includes:

    homelab/
    ├── architecture/
    ├── machines/
    ├── networks/
    └── diagrams/

Machine documentation should eventually contain:

- role;
- OS;
- resources;
- interfaces;
- addresses;
- installed services;
- configuration notes;
- security settings;
- dependencies.

# 22. Secrets

No real secrets should be committed.

Future automation must use appropriate secret-handling patterns.

Example placeholder:

    DB_PASSWORD=<secret>

rather than real credentials.

# 23. Observability readiness

The initial lab does not need a full monitoring stack.

However, its architecture should allow future collection of:

- system logs;
- application logs;
- metrics;
- service health;
- network information.

# 24. Automation readiness

The environment must eventually allow:

- Bash automation;
- Python automation;
- PowerShell automation;
- configuration management;
- IaC;
- CI/CD interaction.

Automation should be introduced only after the manual mechanism is understood.

# 25. HomeLab versions

## HomeLab v1

Goal:

Basic multi-VM infrastructure.

Expected capabilities:

- Linux;
- Windows;
- internal networking;
- Internet access;
- SSH;
- basic services;
- snapshots;
- troubleshooting.

## HomeLab v2

Likely additions:

- more deliberate segmentation;
- routing/firewall component;
- Windows enterprise services;
- centralized DNS;
- monitoring;
- Docker workloads.

## HomeLab v3

Possible additions:

- IaC;
- CI/CD infrastructure;
- Kubernetes;
- security monitoring;
- cloud integration.

Version boundaries are flexible.

# 26. Implementation sequence

The physical build should follow approximately:

    1. Verify Apple Silicon virtualization options
    2. Inspect available host resources
    3. Select virtualization platform
    4. Define storage location
    5. Define initial virtual networks
    6. Deploy first Linux VM
    7. Validate snapshots and cloning
    8. Deploy second Linux / utility VM
    9. Deploy Windows workstation
    10. Validate VM-to-VM connectivity
    11. Document addresses and roles
    12. Establish clean baseline snapshots
    13. Perform first troubleshooting scenarios
    14. Begin Sprint 1 usage

Each stage should be validated before proceeding.

# 27. HomeLab v1 acceptance criteria

HomeLab v1 is considered operational when:

- virtualization works reliably on the M3 Pro host;
- at least two Linux-capable endpoints exist;
- a Windows environment exists;
- internal VM communication works;
- controlled Internet access works;
- SSH access works;
- addressing is documented;
- snapshots / rollback are tested;
- machines are documented in Git;
- no production secrets are present;
- a deliberately broken networking or service scenario can be created and recovered from.

# 28. Non-goals for v1

HomeLab v1 does not require:

- Kubernetes;
- enterprise-grade HA;
- complex VLAN architecture;
- full SIEM;
- full Active Directory deployment;
- production monitoring;
- cloud integration;
- infrastructure automation from day one.

These are later roadmap stages.

# 29. Final principle

The HomeLab exists to support engineering learning.

Its complexity must follow learning needs.

The goal is not to build the largest possible lab.

The goal is to build an environment where systems can be:

- understood;
- configured;
- broken;
- investigated;
- repaired;
- automated;
- secured.
