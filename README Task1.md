
# Elevate Labs – Task 1 (Scan Your Local Network for Open Ports)

**Task:** Scan your local network for open ports on Linux

**Overview:**

For this task, I learned the basics of network reconnaissance. The goal was to identify which TCP ports were open on devices in my local network, observe the packets generated during the scan, and understand what services were running.

**Tools Used:**

Nmap (pre-installed on Linux)

Wireshark or tcpdump (for capturing and inspecting network traffic)

**Steps Followed:**

1. Checked that Nmap was available on the system using nmap --version.

2. Found my IP address and subnet using ip addr (my IP was 192.168.x.x with a /24 subnet).

3. Ran a TCP SYN scan across the subnet:
sudo nmap -sS 192.168.x.0/24

4. Saved the scan results to a text file:
sudo nmap -sS 192.168.x.0/24 -oN scan_results.txt

5. Captured network packets while the scan was running using Wireshark or tcpdump -i <interface>.

6. Applied filters like tcp or tcp.flags.syn==1 to focus on SYN/SYN-ACK handshakes.

7. Looked up the services behind the open ports (e.g., 22 → SSH, 80 → HTTP).

8. Noted which open services could pose potential risks and documented all findings.

**Outcome:**
I gained hands-on experience with network scanning on Linux, learned how to read open ports and associated services, and practiced using packet capture tools to observe network traffic.

