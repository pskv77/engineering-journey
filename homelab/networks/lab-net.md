# LAB-NET

Status: Operational

Type:

VirtualBox Internal Network

Name:

`LAB-NET`

## Purpose

LAB-NET is the isolated internal network used by HomeLab virtual machines.

It provides east-west communication between lab systems without exposing the internal lab network directly to the physical LAN.

## Current Members

- Kali Linux
- Ubuntu Server (`srv-linux-01`)
- Windows 11 ARM

## Network Model

Each machine uses:

    NIC 1 → NAT
    NIC 2 → LAB-NET

NAT provides external connectivity.

LAB-NET provides internal lab connectivity.

## Current Capabilities

The network supports:

- VM-to-VM communication
- Linux / Windows interoperability
- SSH
- client-server experiments
- network troubleshooting
- future application services
- future firewall experiments

## Future Evolution

LAB-NET is intentionally simple.

Future roadmap stages may introduce dedicated logical networks such as:

    USERS
    SERVERS
    DMZ
    MANAGEMENT

Segmentation will be introduced when required by networking and security labs rather than added prematurely.
