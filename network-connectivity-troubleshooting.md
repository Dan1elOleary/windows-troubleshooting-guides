# Network Connectivity Troubleshooting Guide

This guide outlines a structured process for troubleshooting common Windows network connectivity issues. Network issues may involve Wi-Fi, Ethernet, DNS, DHCP, VPN, firewall settings, network adapters, or service outages.

---

## Issue Overview

A user reports that they cannot access the internet, connect to internal resources, access shared drives, use VPN, or reach specific websites or applications.

---

## Common Symptoms

* No internet connection
* Wi-Fi connected but no internet
* Ethernet connected but no access
* Unable to access shared drives
* Unable to connect to VPN
* Websites fail to load
* DNS errors in the browser
* Slow network performance
* Network icon shows limited connectivity
* User can access some resources but not others

---

## Possible Causes

* Wi-Fi or Ethernet connection issue
* Incorrect network selected
* Bad network cable or docking station issue
* DHCP issue
* DNS resolution issue
* VPN client problem
* Firewall or security software blocking traffic
* Network adapter disabled
* Outdated network driver
* Router, switch, or access point issue
* ISP or site outage
* Internal server or application outage

---

## Initial Questions to Ask the User

* Are you using Wi-Fi, Ethernet, or VPN?
* Are other users having the same issue?
* Can you access any websites?
* Can you access internal resources?
* When did the issue start?
* Did anything change recently?
* Are you working onsite or remotely?
* Are you receiving an error message?
* Have you restarted the computer or network connection?

---

## Troubleshooting Steps

### 1. Confirm the Scope of the Issue

Determine whether the issue affects:

* One user
* One device
* Multiple users
* One location
* One application
* All network resources

If multiple users are affected, the issue may be related to the network, firewall, ISP, VPN service, or internal infrastructure.

---

### 2. Check Physical and Wireless Connection

For Ethernet:

* Confirm the cable is connected.
* Try a different network cable.
* Check the docking station if one is being used.
* Confirm link lights if available.

For Wi-Fi:

* Confirm Wi-Fi is enabled.
* Confirm the user is connected to the correct wireless network.
* Forget and reconnect to the network if needed.
* Move closer to the access point if signal is weak.

---

### 3. Restart the Network Connection

Basic restart steps may include:

1. Disconnect and reconnect Wi-Fi or Ethernet.
2. Disable and re-enable the network adapter.
3. Restart the VPN client if applicable.
4. Restart the computer.
5. Restart home network equipment if the user is remote and approved to do so.

---

### 4. Check IP Address Information

Use Command Prompt to review network configuration.

Command:

ipconfig /all

Review:

* IPv4 address
* Default gateway
* DNS servers
* DHCP status
* Network adapter name
* Connection state

Common findings:

* 169.254.x.x address usually indicates DHCP failure.
* Missing default gateway may prevent network access.
* Incorrect DNS servers may cause name resolution issues.

---

### 5. Test Basic Connectivity

Use ping tests to narrow the issue.

Examples:

* Ping the default gateway.
* Ping a known public IP address.
* Ping an internal server if applicable.
* Ping a website name to test DNS.

Example commands:

ping 8.8.8.8

ping google.com

If pinging an IP works but pinging a name fails, the issue may be DNS-related.

---

### 6. Check DNS Resolution

Use nslookup to test DNS.

Command:

nslookup google.com

If DNS fails, possible causes include:

* Incorrect DNS server
* VPN DNS issue
* Local DNS cache problem
* Internal DNS outage
* Network policy issue

A possible basic fix is to flush DNS.

Command:

ipconfig /flushdns

---

### 7. Renew the IP Address

If DHCP appears to be the issue, release and renew the IP address.

Commands:

ipconfig /release

ipconfig /renew

Then confirm the updated IP configuration.

Command:

ipconfig /all

---

### 8. Check VPN Connectivity

For VPN-related issues, confirm:

* User has internet before connecting to VPN
* VPN client opens correctly
* MFA prompt is received if required
* User account is not locked
* VPN profile is correct
* Error message is documented
* Internal resources are reachable after connection

If the internet works but internal resources fail only on VPN, the issue may involve VPN routing, DNS, permissions, or internal access policies.

---

### 9. Check Network Adapter Status

Review the adapter in Windows.

Useful areas:

* Settings > Network & internet
* Control Panel > Network Connections
* Device Manager > Network adapters

Check for:

* Disabled adapter
* Driver warning icon
* Missing adapter
* Outdated driver
* Airplane mode enabled

---

## Resolution Notes

Document the final cause and fix.

Example:

The user was unable to access internal resources because the VPN client was connected but DNS was not resolving internal hostnames. The VPN client was restarted, DNS cache was flushed, and the user reconnected successfully. Internal resources were accessible after reconnecting.

---

## Escalation Points

Escalate the issue if:

* Multiple users are affected
* Network hardware may be down
* VPN service is unavailable
* DNS or DHCP services may be failing
* Firewall rules may be blocking traffic
* The device cannot obtain a valid IP address
* Network adapter driver repair does not resolve the issue
* Internal infrastructure access requires higher-level review

---

## User-Facing Response Example

Hello,

I reviewed the network connectivity issue and confirmed that the device was connected to the network but was not resolving network resources correctly. I refreshed the network connection, cleared the DNS cache, and confirmed that access was restored.

Please let us know if the issue happens again or if you lose access to any specific resources.
