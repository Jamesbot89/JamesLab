# 003 - Monitoring My Network with Suricata

## Goal

Learn how an intrusion detection system (IDS) works and monitor traffic on my home network.

## Hardware Used

* Minisforum MS-01 running pfSense

## Software Used

* Suricata

## Challenges

* My Nmap scan didn't create any alerts.
* I thought Suricata would see every packet on my network.
* I wasn't sure if Suricata was configured correctly or if I misunderstood how it worked.

## What I Learned

* Suricata only sees traffic that crosses the interface it's monitoring.
* If Suricata is only watching the WAN interface, LAN-to-LAN traffic won't generate alerts.
* Seeing alerts doesn't automatically mean something is malicious. It's important to understand what the alert is actually telling me.
* Testing and troubleshooting are the best ways to understand how security tools work.

## Next Time

* Test Suricata with traffic that actually crosses the monitored interface.
* Experiment with monitoring different interfaces.
* Research the difference between IDS and IPS and when to use each.
