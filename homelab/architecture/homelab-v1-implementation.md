# HomeLab v1 — Implemented Architecture

Date: 2026-09-07

Status: Operational

This document describes the actual implemented state of HomeLab v1.

The original design requirements are documented in:

`homelab/architecture/homelab-v1-requirements.md`

# 1. Host Platform

Physical host:

- Apple MacBook Pro
- Apple M3 Pro
- Apple Silicon / ARM64
- 18 GB RAM

Virtualization platform:

- Oracle VirtualBox 7.2.16

The environment is designed around ARM64-compatible guest operating systems.

# 2. Current Virtual Machines

HomeLab v1 currently contains three operational virtual machines:

- Kali Linux
- Ubuntu Server
- Windows 11 ARM

All three machines participate in the internal lab environment.

# 3. Network Architecture

Each VM uses two logical network connections.

## Adapter 1 — NAT

Purpose:

- Internet access
- operating system updates
- package installation
- external API access

## Adapter 2 — Internal Network

VirtualBox network:

`LAB-NET`

Purpose:

- VM-to-VM communication
- isolated lab traffic
- networking experiments
- infrastructure services
- troubleshooting exercises

Conceptually:

    Internet
       |
       |
    VirtualBox NAT
       |
       +------------------+
       |        |         |
     Kali    Ubuntu    Windows
       |        |         |
       +--------+---------+
             LAB-NET

The internal network is separated from the normal physical LAN.

# 4. Kali Linux

Role:

Security / diagnostic workstation.

Primary uses:

- security tooling
- network diagnostics
- traffic inspection
- client-side testing
- future offensive-security labs

Current configuration:

- ARM64 guest
- 2 vCPU
- 4096 MB RAM
- 64 MB video memory
- Adapter 1: NAT
- Adapter 2: Internal Network `LAB-NET`

Internet connectivity is operational.

Internal lab connectivity is operational.

# 5. Ubuntu Server

Logical hostname:

`srv-linux-01`

Role:

Primary Linux server.

Primary uses:

- Linux administration
- SSH
- Bash
- Python services
- systemd
- networking
- future PostgreSQL
- future Nginx
- future Docker workloads

Current network configuration:

- Adapter 1: NAT
- Adapter 2: Internal Network `LAB-NET`

The internal interface was initially inactive and was subsequently configured and brought online.

SSH access has been configured and tested.

Internet connectivity is operational.

Internal lab connectivity is operational.

# 6. Windows 11

Logical role:

Windows workstation.

Platform:

Windows 11 ARM

Primary uses:

- Windows administration
- PowerShell
- Windows networking
- services
- event logs
- firewall
- future enterprise identity labs

Current network architecture:

- Adapter 1: NAT
- Adapter 2: Internal Network `LAB-NET`

Internet connectivity is operational.

Internal lab connectivity is operational.

# 7. Connectivity

The basic HomeLab network has been validated.

The three virtual machines can communicate through the isolated `LAB-NET`.

This establishes the first multi-platform lab environment:

    Kali Linux
        ↕
    Ubuntu Server
        ↕
    Windows 11

The environment can now support practical cross-platform networking and troubleshooting scenarios.

# 8. Current Capabilities

HomeLab v1 currently supports:

- Linux virtualization on Apple Silicon
- Windows ARM virtualization
- multi-VM operation
- isolated VM-to-VM networking
- controlled Internet access through NAT
- SSH administration
- Linux server practice
- Windows workstation practice
- Kali-based diagnostics
- cross-platform networking experiments

# 9. HomeLab v1 Status

The core HomeLab v1 infrastructure is operational.

The original design goal of establishing a small multi-platform virtual infrastructure has been achieved.

Future infrastructure should now be added only when required by the learning roadmap.

The lab should evolve through actual engineering tasks rather than through unnecessary infrastructure expansion.

# 10. Next Use

The immediate next stage is to begin using the environment for the engineering roadmap.

The HomeLab will first support:

    Sprint 1
    CS Foundations through Python

and then increasingly participate in:

    Sprint 2
    Python Engineering Foundations

    Sprint 3
    Linux Fundamentals + Bash

    Sprint 4
    Linux Systems & Networking

Later stages will introduce services, databases, containers, monitoring and additional infrastructure.
