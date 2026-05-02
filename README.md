# Ransomware Incident Response Playbook

A complete, portfolio-grade Incident Response playbook for ransomware attacks. Built on NIST SP 800-61r2 with MITRE ATT&CK technique mapping and Wazuh SIEM detection rule references. Designed to be handed directly to a hiring manager or CISO.

---

## What This Playbook Covers

All 6 phases of the NIST SP 800-61 incident response lifecycle, tailored specifically for ransomware:

| Phase | Focus |
|-------|-------|
| 1 - Preparation | Roles, pre-incident requirements, asset documentation |
| 2 - Detection and Analysis | Wazuh rule IDs, Triage checklist, query commands |
| 3 - Containment | Host isolation CLI commands, network blocking, process termination |
| 4 - Eradication | Persistence removal, credential reset, malware scanning |
| 5 - Recovery | Restore priority order, backup validation, decryption options |
| 6 - Post-Incident Activity | Reporting requirements, 30-day hardening sprint, lessons learned |

---

## Key Features

**Wazuh SIEM Detection Table**
14 specific Wazuh rule IDs mapped to ransomware behavior — from FIM mass-modification alerts (Rule 87103) to VSS shadow copy deletion (Rule 31168), the highest-confidence ransomware indicator in the framework.

**MITRE ATT&CK Integration**
16 techniques mapped across the full ransomware kill chain: T1566 (Phishing), T1490 (Inhibit System Recovery), T1486 (Data Encrypted for Impact), T1489 (Service Stop), and more. Each technique includes Wazuh detection guidance.

**CLI Command Reference**
Ready-to-use commands for every containment and eradication action:
- Linux iptables host isolation
- Windows PowerShell firewall rules
- Process termination (Linux and Windows)
- Persistence hunting (cron, registry, WMI subscriptions, systemd)
- Backup validation and restore

**Lessons Learned Template**
Structured post-incident template with incident timeline fields, root cause analysis, action item tracking table, and sign-off section.

---

## Output

Single self-contained HTML file (`ransomware_ir_playbook.html`) with:
- Dark cybersecurity theme
- Color-coded phases (blue, amber, orange, red, green, purple)
- Table of contents with anchor navigation
- Print-ready layout

Open in any browser -- no dependencies, no build step required.

---

## How to Use

```bash
# Clone the repo
git clone https://github.com/Bphavin1/ransomware-ir-playbook.git

# Open the playbook
open ransomware_ir_playbook.html
```

To customize for your organization:
- Update role names in Phase 1
- Replace Wazuh IP (10.0.0.130) with your SIEM address
- Add your org-specific crown jewel assets to the Pre-Incident Requirements section
- Populate the Lessons Learned template after each incident

---

## Frameworks Referenced

- NIST SP 800-61 Rev. 2 — Computer Security Incident Handling Guide
- MITRE ATT&CK Enterprise — Ransomware technique mapping
- MITRE ATT&CK ATLAS — AI threat considerations
- Wazuh Open Source SIEM — Detection rule references

---

## Skills Demonstrated

- Incident response planning and playbook development
- NIST SP 800-61 lifecycle implementation
- MITRE ATT&CK framework application
- Wazuh SIEM tuning and detection engineering
- Linux and Windows forensic command-line proficiency
- Technical documentation for executive and operational audiences

---

## Author

**Brian Pascal**
GRC and Third-Party Risk Manager | AI Governance | NIST CSF | CompTIA Security+
GitHub: [github.com/Bphavin1](https://github.com/Bphavin1)
LinkedIn: [linkedin.com/in/brianpascalsecurity](https://linkedin.com/in/brianpascalsecurity)
