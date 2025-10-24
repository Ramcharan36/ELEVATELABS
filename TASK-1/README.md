# Task 1 — Local Network Port Scan Report

**Student:** CHILUMURI. SREE RAM SAI CHARAN  
**Date:** 20 October 2025  
**Tools:** Nmap 7.98 (Windows), Npcap

## Objective
Scan local network interfaces to discover open ports and services, assess exposure, and recommend mitigations.

## Environment
- Wi‑Fi IPv4: 192.168.1.35 (home LAN)  
- VirtualBox host-only adapter: 192.168.56.1 (scanned)

## Key Findings
- Target scanned: 192.168.56.1 (VirtualBox host-only). Host up: **192.168.56.1**.  
- Notable open ports: `135, 137 (filtered), 139, 445, 5040, 8000, 8089, 8191, 9997, 49664-49678`.  
- Services: Windows RPC (msrpc), NetBIOS/SMB, and Splunk (Splunkd httpd on 8000/8089).

## Risk Assessment
- SMB/NetBIOS (139/445): medium–high risk if exposed on real LAN.  
- Splunk ports (8000/8089/9997): secure with auth & limit to trusted hosts.

## Recommendations
1. Rescan your real LAN: `nmap -sS -sV -O -T4 --open -oA myscan_wifi 192.168.1.0/24`.  
2. If SMB/NetBIOS are not needed, block them on Windows:
3. Restrict Splunk to localhost or trusted IPs; enable authentication and TLS.
4. Patch OS and apps; re-scan after fixes.

## Files included
- scan_results.txt (raw output)  
- README.md  
