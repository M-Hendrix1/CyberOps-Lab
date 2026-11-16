# CyberOps Lab

A portfolio project for building and documenting an isolated cybersecurity operations lab on a Windows 11 Home PC.

> **Current state:** Project planning and lab bring-up. The tools and capabilities below are in scope; their mention does not mean they are installed or deployed. Update this README as each capability is verified.

## Objectives

- Build an isolated virtual lab using Oracle VirtualBox.
- Prepare an Ubuntu Server VM as the planned host for Wazuh SIEM.
- Add Windows and Linux endpoints for security monitoring.
- Develop and validate detections mapped to MITRE ATT&CK.
- Practice incident triage, response, and evidence-based reporting.
- Publish clear, sanitized documentation suitable for a technical portfolio.

## Host readiness

- Operating system: Windows 11 Home
- Hardware virtualization: Enabled
- Available SSD space: 250–500 GB

## Verified progress

- **VirtualBox 7.2.22:** Installed on the Windows 11 Home host; VirtualBox Manager opened successfully on 2026-11-16.
- No virtual machine has been created yet.

## Planned architecture

The intended lab contains a VirtualBox isolated network, an Ubuntu Server system for Wazuh, and monitored Windows and Linux endpoints. Network design and VM sizing are documented in [the architecture notes](docs/architecture.md). This is a target design, not a deployed topology.

## Work tracking

Planning uses two-week Scrum sprints in Jira:

- [CyberOps-Lab project and backlog](https://mauricehendrix0.atlassian.net/jira/software/projects/SCRUM/summary)
- Sprint 1 focuses on infrastructure and virtualization.

## Documentation

See [docs/README.md](docs/README.md) for the documentation map.

## Safety and evidence

Keep the lab network isolated from production devices. Never commit credentials, tokens, personal data, public IP addresses, or unredacted screenshots. Sanitize hostnames and network details before publishing evidence.

## Project status

| Capability | Status |
| --- | --- |
| Windows host readiness | Confirmed |
| VirtualBox installation | Verified: 7.2.22; Manager opened successfully |
| Isolated lab network | Planned |
| Ubuntu Server VM | Planned |
| Wazuh SIEM | Planned |
| Windows/Linux endpoint monitoring | Planned |
| ATT&CK detections and incident response | Planned |
| Portfolio evidence | Planned |
