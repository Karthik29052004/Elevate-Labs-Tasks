
# Elevate Labs – Task 3 (Basic Vulnerability Scan on Local PC)

**Task:** Basic Vulnerability Scan on Local PC

**Overview:**

In this task, I performed a vulnerability assessment of my local machine using Nessus Essentials, a free vulnerability scanner. The goal was to identify common vulnerabilities, understand their severity, and document potential risks and mitigations.

**Tools Used:**

Nessus Essentials – free vulnerability scanning tool

Web browser – to access Nessus web interface

Linux system – as the scan target

**Steps Followed:**

1. Installed Nessus Essentials

---> Downloaded Nessus from the official website.

---> Installed it on my local machine and created a user account.

2. Configured Scan Target

---> Set my localhost IP / local machine IP as the scan target.

---> Verified connectivity to ensure the scanner could reach the host.

3. Started Full Vulnerability Scan

---> Selected Basic Network Scan template.

---> Launched the scan and waited for completion (~30–60 minutes).

4. Reviewed Scan Results

---> Checked detected vulnerabilities, grouped by severity: Critical, High, Medium, Low, Mixed, and Info.

---> Noted additional hosts or services detected (extra IPs reported by Nessus).

---> Paid special attention to critical/high vulnerabilities for reporting.

5. Analyzed Key Findings

---> Identified outdated Node.js versions and followed Nessus recommendations for secure versions.

---> Checked IP forwarding settings and disabled it as a security measure.

---> Reviewed informational findings like DHCP information disclosure to understand network exposure.

6. Documented and Captured Evidence

---> Took screenshots of the scan summary, top vulnerabilities, and critical findings.

---> Exported Nessus report in PDF format for reference.

7. Researched Mitigations

---> For each critical/high vulnerability, researched official fixes or recommended upgrades.

---> Documented recommended actions for system hardening.


**Outcome:**

---> Gained hands-on experience in performing a basic vulnerability scan.

---> Learned how Nessus categorizes vulnerabilities using CVSS, VPR, EPSS, and severity levels.

---> Identified potential risks and understood how to prioritize remediation based on severity and exploit likelihood.

---> Developed skills in documenting findings and preparing a concise vulnerability report.



