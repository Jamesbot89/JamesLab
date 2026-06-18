# 007 - Deploying Pi-hole DNS Filtering

## Goal

Deploy Pi-hole in Docker and use it as the DNS server for my lab network.

## Hardware Used

* Raspberry Pi 4
* Minisforum MS-01 (pfSense)

## Software Used

* Docker
* Portainer
* Pi-hole
* pfSense

## Challenges

* Pi-hole installed successfully, but DNS queries timed out.
* Queries were being ignored as "non-local network" requests.
* My laptop was still using pfSense for DNS instead of Pi-hole.
* I had to troubleshoot Docker networking and Pi-hole listening settings.

## What I Learned

* DNS requests use port 53.
* Docker containers can have networking restrictions that affect services.
* Pi-hole listening modes determine which clients can query the server.
* DHCP controls which DNS server clients receive.
* Query logs are extremely useful for troubleshooting.
* Pi-hole can be integrated with pfSense to provide network-wide DNS filtering.

## Result

* Successfully deployed Pi-hole in Docker.
* Configured Pi-hole to accept DNS requests from my lab network.
* Configured pfSense DHCP to hand out Pi-hole as the DNS server.
* Verified DNS queries from lab devices appeared in the Pi-hole Query Log.
* Added DNS filtering and visibility to JamesLab.

## Next Time

* Configure DNS filtering policies.
* Learn more about DNS records and local DNS entries.
* Explore blocklists and custom allowlists.
* Integrate Pi-hole into a Homepage Dashboard.
