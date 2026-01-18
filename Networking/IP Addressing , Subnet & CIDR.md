

## How many IPs in IPv4?

- IPv4 address = **32 bits**
- 8 bits = **1 byte**
- Example:
  - If **24 bits** are fixed for network  
  - Remaining bits = **32 − 24 = 8 bits**
  - Total IPs = **2⁸ = 256 IPs**

---

## Common Ports & Protocols

| Port | Protocol | Use |
|-----:|----------|-----|
| 20 / 21 | FTP | File transfer |
| 22 | SSH | Secure shell |
| 23 | Telnet | Insecure remote login |
| 25 | SMTP | Send mail |
| 53 | DNS | Name resolution |
| 67 / 68 | DHCP | IP assignment |
| 80 | HTTP | Web (unsecure) |
| 443 | HTTPS | Secure web |
| 110 | POP3 | Receive mail |
| 143 | IMAP | Receive mail |
| 3389 | RDP | Remote desktop |
| 445 | SMB | Windows file sharing |
| 389 | LDAP | Directory access |
| 636 | LDAPS | Secure LDAP |
| 88 | Kerberos | Authentication |

---

## Kerberos (Short & Clear)

> [!note]
> - Uses **tickets** to verify user identity  
> - No password sent over network  
> - Provides **SSO (Single Sign-On)**  
> - Works on multiple OS and cloud environments  

---

## Classful Routing (Old Method)

- IPs were divided into **fixed classes**
  - **Class A:** 1.0.0.0 – 126.255.255.255
  - **Class B:** 128.0.0.0 – 191.255.255.255
  - **Class C:** 192.0.0.0 – 223.255.255.255
- Problem:
  - Large **IP wastage**
  - Even if few IPs needed, whole class was assigned

---

## CIDR (Classless Inter-Domain Routing)

> [!info]
> CIDR is a method for **efficient IP allocation and routing**

- No IP classes (A, B, C not used)
- Uses **slash notation**
  - Example: `192.168.2.0/28`
- `/28` means:
  - First **28 bits** = network
  - Remaining **4 bits** = host

### CIDR Calculation Example

- Total IPs = **2⁴ = 16**
- Usable IPs = **14**
- Network IP = `192.168.2.0`
- Broadcast IP = `192.168.2.15`

---

## Subnetting (Simple Definition)

- Subnetting = **dividing one network into multiple smaller networks**
- Improves:
  - IP usage
  - Network performance
  - Security

---

## Important Terms

- **MSB:** Most Significant Bit  
- **Switch:** Connects devices within the **same network**  
- **Router:** Connects **different networks**

---

## Classful vs CIDR (One-Line Difference)

- **Classful routing:** Fixed classes (A, B, C)
- **CIDR:** Flexible masks like `/24`, `/28`, `/30`