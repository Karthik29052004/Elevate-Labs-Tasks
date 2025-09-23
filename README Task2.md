
# Elevate Labs – Task 2 (Analyze a Phishing Email Sample)

**Task:** Analyze a Phishing Email Sample

**Overview:**

This project demonstrates a step-by-step analysis of a suspicious email to identify phishing characteristics. The main goal is to understand how phishing emails work, recognize social-engineering tactics, and learn safe methods to inspect email headers, links, and attachments.

Through this task, I have developed practical skills in email threat analysis, including the use of free tools for verification and evidence collection.

**Tools Used:**

MXToolbox – Used to analyze email headers, check SPF/DKIM/DMARC authentication results, and identify anomalies in the sending server chain.

VirusTotal – Used to scan suspicious URLs and attachments to detect potential malware or phishing threats.

Cloudflare Radar – Used to examine the domain reputation and recent activity of suspicious URLs for additional threat context.

**Steps Followed:**

1. Obtained the email sample

Saved the suspicious email in .eml format for safe analysis.

Collected raw headers and all visible links and attachments.

2. Header Analysis with MXToolbox

Checked SPF, DKIM, and DMARC results.

Examined Received headers to verify the origin IP and sending servers.

Noted mismatched domains or suspicious Message-ID entries.

3. URL & Domain Verification

Extracted actual URLs from the email without clicking.

Scanned URLs using VirusTotal to check for phishing or malware.

Used Cloudflare Radar to inspect domain reputation and traffic trends.

4. Social Engineering & Content Inspection

Reviewed email body for urgency, threatening language, generic greetings, and suspicious requests.

Identified mismatches between visible links and actual destinations.

5. Report Preparation

Compiled findings into a structured report including:

---> Header analysis results

---> Suspicious links and attachments

---> Social-engineering indicators

---> IOCs (Indicators of Compromise)



**Outcome:**

By completing this task, I gained practical experience in:

---> Analyzing email headers for spoofing and authentication failures.

---> Safely inspecting suspicious links and attachments.

---> Detecting phishing attempts using a combination of technical and social-engineering indicators.

---> Documenting findings clearly in a professional report format.

This task strengthens awareness of phishing tactics and improves email threat analysis skills, which are critical in cybersecurity operations.

