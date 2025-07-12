# MITRE ATT&CK Mapping in Splunk

This project demonstrates how to map real-world detection use cases in Splunk to MITRE ATT&CK techniques using simulated logs.

## Covered Techniques

| Technique ID | Name                            | Use Case                       |
|--------------|----------------------------------|--------------------------------|
| T1110        | Brute Force                     | Failed login attempts          |
| T1566        | Phishing                        | Emails with suspicious content |
| T1086        | PowerShell                      | Encoded or suspicious commands |
| T1059        | Command and Scripting Interpreter | Command-line executions     |

## Dashboard Preview

<img width="766" height="477" alt="Screenshot 2025-07-12 at 9 07 03 AM" src="https://github.com/user-attachments/assets/8d99e29b-70bd-415a-95ee-554be43b9b9a" />


## Log Format

Each log entry contains:
- `src_ip`, `user`, `event`, `command`, `subject`, `attachment`, `technique`

Example:

2025-07-13 10:03:22,src_ip=192.168.1.101,user=bob,event=email_received,subject="Verify Your Account",attachment="invoice.exe",technique=T1566


## Files

- `mitre_logs.txt` – synthetic log file used for ingestion
- `README.md` – project overview and MITRE mapping
- `screenshots/dashboard.png` – dashboard image

## Tools Used

- Splunk (Free Tier)
- MITRE ATT&CK Framework
- MacBook M2 (Rosetta enabled)

---

## Author

Built by Shravan Kumar Panuganti  
For SOC analyst portfolio showcasing MITRE technique mapping in SIEM


