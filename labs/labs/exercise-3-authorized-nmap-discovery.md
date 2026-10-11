Exercise 3 — Authorized Discovery with Nmap

Objective

Learn how to verify a target VM, discover live hosts on an authorized lab network, identify exposed services, and document scan results.

1. Verify the Target

Target VM: Windows virtual machine (target configuration and suitability to be confirmed).

Target IPv4 address: Pending verification.

The target's IP address must be obtained from the target VM itself. The loopback address 127.0.0.1 must not be used as the target's network address.

2. Perform Basic Host Discovery

Tool: Nmap

Command format:
nmap -sn <LAB-SUBNET/CIDR>

The subnet must be verified from the lab network configuration before running host discovery.

Lab subnet: Pending verification.

Hosts discovered: Pending results.

3. Scan the Authorized Target

Command format:
nmap -sV <TARGET-IP>

The target IP must be replaced with the verified IP address of the authorized lab VM. Angle brackets are placeholders and must not be typed into the command.

Scan status: Pending a verified target and confirmed network connectivity.

4. Read and Document the Results

For each open port, record:

Port number and protocol

Service name

Version, if reported

Why the service matters

Evidence from the actual Nmap output

Observed open ports: Pending scan results.

5. Key Lessons

Host discovery identifies which hosts appear to be reachable.

Nmap's -sV option attempts to identify services and their versions.

An open port does not automatically indicate a vulnerability.

Scanning must remain within the authorized lab environment.

The Kali VM's previously observed address was 10.0.2.15/24, with default gateway 10.0.2.2. The target network still needs to be verified.
