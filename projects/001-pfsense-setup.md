# 001 - Building My First pfSense Network

## Goal

Build my own network that I could learn on without changing my parents' setup.

## Hardware Used

* Minisforum MS-01
* Netgear EX6120
* Netgear MS510TXM Managed Switch

## Challenges

* WAN kept showing "No Carrier"
* I wasn't sure where to plug the WAN cable
* I thought the EX6120 was acting as my router
* Suricata wasn't detecting my Nmap scan

## What I Learned

* "No Carrier" usually means there isn't a physical Ethernet connection.
* The EX6120 is a wireless bridge that brings my parents' Wi-Fi connection into pfSense.
* pfSense became the actual router for my lab once the WAN was connected correctly.
* An IDS only sees traffic that crosses the interface it's monitoring, which is why my LAN Nmap scan didn't trigger alerts on the WAN interface.

## Next Time

* Label cables before plugging everything in.
* Draw the network before I start configuring it.
* Verify which interface is WAN before changing settings.
* Test each component one step at a time instead of changing multiple things at once.
