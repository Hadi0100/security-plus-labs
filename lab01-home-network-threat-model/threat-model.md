# Threat Model

## Asset Inventory

| Asset | Type | Importance | Notes |
|------|------|------------|------|
| ISP Modem | Network Device | High | Internet entry point |
| WiFi Router | Network Device | High | NAT, firewall, routing |
| Windows Desktop | Endpoint | High | Personal data and accounts |
| Laptop | Endpoint | Medium | Browsing and light work |
| Smartphone | Endpoint | High | MFA, banking, email |
| Smart TV | IoT | Medium | Rarely patched |
| VR Headset | IoT / Endpoint | Medium | WiFi connected gaming |

---

## Network Layout (Logical)

Internet  
→ ISP Modem  
→ WiFi Router (Firewall + NAT)  
→ Internal Network  
  • PCs / Phone  
  • IoT Devices  

---

## Attack Surface / Entry Points
- WiFi wireless access
- Router administrative interface
- UPnP service
- IoT device firmware
- User-installed applications
- Phishing and social engineering

---

## Threats, Vulnerabilities, and Controls

| Threat Scenario | Vulnerability | Likelihood | Impact | Risk | Controls / Mitigations |
|---|---|---|---|---|---|
| Unauthorized WiFi access | Weak passphrase / WPS enabled | Medium | High | High | Strong passphrase, disable WPS, WPA3 |
| Router exploitation | Outdated firmware | Low | High | Medium | Firmware updates, disable remote admin |
| Malware infection | Unsafe downloads | Medium | High | High | Defender AV, least privilege |
| IoT compromise | Default credentials | Medium | Medium | Medium | Change passwords, isolate on guest network |
| Phishing attack | No MFA on accounts | Medium | High | High | Enable MFA, awareness training |

---

## Risk Summary
Highest risks include unauthorized wireless access, phishing attacks, and malware infections due to user behavior and device exposure.
