## Firewall in detail..

> Firewall basically checks the IP SRC  protocol port and compares it with the rule set and accordingly allows or drops the request.

## Types of firewall 

1. Packet filtering firewall ( Basic firewall)
2. Stateful Inspection Firewall
3. Application Layer Firewall (Proxy Firewall)
4. Next Generation Firewall (NGFW)



##  Packet filtering firewall ( Basic firewall)

firewall of old times it just checked rules and did not do packet inspection 
it was Very fast but Cannot detect attacks inside allowed ports 


## Stateful Inspection Firewall

Stateful Inspection Firewall are a bit smarter cause they check the whole conversation between two system and also keep record of it and if something suspiciuse is found it will block it but its not too smart to detect a hidden maliciuse intention or something like encoded payload.




## Next Generation Firewall (NGFW)



Modern enterprise firewall = all in one:

Features:

- Deep packet inspection
    
- IDS/IPS
    
- App awareness
    
- User identity
    
- Malware detection
    
- SSL inspection
  
  # Firewall – Simple Explanation

## What is a Firewall?
A firewall is a security system that **monitors and controls network traffic** based on rules.  
It acts like a **security guard** between your device/network and the internet.

### Main Purpose
- Block unauthorized access  
- Allow legitimate communication  
- Protect from hackers and malware

---

## How Firewall Works

1. It **inspects traffic** (IP, port, protocol, application)
2. Matches it with **rules**
3. Takes action:
   - Allow  
   - Block/Drop  
   - Reject  
   - Log

### Example Rule
- Allow: Web traffic → port 80, 443  
- Block: Remote access → port 3389 from internet  
- Allow: Internal network → internet

---

## Types of Firewall

### 1. Packet Filtering Firewall
- Checks only:
  - Source IP  
  - Destination IP  
  - Port  
  - Protocol  
- Fast but not very intelligent.

### 2. Stateful Firewall
- Tracks connections  
- Understands TCP handshake  
- Allows return traffic automatically  
- Most commonly used today.
--- 

### 3. Application Layer Firewall
- Understands applications like:
  - HTTP  
  - DNS  
  - FTP  
- Can block URLs, file types, commands.
--- 
### 4. Next Generation Firewall (NGFW)
- Advanced modern firewall  
- Includes:
  - IDS/IPS  
  - Malware detection  
  - User identity  
  - Deep inspection

---

## Hardware vs Software Firewall

### Hardware Firewall
- Physical device  
- Protects whole network  
- Used in companies  
- Example: Fortinet, Cisco, Router firewall
---

### Software Firewall
- Installed on one system  
- Protects only that device  
- Example: Windows Firewall, iptables, ufw

> Easy Memory  
> Hardware = main gate  
> Software = door lock

---

## Firewall Actions

- DROP → silently discard  
- REJECT → send error reply  
- ALLOW → permit traffic  
- LOG → record event

---

## Best Practice

- Default Deny policy  
- Allow only required ports  
- Separate zones:
  - LAN  
  - WAN  
  - DMZ

---

## What Firewall Can Block

- Port scanning  
- Unauthorized login  
- Malware communication  
- Brute force  
- Suspicious IPs

## What Firewall Cannot Stop

- Social engineering  
- Insider misuse  
- Encrypted threats (without inspection)

---

## SOC Analyst View

You analyze:
- Which rule blocked traffic  
- False positive or attack  
- Source IP reputation  
- Repeated attempts
