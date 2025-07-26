# IntermediateNetworkSecurity
<br/>s
This is a set of intermediate network security tasks!

<br/><br/>


## 🌐 TCP Port Scanner (Python)

### 🎯 Overview
A Python-based tool to check host availability and scan for open TCP ports within a configurable range. Designed for a friendly GUI, speed, and diagnostic feedback.
- 🔍 Scans individual IPs or hostnames across user-defined port ranges
- ⚙️ Validates input with clean error handling and prompt feedback
- ⏱️ Uses socket timeouts to optimize performance and detect filtered vs. closed ports
- 💬 Console interaction enhanced with status messages and result formatting
- 🛠️ Tools Used: Python 3, socket, CLI prompts
- 📊 Outcome: Confirms host reachability and port exposure, useful for diagnostics or ethical pen-testing
<br/>
  This is our home-page menu. <br/>
<img width="553" height="215" alt="image" src="https://github.com/user-attachments/assets/6ac81fb1-81a2-46e9-b90c-919e1d46540e" />

This TCP-scanner will go through the range, informing the user of open ports.
<img width="486" height="263" alt="image" src="https://github.com/user-attachments/assets/f774c0df-8aba-4256-8daa-da32169212b6" />

Port 80 (HTTP) is open on this web server, which could indicate redirection to HTTPS on port 443 for legacy browser support, or alternatively, suggest that unencrypted traffic is still being permitted.


## 📊 Skills Demonstrated

| Skill Area                | Description                                                           |
|--------------------------|-----------------------------------------------------------------------|
| 🔍 Network Reconnaissance | Created a Python TCP port scanner for identifying open services        |
| 🐍 Python Scripting       | Utilized sockets, efficient looping, and exception handling            |
| 🧪 Input Validation       | Verified user-supplied IP addresses and port ranges before scanning    |
| 🧠 Protocol Awareness     | Applied understanding of TCP behavior in port scanning methodology     |
| 🚨 Robust Error Handling  | Handled unreachable hosts and filtered ports without crashing          |



### 📁 Files Included
- demo_notes.md: Step-by-step walkthrough
- lab_topology.png: Network diagram
- wireshark_capture.pcap: Sample packet dump (sanitized)
- README.md: This overview


---



<br/><br/>
## 🔐 Nessus Essentials Lab: Vulnerability Scanning in Practice

### 🎯 Overview
This project simulates real-world vulnerability scanning using Tenable Nessus Essentials, conducted entirely within a local lab environment. It demonstrates hands-on proficiency in identifying, categorizing, and remediating security risks across simulated endpoints.

### 🧠 Why It Matters
Vulnerability assessment is the backbone of proactive cybersecurity. This lab highlights my ability to:
- Deploy and configure industry-standard tools
- Navigate authenticated scanning challenges
- Interpret CVEs and exploit paths
- Apply remediation and verify risk reduction

### 🛠️ Lab Setup
- Installed Nessus Essentials and configured scans via local web UI (`localhost:8834`)
- Designed target environments using Windows/Linux VMs with known flaws
- Tuned scan profiles for performance vs. depth

### 🔍 Key Activities
- Ran authenticated and unauthenticated scans on `192.168.x.x/24`
- Isolated high-severity vulnerabilities and tracked exploitability
- Applied OS patches and software updates to test remediation
- Logged scan deltas to confirm fix effectiveness
- Exported detailed reports for audit and review

### 📊 Skills Demonstrated
| Category            | Examples                                                      |
|---------------------|---------------------------------------------------------------|
| 🔧 Tooling Expertise | Nessus configuration, scan profile tuning, credential setup   |
| 📋 Analysis          | CVE parsing, severity triage, exploit validation               |
| 🔄 Lifecycle Testing | Scan → Fix → Re-scan workflows with patch confirmation        |
| 📁 Reporting         | Exported scan results, annotated findings, documented process |

### 📁 Files Included
- demo_notes.md: Step-by-step walkthrough
- lab_topology.png: Network diagram
- wireshark_capture.pcap: Sample packet dump (sanitized)
- README.md: This overview


---

        

<br/><br/>
## 🔍 ARP Spoofing Demonstration (Educational Lab)
### 🧠 Overview
This lab simulates an ARP spoofing attack to demonstrate vulnerabilities in local network trust models. It highlights how attackers manipulate ARP tables to intercept traffic and how security tools can detect or mitigate such behavior.
#### ⚠️ This project is strictly educational and intended for controlled lab environments. Always ensure explicit permission before testing on any network.

<br/><br/>

### 🛠️ Lab Setup
| Component | Description | 
| Test Network | 1 Attacker VM, 1 Victim VM (e.g., Kali + Windows) | 
| OS & Tools | Kali Linux with arpspoof, wireshark, iptables | 
| Network Configuration | Same subnet, no dynamic port security | 
| Traffic Generator | Use ping, curl, or a web browser on victim | 


<br/>


### 🧪 Attack Workflow
#### 1. Enable IP forwarding
echo 1 > /proc/sys/net/ipv4/ip_forward


#### 2. Launch ARP spoof against victim and gateway
arpspoof -i eth0 -t [victim_ip] [gateway_ip]
arpspoof -i eth0 -t [gateway_ip] [victim_ip]


#### 3. Capture traffic (e.g., credentials) with Wireshark
<br/>


### 📁 Files Included
- demo_notes.md: Step-by-step walkthrough
- lab_topology.png: Network diagram
- wireshark_capture.pcap: Sample packet dump (sanitized)
- README.md: This overview









