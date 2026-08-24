| Step No. | Command | Explanation | Output of the Command | Takeaway |
|---|---|---|---|---|
| **1** | `nmap -sV <IP>` | Scan the target to identify open ports and services. | **[Screenshot of Nmap output]** | Ports **22** and **80** are open, so SSH and HTTP should be investigated. |
| **2** | `curl http://<IP>` | Retrieve the web server's response. | **[Screenshot of terminal output]** | The web server is accessible and returns a webpage. |
| **3** | `gobuster dir ...` | Enumerate directories on the web server. | **[Screenshot of Gobuster output]** | `/admin` was discovered and should be investigated. |
| **4** | **Browser** | Investigate the discovered `/admin` endpoint. | **[Screenshot of webpage]** | The page contains a login form. |