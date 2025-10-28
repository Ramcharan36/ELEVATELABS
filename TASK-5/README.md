Task 5: Capture and Analyze Network Traffic Using Wireshark
🎯 Objective



To capture live network packets, identify different network protocols, and analyze traffic using Wireshark.

🧰 Tools Used
Wireshark (Free, Open Source)
⚙️ Steps Performed
Installed Wireshark from the official website.
Started live capture on the active network interface (Wi-Fi).
Generated traffic by:
Browsing websites like google.com and github.com
Running the command:
ping www.google.com

Stopped capture after one minute.
Filtered packets by protocol using filters such as http, dns, and tcp.
Saved the capture as network_capture_task5.pcap.
Analyzed the captured packets to identify different protocol types and behavior.
🔍 Protocols Identified
Protocol	Description	Example Observation
DNS	Used to resolve domain names into IP addresses.	Query for www.google.com.
TCP	Connection-oriented protocol ensuring reliable data transmission.	TCP Handshake: SYN → SYN-ACK → ACK
HTTP	Used for web communication between browser and server.	GET / HTTP/1.1 request sent to Google.
ICMP	Used for network diagnostics (ping).	Echo request and reply to 8.8.8.8.
📊 Packet Summary
Total Packets Captured: ~800
Top Protocols: TCP (65%), DNS (20%), HTTP (15%)
Average Packet Size: ~74 bytes
Traffic Type: Mostly browsing and ICMP echo requests.
🧩 Observations
DNS requests occur before HTTP traffic to resolve domain names.
TCP establishes a three-way handshake before data transfer.
HTTP packets show successful GET requests and responses.
ICMP packets confirm connectivity and latency.
🧾 Conclusion



Wireshark provides detailed insights into live network communications.
By analyzing captured packets, one can understand how protocols interact within the TCP/IP stack and detect potential network or configuration issues.