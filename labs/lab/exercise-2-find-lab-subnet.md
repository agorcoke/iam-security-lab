Exercise 2 — Find Your Own Lab Subnet

Objective

Identify the Kali Linux virtual machine's IP address, active network interface, subnet, and default gateway.

1. Display IP Configuration

Command:
ip addr

Observed results:

Active interface: eth0

IPv4 address: 10.0.2.15

Prefix length: /24

Broadcast address: 10.0.2.255

Interface state: UP

Explanation:
The eth0 interface is active and has been assigned the IPv4 address 10.0.2.15/24. The /24 prefix corresponds to the subnet mask 255.255.255.0.

2. Identify the Route

Command:
ip route

Observed results:

Default gateway: 10.0.2.2

Network route: 10.0.2.0/24

Interface: eth0

Source address: 10.0.2.15

Explanation:
The default route sends traffic for destinations without a more specific route through gateway 10.0.2.2. The directly connected route identifies the 10.0.2.0/24 network.

3. Network Assessment

The IP configuration indicates that Kali Linux is using the 10.0.2.0/24 subnet. This address range is commonly used by VirtualBox NAT networking. The VirtualBox network mode and connectivity to any target VM must be verified before conducting further lab tests.

4. Key Lessons

ip addr displays network interfaces and assigned addresses.

ip route displays routing information.

eth0 is the active interface observed in this exercise.

127.0.0.1 is the loopback address and is not the lab network address.

A VM's assigned IP address alone does not establish that it can communicate directly with another VM.
