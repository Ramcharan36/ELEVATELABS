# Task 4 – Firewall Configuration (Windows)

**Objective:**  
Configure and test firewall rules to allow or block network traffic.

**Tools:**  
Windows Defender Firewall (wf.msc)

**Steps:**  
1. Viewed current inbound/outbound rules.  
2. Created a rule to block TCP Port 23 (Telnet).  
3. Tested and verified the connection was blocked.  
4. Removed the test rule to restore defaults.

**Commands Used:**  
netsh advfirewall firewall add rule name="Block Telnet" dir=in action=block protocol=TCP localport=23  
netsh advfirewall firewall delete rule name="Block Telnet"  

**Screenshots:**  
- Firewall rules window  
- New rule creation window  
- Telnet blocked output  

**Conclusion:**  
Firewall successfully blocked unwanted traffic and protected the system.
