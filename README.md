## 🎯 Why This Matters for Cybersecurity Roles
This lab demonstrates hands-on skills in:
- Network segmentation (NIST SP 800-53 AC-4)
- Access control (NIST SP 800-192)
- Secure remote access (CIS Control 12)
-
- # 🌐 Enterprise Network Fortification Project

**Cisco Packet Tracer | Network Security | Zero Trust Architecture**

[![Cisco Certified](https://img.shields.io/badge/Cisco_Networking_Academy-Student-blue?logo=cisco)](https://www.netacad.com)
[![Security Focused](https://img.shields.io/badge/Security-Hardened-orange)](https://owasp.org)

## 🔐 Security Features Implemented
- **VLAN Segmentation** (Isolated Finance/HR/Guest networks)
- **ACLs** blocking:
  - ICMP between departments
  - Unauthorized SSH access
- **Site-to-Site VPN** with AES-256 encryption
- **Port Security** on all access switches

## 📦 Repository Contents
```
/enterprise-network-lab/
├── enterprise_secure.pkt          # Packet Tracer file
├── /configs/
│   ├── core_router_acl.txt        # Access control lists
│   └── vpn_gateway_config.txt     # Crypto map settings
├── /screenshots/
│   ├── topology.png               # Network diagram
│   └── vpn_status.png             # Tunnel verification
```

## 🛠️ How to Test Security Controls
1. Open `enterprise_secure.pkt` in Packet Tracer
2. Attempt ping between VLANs (should fail per ACLs)
3. Verify VPN tunnel status: `show crypto session`

## 🔍 Security Analysis
**Threats Mitigated:**
- Lateral movement via VLAN hopping
- Unauthorized access to financial systems
- Eavesdropping on inter-site traffic

**OWASP Top 10 Relevance:**
- A1: Broken Access Control (prevented via ACLs)
- A2: Cryptographic Failures (addressed with VPN)
