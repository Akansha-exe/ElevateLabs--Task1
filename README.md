Task 1 – Scan Your Local Network for Open Ports

Objective
To scan my local network using Nmap and identify active hosts and open TCP ports.

Tool Used
- Nmap

Command Used
```bash
nmap -sS 192.168.1.0/24
```

 Results

 Active Hosts
- 192.168.1.4
- 192.168.1.5
- 192.168.1.6
- 192.168.1.9

 Open Ports
**192.168.1.5**
- 135/tcp – MSRPC
- 139/tcp – NetBIOS Session Service
- 445/tcp – Microsoft-DS (SMB)

**192.168.1.6**
- 9080/tcp – Filtered

Security Risks
- Open ports increase the attack surface.
- SMB (Port 445) should only be accessible on trusted networks.
- Firewalls should restrict unnecessary access.
- Systems should be regularly updated.

## Outcome
Successfully performed a TCP SYN scan using Nmap and analyzed the exposed network services.
