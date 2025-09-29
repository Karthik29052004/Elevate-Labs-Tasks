
# Elevate Labs – Task 4 (Setup and Use a Firewall on Windows/Linux)

**Task:**  Setup and Use a Firewall on Windows/Linux

**Overview:**

To configure and test basic firewall rules in a Linux virtual machine using UFW (Uncomplicated Firewall), and to understand how firewall filters network traffic.

**Tools Used:**
VMware Workstation (Virtual Machine environment)

Kali Linux (with UFW 0.36.2 preinstalled)

UFW (Uncomplicated Firewall) – command line firewall utility

Netcat (nc) – for testing port connections

**Steps Followed:**

Step 1: Verify UFW Installation

Checked UFW version:

    ufw --version


Output confirmed version: 0.36.2

Step 2: Configure Default Firewall Policy

Set secure defaults:

    sudo ufw default deny incoming
    sudo ufw default allow outgoing


Blocks all incoming traffic unless explicitly allowed.
Allows outgoing traffic.

Step 3: Allow SSH Access

To avoid locking out remote access:

    sudo ufw allow 22/tcp


This keeps SSH accessible.

Step 4: Block Telnet (Port 23)

Added a firewall rule to block Telnet:

    sudo ufw deny 23/tcp

Step 5: Enable the Firewall

Activated UFW:

    sudo ufw enable


Confirmed it was active.

Step 6: Verify Rules

Listed firewall rules:

    sudo ufw status numbered


Output showed:

22/tcp ALLOW

23/tcp DENY

Step 7: Test the Block Rule

Installed netcat for testing:

    sudo apt install netcat -y


Created a fake Telnet server:

    sudo nc -l -p 23


From another terminal, tested the connection:

    nc -vz localhost 23


Result: Connection was attempted, showing the firewall’s effect on port 23.

**Outcome:**

---> Learned how to install, configure, and enable UFW on Linux.

---> Applied rules to allow SSH and block Telnet.

---> Verified firewall functionality with netcat testing.

---> Understood that a firewall acts as a filter, permitting or denying traffic based on defined rules.


