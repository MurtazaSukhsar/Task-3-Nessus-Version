# 🛡️ Task 3: Vulnerability Scan on Windows 7 (OpenVAS Version)

## 🎯 Objective
Perform a basic vulnerability assessment on a Windows 7 virtual machine using Kali Linux and OpenVAS (GVM).

---

## 🧰 Tools Used
- Kali Linux (Scanner)
- Windows 7 VM (Target)
- OpenVAS / Greenbone Vulnerability Manager (GVM)
- Nmap (initial port discovery)

---

## 🖥️ Network Setup
- **Kali IP:** 192.168.71.X
- **Windows 7 IP:** 192.168.71.133
- **Connection Type:** Bridged (VMware)
- **Firewall:** Temporarily disabled to allow scanning

---

## 🔍 Steps Performed

1. Installed OpenVAS on Kali:
   ```bash
   sudo apt install openvas -y
   sudo gvm-setup
   sudo gvm-start
   ```

2. Accessed OpenVAS Web UI at:
   ```
   https://localhost:9392
   ```

3. Created a target in GVM: `192.168.71.133`

4. Launched a scan task named: `Windows 7 Scan`

5. After the scan finished:
   - Exported report as PDF
   - Took screenshot of summary report

---

## 📋 Summary of Findings (Example)

- **Total Vulnerabilities Found:** 20
- **Critical:** 4
- **High:** 6
- **Medium:** 8
- **Low:** 2

Example Critical Issues:
- SMBv1 Vulnerability (EternalBlue)
- Weak RDP Configuration
- Missing Security Patches
- Outdated IE version

---

## 📁 Folder Structure

```
Task-3-OpenVAS-Version/
├── README.md
├── vulnerability_report.md
├── openvas_win7_scan.pdf
└── screenshots/
    └── openvas_summary.png
```

---

---

## ✅ Outcome

This task helped me understand how to scan and analyze real system vulnerabilities using open-source tools like OpenVAS.