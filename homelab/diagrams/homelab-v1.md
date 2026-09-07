# HomeLab v1 Diagram

```mermaid
flowchart TB
    Internet((Internet))

    NAT[VirtualBox NAT]

    Kali[Kali Linux]
    Ubuntu[Ubuntu Server<br/>srv-linux-01]
    Windows[Windows 11 ARM]

    LAB[LAB-NET<br/>VirtualBox Internal Network]

    Internet --> NAT

    NAT --> Kali
    NAT --> Ubuntu
    NAT --> Windows

    Kali --- LAB
    Ubuntu --- LAB
    Windows --- LAB
```

## Network Model

Each virtual machine has two network adapters:

    Adapter 1 → NAT
    Adapter 2 → LAB-NET

NAT is used for Internet connectivity.

LAB-NET is used for isolated communication between HomeLab systems.
