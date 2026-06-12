# 002 - Configuring My AX80 as an Access Point

## Goal

Add Wi-Fi to my lab without creating another router or a double NAT situation.

## Hardware Used

* TP-Link Archer AX80
* Netgear MS510TXM Managed Switch
* Minisforum MS-01 running pfSense

## Challenges

* I wasn't sure if I should use Router Mode or Access Point Mode.
* The setup wizard reported that the internet port was disconnected.
* I had trouble accessing the management page at first.

## What I Learned

* Running the AX80 in Access Point mode lets pfSense stay in control of routing and DHCP.
* Access Point mode extends my network instead of creating a second one.
* The WAN port on the AX80 isn't needed when it's acting as an Access Point.
* Devices connected to the AX80 are still part of the same LAN managed by pfSense.

## Next Time

* Put the device in Access Point mode before changing other settings.
* Give the AX80 a static management IP so it's easy to find later.
* Document the management IP and login location in my network diagram.
