# Task 3 — Vulnerability Assessment

## Objective
Perform a basic vulnerability scan of a Windows 7 virtual machine using Nessus Essentials from the host machine, identify security issues, and document the findings.

## Environment
- **Scanning Tool:** Nessus Essentials (Basic Network Scan)
- **Scanner Host:** Windows 11 (Host machine)
- **Target Machine:** Windows 7 (VMware Workstation)
- **Target IP:** 192.168.91.129
- **Network Mode:** Host-only Adapter

## Steps Performed
1. Configured VMware networking to allow communication between host and VM.
2. Verified target connectivity with `ping` and `nmap` scan.
3. Installed and launched Nessus Essentials on the host machine.
4. Created a new **Basic Network Scan** in Nessus with the target IP.
5. Ran the scan and waited for completion.
6. Exported results and captured screenshots for documentation.

## Scan Details
- **Policy:** Basic Network Scan
- **Scanner:** Local Scanner
- **Status:** Completed
- **Total Vulnerabilities Found:** 39  
  - Critical: 1
  - High: 1
  - Medium: 2
  - Low: 1
  - Info: 34

## Files in this folder
- `README.md` — Scan process and setup details.
- `vulnerability_report.md` — Summary of vulnerabilities and recommendations.
- `scan_screenshot.png` — Screenshot of Nessus results dashboard.




