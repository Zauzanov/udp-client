<p align="center">
  <h1 align="center"> UDP-client </h1>
</p>

## 🚀 Quick Start
## 1. Download 'udp-client.py' file and specify an IP-address and port.
## 2. Get some UDP-ports from Metasploitable 2, which is an intentionally vulnerable Ubuntu Linux virtual machine that is designed for testing common vulnerabilities:
```bash
nmap -sU --top-ports 100 192.168.204.129
Starting Nmap 7.95 ( https://nmap.org ) at 2025-10-28 04:26 EDT
Nmap scan report for 192.168.204.129
Host is up (0.00083s latency).
Not shown: 93 closed udp ports (port-unreach)
PORT     STATE         SERVICE
53/udp   open          domain
68/udp   open|filtered dhcpc
69/udp   open|filtered tftp
111/udp  open          rpcbind
137/udp  open          netbios-ns
138/udp  open|filtered netbios-dgm
2049/udp open          nfs
MAC Address: 00:0C:29:0A:12:6B (VMware)

Nmap done: 1 IP address (1 host up) scanned in 110.98 seconds
```
## 3. Run the script using Python interpretator: 
```bash
 python udp-client.py
```
## 4. If no response arrives, the program will hang forever here (because no timeout is set).
