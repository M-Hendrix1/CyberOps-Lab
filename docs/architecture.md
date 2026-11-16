# Lab architecture

**Status: Planned.** This page describes the target design. Update it with observed details only after the lab is built and validated.

## Scope

- **Host:** Windows 11 Home PC; hardware virtualization is enabled; 250–500 GB SSD space is available.
- **Virtualization:** Oracle VirtualBox is the selected hypervisor.
- **Lab network:** Isolated VirtualBox network for lab systems, with no inbound exposure from the public internet.
- **SIEM:** Planned Ubuntu Server VM running Wazuh.
- **Endpoints:** Planned Windows and Linux VMs monitored by Wazuh agents.
- **Operations:** Detection and response exercises mapped to MITRE ATT&CK.

## Planned traffic flow

1. Windows and Linux lab endpoints generate system and security events.
2. Wazuh agents forward telemetry over the isolated lab network.
3. The Ubuntu Server Wazuh system stores and presents the events for investigation.
4. The analyst documents validated alerts, response actions, and sanitized evidence.

This is a conceptual flow, not a deployed topology. Add the selected VirtualBox network mode, subnet, VM sizing, and verified connectivity results after testing. Do not publish real public IP addresses, credentials, or sensitive host details.

## Validation checklist

- [ ] Confirm the lab network is separate from the household or production network.
- [ ] Confirm only intended lab systems can communicate.
- [ ] Record VM CPU, memory, and disk allocations.
- [ ] Record OS and application versions after installation.
- [ ] Verify an endpoint event reaches Wazuh before marking monitoring operational.

## Change log

| Date | Change | Evidence |
| --- | --- | --- |
| TBD | Record verified design changes here | Link to sanitized evidence |
