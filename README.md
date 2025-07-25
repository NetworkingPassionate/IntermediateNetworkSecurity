# IntermediateNetworkSecurity
This is a set of intermediate network security tasks!


## 🌐 TCP Port Scanner (Python)
A Python-based tool to check host availability and scan for open TCP ports within a configurable range. Designed for a friendly GUI, speed, and diagnostic feedback.
- 🔍 Scans individual IPs or hostnames across user-defined port ranges
- ⚙️ Validates input with clean error handling and prompt feedback
- ⏱️ Uses socket timeouts to optimize performance and detect filtered vs. closed ports
- 💬 Console interaction enhanced with status messages and result formatting
- 🛠️ Tools Used: Python 3, socket, CLI prompts
- 📊 Outcome: Confirms host reachability and port exposure, useful for diagnostics or ethical pen-testing

  This is our home-page menu. 
<img width="631" height="432" alt="image" src="https://github.com/user-attachments/assets/e45be81c-4019-411e-931b-fed4c64eefd9" />

This TCP-scanner will go through the range, informing the user of open ports.
<img width="486" height="263" alt="image" src="https://github.com/user-attachments/assets/f774c0df-8aba-4256-8daa-da32169212b6" />

As you can see, this web server has an open port 80 (HTTP), which may be a sign it's redirecting traffic to port 443 for backwards compatibillity of old browsers, but could also be a sign that they're accepting un-encrypted traffic through it. 
