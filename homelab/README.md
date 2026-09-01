# HomeLab

This directory documents the personal infrastructure laboratory used for hands-on engineering practice.

The homelab is intended to become the primary environment for learning:

- Linux administration;
- Windows administration;
- networking;
- Active Directory;
- security;
- Docker;
- monitoring;
- Infrastructure as Code;
- Kubernetes;
- cloud-related infrastructure concepts.

## Host platform

Primary physical host:

- Apple MacBook Pro
- Apple M3 Pro

Virtual machines and isolated virtual networks will be used to build training infrastructure.

## Core principle

The homelab should evolve gradually with the roadmap.

It should not be built as a large complex environment before the required technologies are understood.

New components are added when they become useful for a sprint or project.

## Initial architecture

The first version should remain small.

Expected initial machines:

- Linux server
- second Linux host or client
- Windows workstation

Later additions may include:

- Windows Server;
- Active Directory Domain Services;
- DNS infrastructure;
- routing/firewall VM;
- DMZ segment;
- Docker hosts;
- monitoring infrastructure;
- Kubernetes nodes.

## Network evolution

Possible future logical networks:

    USERS
    10.10.10.0/24

    SERVERS
    10.10.20.0/24

    DMZ
    10.10.30.0/24

    MANAGEMENT
    10.10.40.0/24

The final addressing scheme may change during implementation.

## Documentation structure

### `architecture/`

Overall architecture, diagrams and design decisions.

### `machines/`

Documentation for virtual machines and their roles.

### `networks/`

Subnets, addressing, routing, DNS, firewall rules and connectivity.

### `diagrams/`

Architecture and network diagrams.

## Documentation requirements

Important infrastructure changes should be documented.

Useful information includes:

- hostname;
- operating system;
- role;
- IP address;
- network;
- installed services;
- dependencies;
- credentials policy;
- security configuration;
- troubleshooting notes.

## Learning approach

The homelab should contain both working and intentionally broken scenarios.

Examples:

- broken DNS;
- incorrect firewall rule;
- inaccessible service;
- wrong permissions;
- failed systemd service;
- routing failure;
- certificate problem;
- Docker networking issue;
- Active Directory authentication problem.

The expected troubleshooting process is:

    symptom
        ↓
    hypothesis
        ↓
    evidence
        ↓
    diagnosis
        ↓
    change
        ↓
    verification

## Security

The homelab must remain isolated from production environments.

Do not store:

- company credentials;
- production configuration;
- confidential corporate information;
- real production secrets.

Use synthetic users, test credentials and intentionally created training data.

## Long-term goal

The homelab should gradually evolve from several basic virtual machines into a small realistic infrastructure environment where networking, systems, automation and security can be practiced together.
